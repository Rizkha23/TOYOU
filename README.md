body {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(135deg, #e0f2fe 0%, #dcfce7 35%, #fef9c3 65%, #ffe4e6 100%);
  background-size: 300% 300%;
  animation: pastelShift 12s ease infinite;
  padding: 20px;
  overflow: hidden;
  position: relative;
  color: #334155;
}

@keyframes pastelShift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* Ambient Glowing Pastel Lights */
.light-glow {
  position: fixed;
  border-radius: 50%;
  filter: blur(80px);
  opacity: 0.6;
  pointer-events: none;
}

.glow-1 {
  width: 320px;
  height: 320px;
  background: radial-gradient(circle, #fbcfe8 0%, rgba(251, 207, 232, 0) 70%);
  top: -5%;
  left: -5%;
}

.glow-2 {
  width: 350px;
  height: 350px;
  background: radial-gradient(circle, #bbf7d0 0%, rgba(187, 247, 208, 0) 70%);
  bottom: -5%;
  right: -5%;
}

/* Container Partikel Cahaya Background */
.bg-sparkle-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 1;
  overflow: hidden;
}

.floating-bg-sparkle {
  position: absolute;
  bottom: -20px;
  border-radius: 50%;
  background: radial-gradient(circle, #ffffff 0%, #fda4af 60%, rgba(253, 164, 175, 0) 100%);
  box-shadow: 0 0 10px #ffffff, 0 0 20px #fda4af;
  pointer-events: none;
  opacity: 0;
  animation: floatBgSparkle var(--duration) ease-in-out infinite;
  animation-delay: var(--delay);
}

@keyframes floatBgSparkle {
  0% { opacity: 0; transform: translateY(0) scale(0.5); }
  30% { opacity: 0.8; }
  70% { opacity: 0.8; }
  100% { opacity: 0; transform: translateY(-105vh) scale(1.5); }
}

/* Outer Wrapper */
.wrapper {
  width: 100%;
  max-width: 360px;
  z-index: 2;
}

/* Card Styling */
.card {
  display: none;
  background: rgba(255, 255, 255, 0.85);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  border-radius: 24px;
  padding: 24px;
  text-align: center;
  box-shadow: 0 15px 35px rgba(148, 163, 184, 0.25),
              inset 0 1px 1px rgba(255, 255, 255, 0.9);
  border: 1px solid rgba(255, 255, 255, 0.7);
  width: 100%;
}

.card.active {
  display: block;
  animation: fadeIn 0.5s cubic-bezier(0.16, 1, 0.3, 1) forwards;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px) scale(0.96); }
  to { opacity: 1; transform: translateY(0) scale(1); }
}

/* TAMPILAN ENVELOPE / SURAT DEPAN */
.envelope-card {
  background: rgba(255, 255, 255, 0.9);
  border-radius: 24px;
  padding: 30px 20px;
  text-align: center;
  cursor: pointer;
  box-shadow: 0 15px 35px rgba(244, 63, 94, 0.15);
  border: 2px dashed #fda4af;
  transition: all 0.3s ease;
}

.envelope-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 40px rgba(244, 63, 94, 0.25);
}

.envelope-icon {
  font-size: 4.5rem;
  margin-bottom: 10px;
  display: inline-block;
  animation: pulseHeart 1.5s infinite alternate;
  filter: drop-shadow(0 4px 10px rgba(244, 63, 94, 0.3));
}

@keyframes pulseHeart {
  0% { transform: scale(1); }
  100% { transform: scale(1.15); }
}

/* KALENDER STYLING */
.calendar-box {
  background: #ffffff;
  border-radius: 16px;
  padding: 16px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.06);
  margin-bottom: 20px;
  border: 1px solid #f1f5f9;
}

.calendar-header {
  font-weight: 700;
  color: #f43f5e;
  font-size: 1.1rem;
  margin-bottom: 12px;
  letter-spacing: 0.5px;
}

.calendar-grid {
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  gap: 6px;
  text-align: center;
  font-size: 0.85rem;
}

.day-name {
  font-weight: 600;
  color: #94a3b8;
  font-size: 0.75rem;
  padding-bottom: 4px;
}

.day-num {
  padding: 8px 0;
  color: #475569;
  border-radius: 50%;
  position: relative;
}

.day-num.empty {
