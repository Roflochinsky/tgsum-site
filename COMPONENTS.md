# TGSUM components

## Tokens

| Token | Value | Purpose |
|---|---|---|
| `--paper` | `#f9efe3` | Warm page background |
| `--ink` | `#191919` | Primary text, primary button |
| `--accent` | `#f05a36` | Orange accent |
| `--muted` | `#69665f` | Secondary text |
| `--line` | `#d9cec1` | Dividers |
| `--radius` | `22px` | Large surfaces |

Manrope Variable includes Cyrillic. Layout uses 8px-inspired spacing, fluid display typography and breakpoints at 1000, 760 and 450 CSS pixels. Reduced-motion preferences disable animation and smooth scrolling.

## API

```jsx
import { Button, Badge, SectionHeading, FeatureCard, AccordionItem,
  DemoDashboard, StepTabs, CopyButton, icons } from './components';

<Button href="#demo" variant="dark">Посмотреть демо</Button>
<Badge tone="green" icon={icons.Check}>Готово к проверке</Badge>
<SectionHeading eyebrow="01 / ВОЗМОЖНОСТИ" title="Ваш заголовок">
  Короткое описание раздела.
</SectionHeading>
<FeatureCard number="01" icon={icons.ChatsCircle}
  title="Название функции" tag="ИМПОРТ">
  Описание функции.
</FeatureCard>
<AccordionItem index={1} question="Вопрос?">Ответ.</AccordionItem>
<CopyButton text="Текст для копирования" />
<StepTabs />
<DemoDashboard />
```

### Variants

- Button: `dark`, `cream`, `orange`; `href` renders a link, otherwise a button. `icon={false}` omits arrow. Native props are forwarded.
- Badge: `neutral`, `green`, `orange`, `cream`, `glass`; optional icon component.
- SectionHeading: `align="left"` or `align="center"`.
- AccordionItem: native button with `aria-expanded` / associated content.
- StepTabs: three real panels; click and arrow-key navigation.
- CopyButton: Clipboard API with visible success/error status.
- DemoDashboard: overview/tasks/sources, date filter, task checkboxes, source inspection, synthetic Markdown download.

## Accessibility and integration

Semantic landmarks, visible focus outlines, skip link, labels for icon-only controls, keyboard-operable tabs and accordions, decorative hero `alt=""`. No synthetic demo component connects to production services. Preserve its demonstration labels when reusing it publicly.

Replace synthetic content only in a separately authorized authenticated application. Do not paste user/customer conversations into this public repository.
