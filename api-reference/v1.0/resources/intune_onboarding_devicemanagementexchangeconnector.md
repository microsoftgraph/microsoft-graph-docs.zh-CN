# <a name="devicemanagementexchangeconnector-resource-type"></a>deviceManagementExchangeConnector 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示与 Exchange 环境的连接的实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementExchangeConnectors](../api/intune_onboarding_devicemanagementexchangeconnector_list.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 集合|列出 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象的属性和关系。|
|[获取 deviceManagementExchangeConnector](../api/intune_onboarding_devicemanagementexchangeconnector_get.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|读取 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象的属性和关系。|
|[创建 deviceManagementExchangeConnector](../api/intune_onboarding_devicemanagementexchangeconnector_create.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|创建新的 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象。|
|[删除 deviceManagementExchangeConnector](../api/intune_onboarding_devicemanagementexchangeconnector_delete.md)|无|删除 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)。|
|[更新 deviceManagementExchangeConnector](../api/intune_onboarding_devicemanagementexchangeconnector_update.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|更新 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象的属性。|
|[同步操作](../api/intune_onboarding_devicemanagementexchangeconnector_sync.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|lastSyncDateTime|DateTimeOffset|Exchange Connector 的上一次同步时间|
|状态|[deviceManagementExchangeConnectorStatus](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|Exchange 连接器状态。 可取值为：`none`、`connectionPending`、`connected`、`disconnected`。|
|primarySmtpAddress|String|用于配置服务到服务 Exchange Connector 的电子邮件地址。|
|serverName|String|Exchange server 的名称。|
|connectorServerName|String|托管 Exchange Connector 的服务器的名称。|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|配置的 Exchange Connector 的类型。 可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。|
|version|String|ExchangeConnectorAgent 版本|
|exchangeAlias|String|分配到 Exchange 服务器的别名|
|exchangeOrganization|String|Exchange 服务器的 Exchange 组织|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```



