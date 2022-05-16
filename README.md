# React Function Snippets

![icon](./icon.png)

[react-function-snippets](https://github.com/reonce/react-function-snippets)

## Supported Snippets

| Prefix  | Snippet                                                    |
| ------- | ---------------------------------------------------------- |
| `cl`    | `console.log($0)`                                          |
| `clo`   | `console.log({$0})`                                        |
| `cln`   | `className={styles.$1}$0 `                                 |
| `sty`   | `style={{ $1 }}`                                           |
| `esp`   | `e.stopPropagation(); e.preventDefault();`                 |
| `cus`   | `const [$1,set$1] = useState($2);`                         |
| `ue`    | `useEffect` template                                       |
| `uc`    | `useCallback` template                                     |
| `um`    | `useMemo` template                                         |
| `uf`    | `const $1 = useRef(${2:null})`                             |
| `ifd`   | `import $1 from '$2$1'` import xx from xx                  |
| `ifo`   | `import { $1 } from '$2'` import { a } from b              |
| `ir`    | `import * as React from 'react';`                          |
| `irc`   | `import React, { xx } from 'react';`                       |
| `ird`   | `import { useSelector, useDispatch } from 'react-redux';`  |
| `iac`   | `import { $1 } from 'antd';$0` import { } from antd        |
| `ics`   | `import classNames from 'classnames';`                     |
| `isg`   | `import { ReactComponent as $1Svg } from '$1.svg';`        |
| `els`   | `css text-overflow: ellipsis`                              |
| `sgl`   | `& :global($1){$2};` cover styles with global              |
| `esp`   | `e.stopPropagation(); && e.preventDefault();`              |
| `rct`   | a react component template as follows                      |
| `rctm`  | a react memo component template as follows                 |

**rct**

```js
import React from 'react';
import styles from './index.module.less';

const FC = () => {
  return (
    <div className={styles.wrap}>
       
    </div>
  );
};
export default FC;
```

**rctm**

```js
import React from 'react';
import styles from './index.module.less';
    
const FC = () => {
  return (
    <div className={styles.wrap}>
       
    </div>
  );
};
export default React.memo(FC);
```
