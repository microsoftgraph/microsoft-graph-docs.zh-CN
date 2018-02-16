# <a name="deviceconfigurationstate-resource-type"></a>deviceConfigurationState 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

给定设备的设备配置状态。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceConfigurationStates](../api/intune_deviceconfig_deviceconfigurationstate_list.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 集合|列出 [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 对象的属性和关系。|
|[获取 deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_get.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|读取 [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 对象的属性和关系。|
|[创建 deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_create.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|创建新的 [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 对象。|
|[删除 deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_delete.md)|无|删除 [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)。|
|[更新 deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_update.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|更新 [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|settingStates|[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) 集合|尚未记录|
|displayName|String|此 policyBase 的策略名称|
|version|Int32|策略版本|
|platformType|String|策略适用的平台类型 可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all`。|
|state|String|策略符合性状态 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。|
|settingCount|Int32|策略保留的设置计数|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "String",
      "settingName": "String",
      "instanceDisplayName": "String",
      "state": "String",
      "errorCode": 1024,
      "errorDescription": "String",
      "userId": "String",
      "userName": "String",
      "userEmail": "String",
      "userPrincipalName": "String",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "String",
          "displayName": "String"
        }
      ],
      "currentValue": "String"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```



