# <a name="managedappdiagnosticstatus-resource-type"></a>managedAppDiagnosticStatus 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示诊断状态。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|validationName|String|验证友好名称|
|状态|String|操作状态|
|mitigationInstruction|String|有关如何降低失败验证的说明|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



