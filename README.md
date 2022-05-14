# NR React Hooks Snippets

![icon](./icon.png)

Code less, think more.

Folked from [react-hooks-snippets](https://github.com/alDuncanson/react-hooks-snippets)

## Supported Snippets

| Prefix  | Snippet                                                    |
| ------- | ---------------------------------------------------------- |
| `clg`   | `console.log( $1 )`                                        |
| `clgn`  | `console.log("$1", $1)`                                    |
| `cls`   | `className={styles.$1}`                                    |
| `sty`   | `style={{ $1 }}`                                           |
| `esp`   | `e.stopPropagation(); e.preventDefault();`                 |
| `glb`   | `& :global($1){$2};`                                       |
| `v--`   | `var(--$1);`                                               |
| `elli`  | `css text-overflow: ellipsis`                              |
| `ush`   | `const [$1,set$1] = useState($2);`                         |
| `ueh`   | `useEffect` template                                       |
| `uch`   | `useCallback` template                                     |
| `umh`   | `useMemo` template                                         |
| `urh`   | `const $1 = useRef(${2:null})`                             |
| `uss`   | `const $1 = useSelector((state: iRootState) => state.$2);` |
| `usd`   | `const dispatch = useDispatch<Dispatch>();`                |
| `usc`   | `const { $2 } = $1.useContainer();`                        |
| `usm`   | `const is$1 = useMedia('(max-width: $1px)');`              |
| `uswr`  | `useSWR` template                                          |
| `imr`   | `import * as React from 'react';`                          |
| `imrh`  | `import React, { xx } from 'react';`                       |
| `imd`   | `import { useSelector, useDispatch } from 'react-redux';`  |
| `ima`   | `import { xx } from 'antd';`                               |
| `imc`   | `import classnames from 'classnames';`                     |
| `ims`   | `import { ReactComponent as $1Svg } from '$1.svg';`        |
| `imswr` | `import useSWR from 'swr';`                                |
| `iml`   | `import loadable from '@loadable/component';`              |
| `lmm`   | `const $1 = loadable(() => import('$1'));$0`               |
| `imc`   | `import classnames from 'classnames';`                     |
| `imt`   | a template of normal react component                       |
| `imdt`  | a template of react component with Redux                   |
| `imut`  | a template of unstated-next                                |

**imt**

```js
import React from 'react';
import styles from './index.module.less';
interface Props {

}
const FC = (props: Props) => {
  return (

  );
};
export default React.memo(FC);
```

**imdt**

```js
import React from 'react';
import styles from './index.module.less';
import { useDispatch, useSelector } from 'react-redux';
import { Dispatch, iRootState } from '../store';
interface Props {

}
const FC = (props: Props) => {
  const dispatch = useDispatch<Dispatch>();
  const  = useSelector((state: iRootState) => state.);
  return (

  );
};
export default React.memo(FC);
```

**imut**

```js
import { useState } from "react";
import { createContainer } from "unstated-next";

function useCounter() {
  const [state, setState] = useState < any > null;
  return { state, setState };
}

export default createContainer(useCounter);
```

![icon](./example.gif)

## Add to your project

There are 2 ways you can add React Hooks Snippets to your project:

#### By command

Launch VS Code Quick Open (`Ctrl+P`), paste `ext install Orainsink.nr-react-hooks-snippets`, and press enter.

#### By the Extension Marketplace

Launch VS Code Extension Marketplace (Ctrl+Shift+X), search for `NR React Hooks Snippets`, and look for my logo!

## Contributing

Submit a pull request with your proposed fixes, changes, and/or improvements and I'll take a look!

## License

Usage is provided under the [MIT License](https://opensource.org/licenses/MIT). See LICENSE.txt for the full details.
