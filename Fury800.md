# Таблица параметров для разработки UI/UX VST3 плагина Fury800

## Основная информация
| Параметр | Значение |
|----------|----------|
| **Название плагина** | Fury800 |
| **Всего параметров** | 2160 |
| **Аудио параметров** | 300 |
| **Путь к плагину** | /Library/Audio/Plug-Ins/VST3/Fury800.vst3 |

---

## Категории параметров для интерфейса

### 1. 🎛️ OSCILLATORS (Осцилляторы) - 18 параметров
| ID | Название | Default | Automatable | Группа |
|----|----------|---------|-------------|--------|
| 5 | DCO1 Octave | 0.5 | ✅ | DCO1 |
| 6 | DCO1 Waveform | 1.0 | ✅ | DCO1 |
| 7 | DCO1 16' | 1.0 | ✅ | DCO1 |
| 8 | DCO1 8' | 1.0 | ✅ | DCO1 |
| 9 | DCO1 4' | 1.0 | ✅ | DCO1 |
| 10 | DCO1 2' | 1.0 | ✅ | DCO1 |
| 11 | DCO1 Level | 1.0 | ✅ | DCO1 |
| 13 | DCO2 Octave | 0.5 | ✅ | DCO2 |
| 14 | DCO2 Waveform | 1.0 | ✅ | DCO2 |
| 15 | DCO2 16' | 1.0 | ✅ | DCO2 |
| 16 | DCO2 8' | 1.0 | ✅ | DCO2 |
| 17 | DCO2 4' | 1.0 | ✅ | DCO2 |
| 18 | DCO2 2' | 1.0 | ✅ | DCO2 |
| 19 | DCO2 Level | 1.0 | ✅ | DCO2 |
| 20 | DCO2 Interval | 0.0 | ✅ | DCO2 |
| 21 | DCO2 Detune | 0.0 | ✅ | DCO2 |
| 22 | Noise Level | 0.0 | ✅ | Noise |
| 12 | DCO Mode | 0.0 | ✅ | Mode |

### 2. 🔊 FILTERS (Фильтры) - 2 параметра
| ID | Название | Default | Automatable |
|----|----------|---------|-------------|
| 23 | VCF Cutoff | 1.0 | ✅ |
| 24 | VCF Resonance | 0.0 | ✅ |
| 25 | VCF KBD Track | 0.0 | ✅ |
| 26 | VCF EG Polarity | 1.0 | ✅ |
| 27 | VCF EG Intensity | 0.0 | ✅ |
| 28 | VCF Trigger | 1.0 | ✅ |

### 3. 📈 ENVELOPES (Огибающие) - 12 параметров
| ID | Название | Default | Automatable | Группа |
|----|----------|---------|-------------|--------|
| 30 | DEG1 Attack | 0.0 | ✅ | ENV1 |
| 31 | DEG1 Decay | 0.0 | ✅ | ENV1 |
| 32 | DEG1 Break Point | 1.0 | ✅ | ENV1 |
| 33 | DEG1 Slope | 0.0 | ✅ | ENV1 |
| 34 | DEG1 Sustain | 1.0 | ✅ | ENV1 |
| 35 | DEG1 Release | 0.0 | ✅ | ENV1 |
| 36 | DEG2 Attack | 0.0 | ✅ | ENV2 |
| 37 | DEG2 Decay | 0.0 | ✅ | ENV2 |
| 38 | DEG2 Break Point | 1.0 | ✅ | ENV2 |
| 39 | DEG2 Slope | 0.0 | ✅ | ENV2 |
| 40 | DEG2 Sustain | 1.0 | ✅ | ENV2 |
| 41 | DEG2 Release | 0.0 | ✅ | ENV2 |
| 42-47 | DEG3 (Attack/Decay/BP/Slope/Sustain/Release) | 0.0 | ✅ | ENV3 |

### 4. 🎭 MODULATION (Модуляция) - 6 параметров
| ID | Название | Default | Automatable |
|----|----------|---------|-------------|
| 48 | MG Frequency | 0.53 | ✅ |
| 49 | MG Delay | 0.0 | ✅ |
| 50 | MG DCO | 0.0 | ✅ |
| 51 | MG VCF | 0.0 | ✅ |
| 58 | Mod.Wheel to DCO | 0.0 | ✅ |
| 59 | Mod.Wheel to VCF | 0.0 | ✅ |

### 5. 🎪 EFFECTS (Эффекты) - 4 параметра
| ID | Название | Default | Automatable |
|----|----------|---------|-------------|
| 29 | Chorus | 0.0 | ✅ |
| 57 | Stereo Chorus | 0.0 | ✅ |
| 61 | Chorus Rate | 0.13 | ✅ |
| 4 | Mode | 0.0 | ✅ |

### 6. 🎚️ MASTER (Мастер) - 3 параметра
| ID | Название | Default | Automatable |
|----|----------|---------|-------------|
| 0 | Volume | 0.5 | ✅ |
| 63 | Gain Boost | 1.0 | ✅ |
| 64 | Brightness | 1.0 | ✅ |

### 7. ⚙️ OTHER (Другие) - 8 параметров
| ID | Название | Default | Automatable |
|----|----------|---------|-------------|
| 1 | Tune | 0.5 | ✅ |
| 2 | Bend | 0.17 | ✅ |
| 3 | Seq. Frequency | 0.50 | ✅ |
| 52 | Seq. Clock | 0.0 | ✅ |
| 53 | Seq. Play On Note | 0.0 | ✅ |
| 54 | Seq. Transpose | 0.0 | ✅ |
| 55 | Voices | 0.0 | ✅ |
| 56 | God Mode | 0.0 | ✅ |
| 60 | Velocity | 0.0 | ✅ |
| 62 | Legacy Mode | 1.0 | ✅ |

---

## 🎨 Рекомендации для UI/UX

### Структура интерфейса
```
┌─────────────────────────────────────────────────────────────┐
│  [MASTER] Volume │ Gain │ Brightness                        │
├─────────────┬─────────────┬─────────────┬───────────────────┤
│  OSCILLATOR │   FILTER    │  ENVELOPES  │    MODULATION     │
│     DCO1    │   Cutoff    │    ENV1     │    LFO            │
│     DCO2    │  Resonance  │    ENV2     │    Wheel          │
│    Noise    │   KBD Track │    ENV3     │                   │
├─────────────┴─────────────┴─────────────┴───────────────────┤
│  [EFFECTS] Chorus │ Stereo │ Rate                           │
├─────────────────────────────────────────────────────────────┤
│  [SEQUENCER] Freq │ Clock │ Play │ Transpose │ Voices       │
└─────────────────────────────────────────────────────────────┘
```

### Цветовая схема (рекомендация)
| Секция | Цвет |
|--------|------|
| Oscillators | 🔵 Синий |
| Filter | 🟢 Зелёный |
| Envelopes | 🟠 Оранжевый |
| Modulation | 🟣 Фиолетовый |
| Effects | 🟡 Жёлтый |
| Master | 🔴 Красный |

### Приоритет параметров для отображения
1. **Высокий приоритет**: Volume, Cutoff, Resonance, DCO Waveforms, ENV ADSR
2. **Средний приоритет**: Chorus, LFO, DCO Levels, Detune
3. **Низкий приоритет**: Seq. parameters, God Mode, Legacy Mode

---

## 📊 Статистика по категориям
| Категория | Кол-во параметров | % от общих |
|-----------|-------------------|------------|
| Effects | 116 | 5.4% |
| Modulation | 102 | 4.7% |
| Other | 32 | 1.5% |
| Master | 18 | 0.8% |
| Oscillators | 18 | 0.8% |
| Envelopes | 12 | 0.6% |
| Filters | 2 | 0.1% |
| **MIDI CC (скрытые)** | **1870** | **86.6%** |

Эта таблица поможет вам организовать разработку интерфейса VST3 плагина эффективно! 🎹
