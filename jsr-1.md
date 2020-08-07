# JSR-1: Basic Conding Standard

## Constants

Constants are commonly used to define the default configuration of a program, module, class, function or component.

```javascript
const DEFAULT_PROPS = {
  name: 'Kaluã Bentes',
  birthday: '1992-12-29'
}

const INITIAL_STATE = {
  orientation: Orientation.Landscape,
}

const APP_TITLE = 'Facebook'

const COLOR_WHITE = '#fffff'
```

Always use uppcased words to highlight that that constant is a default configuration.

## Enums

Enums are data types that define an finite number of options or choices.

```javascript

const Align = {
  Center: 'CENTER',
  Right: 'RIGHT',
  Left: 'LEFT'
}
```

Always use PascalCase to name an enum and its keys options, use uppercase for choice values.

## Interface

Interfaces are used to define the api contract of a entity.

```javascript
const Props = {
  avatar: PropTypes.string,
  name: PropTypes.string,
}

export default function User({avatar, name}) {
  return (
    <Container>
      <Avatar src={avatar} alt={name} />
      <Name>{name}</Name>
    </Container>
  );
}

User.propTypes = Props;
```

Always use PascalCase to name an interface, the keys represents the shape of the api of a object or component.
