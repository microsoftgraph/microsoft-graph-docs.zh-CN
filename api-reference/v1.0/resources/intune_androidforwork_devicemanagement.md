# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

充当设备管理下的 Android for Work 设置功能容器的单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[Get deviceManagement](../api/intune_androidforwork_devicemanagement_get.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|读取 [deviceManagement](../resources/intune_androidforwork_devicemanagement.md) 对象的属性和关系。|
|[Update deviceManagement](../api/intune_androidforwork_devicemanagement_update.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|更新 [deviceManagement](../resources/intune_androidforwork_devicemanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Android for Work 设置单例实体。|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) 集合|Android for Work 应用配置架构实体。|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 集合|Android for Work 注册配置文件实体。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



