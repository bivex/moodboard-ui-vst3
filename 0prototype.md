# 🔘 Fury800: Состояния кнопок (Button States Specification)

> ✅ Checklist-style, категория за категорией  
> 🎯 Формат именования PNG: `Fury800_[Category]_[Button]_[State]_[Theme].png`

---

## 🧭 Типология кнопок в Fury800

| Тип кнопки | Примеры | Поведение |
|------------|---------|-----------|
| **Toggle** | Chorus On/Off, God Mode | Вкл/Выкл, запоминает состояние |
| **Momentary** | Seq. Play On Note | Активна только при нажатии |
| **Radio/Segmented** | DCO Waveform, VCF Trigger | Выбор одного из нескольких |
| **Stepper** | Voices (1→8), Octave (-2→+2) | Циклическое переключение |
| **Menu Trigger** | Waveform Selector (dropdown) | Открывает popup-меню |
| **Bypass** | Effect Bypass | Альтернативный toggle с индикацией |

---

## 📋 Универсальные состояния (для всех кнопок)

```
✅ Default          — обычное состояние
✅ Hover           — курсор над кнопкой
✅ Pressed/Active  — кнопка нажата (mouse down)
✅ Focused         — фокус клавиатуры (Tab navigation)
✅ Disabled        — неактивна (grayed out)
✅ AutomationOn    — параметр автоматизирован в DAW
✅ ValueChanged    — значение изменено от default (визуальный акцент)
```

> 🎨 **Визуальные маркеры состояний:**
> - `Hover`: +10% brightness, subtle glow
> - `Pressed`: -15% brightness, inner shadow, 1px shift down
> - `Focused`: 2px outer ring (color by section)
> - `AutomationOn`: pulsing blue ring (1px, 2Hz)
> - `ValueChanged`: small dot indicator ● top-right

---

## 🎛️ Состояния по категориям (PNG Naming)

### 1. 🎛️ OSCILLATORS

#### Waveform Selector (Radio Group)
```
Fury800_Oscillators_Waveform_Sine_Default_Dark.png
Fury800_Oscillators_Waveform_Sine_Selected_Dark.png
Fury800_Oscillators_Waveform_Sine_Hover_Dark.png
Fury800_Oscillators_Waveform_Sine_Disabled_Dark.png

Fury800_Oscillators_Waveform_Saw_Default_Dark.png
Fury800_Oscillators_Waveform_Saw_Selected_Dark.png
... (repeat for Pulse, Noise, Triangle)
```

#### Footage Toggles (16'/8'/4'/2') — Toggle Buttons
```
Fury800_Oscillators_Footage_16_Off_Default.png
Fury800_Oscillators_Footage_16_On_Default.png
Fury800_Oscillators_Footage_16_On_Hover.png
Fury800_Oscillators_Footage_16_On_Pressed.png
Fury800_Oscillators_Footage_16_On_Automation.png
Fury800_Oscillators_Footage_16_Off_Disabled.png
```

#### DCO Mode Switch (Segmented)
```
Fury800_Oscillators_Mode_Poly_Selected.png
Fury800_Oscillators_Mode_Unison_Selected.png
Fury800_Oscillators_Mode_Duo_Selected.png
Fury800_Oscillators_Mode_Segment_Hover.png
```

---

### 2. 🔊 FILTERS

#### VCF Trigger (Radio: Gate/Retrig/Legato)
```
Fury800_Filters_Trigger_Gate_Default.png
Fury800_Filters_Trigger_Gate_Selected.png
Fury800_Filters_Trigger_Legato_Selected.png
Fury800_Filters_Trigger_Segment_Hover.png
```

#### EG Polarity Toggle (±)
```
Fury800_Filters_EG_Polarity_Pos_On.png
Fury800_Filters_EG_Polarity_Pos_Off.png
Fury800_Filters_EG_Polarity_Neg_On.png
Fury800_Filters_EG_Polarity_Neg_Off.png
Fury800_Filters_EG_Polarity_Toggle_Hover.png
```

---

### 3. 🎭 MODULATION

#### LFO Waveform Selector
```
Fury800_Modulation_LFO_Wave_Sine_Selected.png
Fury800_Modulation_LFO_Wave_Triangle_Selected.png
Fury800_Modulation_LFO_Wave_Square_Selected.png
Fury800_Modulation_LFO_Wave_Random_Selected.png
Fury800_Modulation_LFO_Wave_Segment_Disabled.png
```

#### Mod Wheel Routing Slots
```
Fury800_Modulation_WheelSlot_Empty_Default.png
Fury800_Modulation_WheelSlot_Assigned_Default.png
Fury800_Modulation_WheelSlot_Assigned_Hover.png
Fury800_Modulation_WheelSlot_DragPreview.png  ← при перетаскивании
```

---

### 4. 🎪 EFFECTS

#### Chorus Bypass Toggle
```
Fury800_Effects_Chorus_Bypass_Off_Default.png
Fury800_Effects_Chorus_Bypass_On_Default.png
Fury800_Effects_Chorus_Bypass_On_Glow.png      ← активный эффект
Fury800_Effects_Chorus_Bypass_Hover.png
Fury800_Effects_Chorus_Bypass_Automation.png
```

#### Stereo Toggle
```
Fury800_Effects_Stereo_Toggle_Off.png
Fury800_Effects_Stereo_Toggle_On.png
Fury800_Effects_Stereo_Toggle_On_Pulsing.png   ← при изменении в реальном времени
```

---

### 5. ⚙️ GLOBAL / OTHER

#### God Mode / Legacy Mode (Warning Toggles)
```
Fury800_Global_GodMode_Off_Default.png
Fury800_Global_GodMode_On_Default.png
Fury800_Global_GodMode_On_Warning.png          ← красный пульсирующий контур
Fury800_Global_GodMode_ConfirmOverlay.png      ← popup-подтверждение
```

#### Seq. Clock Source (Radio: Internal/MIDI/USB)
```
Fury800_Global_SeqClock_Internal_Selected.png
Fury800_Global_SeqClock_MIDI_Selected.png
Fury800_Global_SeqClock_USB_Disabled.png       ← если не подключено
```

#### Voices Stepper (1→2→4→8)
```
Fury800_Global_Voices_Stepper_Dec_Default.png
Fury800_Global_Voices_Stepper_Dec_Hover.png
Fury800_Global_Voices_Stepper_Dec_Disabled.png ← при min value
Fury800_Global_Voices_Stepper_Inc_Default.png
Fury800_Global_Voices_Stepper_Inc_Hover.png
Fury800_Global_Voices_Stepper_Inc_Disabled.png ← при max value
Fury800_Global_Voices_Display_Value_8.png      ← текущее значение
```

---

## 🎨 Визуальная спецификация состояний

### Цветовые токены по состояниям:
```css
/* Base button */
--btn-bg-default: #2A2A2A;
--btn-bg-hover: #3A3A3A;
--btn-bg-pressed: #1A1A1A;
--btn-bg-disabled: #1F1F1F;
--btn-border-default: #444444;
--btn-border-hover: #666666;
--btn-border-focused: var(--color-section); /* по секции */

/* Toggle ON states */
--btn-toggle-on-bg: var(--color-section);    /* синий/зелёный и т.д. */
--btn-toggle-on-text: #FFFFFF;
--btn-toggle-on-glow: rgba(74, 144, 226, 0.4);

/* Automation indicator */
--automation-ring: #4A90E2;
--automation-pulse: 0 0 0 1px var(--automation-ring), 
                    0 0 8px 2px rgba(74, 144, 226, 0.6);

/* Value changed indicator */
--value-dot: #F5A623;  /* оранжевая точка */
```

### Анимации (для прототипа/dev):
| Состояние | Длительность | Easing | Примечание |
|-----------|--------------|--------|------------|
| Hover → Default | 150ms | ease-out | плавное затухание glow |
| Pressed → Default | 100ms | ease-in | быстрый отскок |
| AutomationOn pulse | 500ms цикл | linear | бесконечный pulse |
| ValueChanged dot appear | 200ms | ease-out | fade-in + scale |

---

## 📐 Размеры и отступы (Pixel Perfect)

```
🔘 Standard Toggle Button:
- Size: 28×28px (icon), 48×24px (text toggle)
- Border radius: 4px
- Icon padding: 6px
- Hit area: 32×32px (для удобства)

🔘 Segmented Control:
- Segment width: 40px
- Height: 24px
- Border radius: 3px (outer), 0 (inner)
- Divider: 1px #333

🔘 Stepper:
- Arrow btn: 20×20px
- Display: 32×20px
- Gap between: 4px
```

---

## 🗂️ Экспорт PNG: Чеклист по папкам

```
03_States_Variants/
├── Oscillators/
│   ├── Waveform/
│   │   ├── Fury800_Oscillators_Waveform_[Type]_[State]_[Theme].png
│   │   └── ...
│   ├── Footage/
│   │   └── Fury800_Oscillators_Footage_[Value]_[OnOff]_[State].png
│   └── Mode/
│       └── Fury800_Oscillators_Mode_[Mode]_[State].png
├── Filters/
│   ├── Trigger/
│   └── Polarity/
├── Modulation/
│   ├── LFO_Waveform/
│   └── WheelSlot/
├── Effects/
│   └── Bypass_Toggles/
├── Global/
│   ├── GodMode/
│   ├── SeqClock/
│   └── Voices_Stepper/
└── _System/
    ├── Fury800_BTN_Hover_Glow_Overlay.png      ← reusable effect
    ├── Fury800_BTN_Automation_Ring.png         ← reusable ring
    ├── Fury800_BTN_ValueChanged_Dot.png        ← reusable indicator
    └── Fury800_BTN_Focus_Ring_Blue.png         ← accessibility
```

---

## 🔄 Особые случаи и edge cases

### 1. **Multi-select Footage toggles** (можно включить несколько):
```
✅ State: Multiple_On (16'+8' active)
→ PNG: Fury800_Oscillators_Footage_Multi_16_8_On.png
→ Visual: Both buttons highlighted, subtle connector line
```

### 2. **Modulation matrix drag-and-drop**:
```
✅ State: DragPreview (полупрозрачный clone)
✅ State: DropTarget_Highlight (подсветка слота)
✅ State: InvalidDrop (красный крестик)
```

### 3. **God Mode confirmation**:
```
✅ State: WarningPulse (красный пульсирующий контур)
✅ State: ConfirmOverlay (modal: "Are you sure?")
✅ State: Confirmed_Flash (brief white flash on enable)
```

### 4. **MIDI Learn mode**:
```
✅ State: Learning_Mode (кнопка мигает жёлтым)
✅ State: MIDI_Assigned (зелёная точка + CC# label)
✅ PNG: Fury800_BTN_MIDILearn_Active_Pulsing.png
```

---

## 🚀 Quick Checklist: Реализация состояний

```markdown
[ ] Создать master-компонент кнопки с Variants (Figma/Sketch)
[ ] Настроить 6 базовых состояний: Default/Hover/Pressed/Focused/Disabled/Auto
[ ] Добавить section-specific colors через Design Tokens
[ ] Экспортировать все состояния в PNG с суффиксами _2x
[ ] Создать SpriteSheet для dev: Fury800_BTN_Sprite_AllStates.png
[ ] Документировать hit areas в Figma (red overlay layer)
[ ] Подготовить animation specs для Lottie/After Effects (если нужно)
[ ] Протестировать контраст: WCAG AA для focused state
[ ] Добавить alt-text metadata для accessibility (dev handoff)
```

---

## 📤 Dev Handoff: JSON Spec Example

```json
{
  "component": "Fury800_Oscillators_Footage_Toggle",
  "param_id": 7,
  "type": "toggle",
  "states": {
    "default": { "bg": "#2A2A2A", "border": "#444", "icon": "footage_16_off" },
    "hover": { "bg": "#3A3A3A", "border": "#666", "glow": true },
    "pressed": { "bg": "#1A1A1A", "offset_y": 1 },
    "on": { "bg": "#4A90E2", "text": "#FFF", "glow": "rgba(74,144,226,0.4)" },
    "automation": { "ring": "#4A90E2", "pulse": true, "frequency_hz": 2 }
  },
  "hit_area": { "x": 0, "y": 0, "w": 32, "h": 32 },
  "export": {
    "1x": "Fury800_Oscillators_Footage_16_[State]_1x.png",
    "2x": "Fury800_Oscillators_Footage_16_[State]_2x.png"
  }
}
```

---

> 💡 **Pro Tip**: Используйте Figma Variables + Modes для переключения тем (Dark/Light/Retro) без дублирования компонентов. Имя переменной: `btn/state/automation_ring`

Нужен шаблон Figma с готовыми Variants кнопок или CSV-манифест для批量-экспорта? Готов помочь! 🎹🔧
