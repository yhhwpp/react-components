#Toast 轻提示

一种轻量级反馈/提示，可以用来显示不会打断用户操作的内容，适合用于页面转场、数据交互的等场景中。


### 规则
- 一次只显示一个 toast。
- 有 Icon 的 Toast，字数为 4-6 个；没有 Icon 的 Toast，字数不宜超过 14 个。


## API

- `Toast.success(content, duration)`
- `Toast.fail(content, duration)`
- `Toast.info(content, duration)`
- `Toast.loading(content, duration)`
- `Toast.offline(content, duration)`


| 参数       | 说明           | 类型                       | 默认值       |
|------------|----------------|----------------------------|--------------|
| content    | 提示内容       | React.Element or String    | 无           |
| duration   | 自动关闭的延时，单位秒 | number                 | 3          |

> **注：**  duration = 0 时，toast 不会消失；隐藏 toast 需要手动调用 hide

全局配置和全局销毁方法：

- `Toast.hide()`
