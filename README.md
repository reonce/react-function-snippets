# React Function Snippets

A minimalist VSCode template plug-in, designed to be concise syntax.<br/>
一个极简的VSCode模板插件，设计原则是极简语法 <br/>

After the installation, run the following command in the JS file, CSS file, or extended file (such as TSX and less).<br/>
安装后，在js、css文件及拓展文件(tsx、less等)中输入以下命令使用
## Supported Snippets

| Prefix  | Snippet                                                    |
| ------- | ---------------------------------------------------------- |
| `cl`    | `console.log($0)`                                          |
| `clo`   | `console.log({$0})`                                        |
| `cln`   | `className={styles.$1}$0 `                                 |
| `sty`   | `style={{ $1 }}`                                           |
| `esp`   | `e.stopPropagation(); e.preventDefault();`                 |
| `cus`   | `const [$1,set$1] = useState($2);`                         |
| `ue`    | `useEffect` template                                      |
| `uc`    | `useCallback` template                                     |
| `um`    | `useMemo` template                                         |
| `uf`    | `const $1 = useRef(${2:null})`                             |
| `im`   | `import $1 from '$2$1'` import xx from xx                   |
| `imo`   | `import { $1 } from '$2'` import { a } from b              |
| `imr`    | `import * as React from 'react';`                         |
| `iro`   | `import React, { xx } from 'react';`                       |
| `ird`   | `import { useSelector, useDispatch } from 'react-redux';`  |
| `ima`   | `import { $1 } from 'antd';$0` import { } from antd        |
| `ims`   | `import styles from './index.module.less';`                |
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
import { memo } from 'react';
import styles from './index.module.less';
    
const FC = () => {
  return (
    <div className={styles.wrap}>
       
    </div>
  );
};
export default memo(FC);
```
