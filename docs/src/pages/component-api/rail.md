# Rail

The `Rail` component is used as a child of `Slider` to render your rail content.
The only motivation for using this component is to hook the rail into the slider events.
If you don't want to have the handles move when the user clicks on the rail then just render your rail as a direct child of `Slider`.

### Example Usage:
```jsx
import Slider, { Rail } from 'react-compound-slider'

<Slider
  ...
>
  <Rail>
    {({ getRailProps }) => (
      <div style={railStyle} {...getRailProps()} /> // the rail props will make the rail clickeable
    )}
  </Rail>
  ...
</Slider>
```