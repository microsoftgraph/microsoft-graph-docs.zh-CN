# <a name="mimecontent-resource-type"></a>mimeContent 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含通用 MIME 内容的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|类型|String|指示内容 MIME 类型。|
|value|Binary|包含实际内容的字节数组。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



