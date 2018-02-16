# <a name="reportroot-resource-type"></a>reportRoot 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示一个历史记录报告实例的资源。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 reportRoot](../api/intune_deviceconfig_reportroot_get.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|读取 [reportRoot](../resources/intune_deviceconfig_reportroot.md) 对象的属性和关系。|
|[更新 reportRoot](../api/intune_deviceconfig_reportroot_update.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|更新 [reportRoot](../resources/intune_deviceconfig_reportroot.md) 对象的属性。|
|[deviceConfigurationUserActivity 函数](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[报告](../resources/intune_deviceconfig_report.md)|设备配置用户活动报告的元数据|
|[deviceConfigurationDeviceActivity 函数](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[报告](../resources/intune_deviceconfig_report.md)|设备配置设备活动报告的元数据|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



