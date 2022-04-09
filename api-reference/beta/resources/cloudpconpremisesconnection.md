---
title: cloudPcOnPremisesConnection 资源类型
description: 表示可用于为云电脑建立 Azure 网络连接的 Azure 资源信息的定义集合。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3c6e3630ffe7ed1853c758ce14a32178ea835549
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733225"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>cloudPcOnPremisesConnection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可用于为云电脑建立 Azure 网络连接的 Azure 资源信息的定义集合。

[!INCLUDE [on-premise-rename-note](../../includes/on-premise-rename-note.md)]

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|列出 [cloudPcOnPremisesConnection 对象的](../resources/cloudpconpremisesconnection.md) 属性和关系。|
|[获取 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|读取 [cloudPcOnPremisesConnection 对象的](../resources/cloudpconpremisesconnection.md) 属性和关系。|
|[创建 cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。|
|[更新 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|更新 [cloudPcOnPremisesConnection 对象的](../resources/cloudpconpremisesconnection.md) 属性。|
|[删除 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|无|删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。 无法删除正在使用的连接。|
|[cloudPcOnPremisesConnection 的 RunHealthChecks](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|在 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 上运行运行运行状况检查。|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|无|为成功的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 更新 Active Directory 域密码。 当 **cloudPcOnPremisesConnection** 对象的类型为 `hybridAzureADJoin` 时，支持此 API。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Azure 网络连接的唯一标识符。 只读。|
|managedBy|[cloudPcManagementService](#cloudpcmanagementservice-values)|指定管理 Azure 网络连接的服务。 可能的值为： `windows365`和 `unknownFutureValue``devBox` . 只读。
|类型|[cloudPcOnPremisesConnectionType](#cloudpconpremisesconnectiontype-values)|指定如何将预配的云电脑加入Azure Active Directory。 默认值为 `hybridAzureADJoin`。 可取值为：`azureADJoin`、`hybridAzureADJoin`、`unknownFutureValue`。|
|displayName|String|Azure 网络连接的显示名称。|
|subscriptionId|String|与租户关联的目标 Azure 订阅的 ID。|
|subscriptionName|String|目标 Azure 订阅的名称。 只读。|
|adDomainName|String|要加入的 Active Directory 域的完全限定域名 (FQDN) 。 可选。|
|adDomainUsername|String|Active Directory 帐户的用户名 (用户或服务帐户) ，该帐户有权在 Active Directory 中创建计算机对象。 必需格式：admin@contoso.com。 可选。|
|adDomainPassword|字符串|与 **adDomainUsername** 关联的密码。|
|organizationalUnit|字符串|在其中创建计算机帐户的组织单位 (OU) 。 如果留空，则会使用配置为默认 (Active Directory 域中已知计算机对象容器) 的 OU (OU) 。 可选。|
|resourceGroupId|String|目标资源组的 ID。 必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。|
|virtualNetworkId|字符串|目标虚拟网络的 ID。 必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。|
|subnetId|String|目标子网的 ID。 必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|在 Azure 网络连接上执行的最新运行状况检查的状态。 例如，如果状态为"传递"，则 Azure 网络连接已通过服务运行的所有检查。 可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。 只读。|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|连接运行状况检查的详细信息和相应的结果。 仅返回 。 `$select`有关演示如何获取 **inUse** 属性的示例，请参阅 [示例 2：获取 Azure 网络连接的选定属性，包括 healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md)。 只读。|
|inUse|Boolean|当 `true`Azure 网络连接正在使用时。 当 `false`连接未使用时。 无法删除正在使用的连接。 仅在 `$select` 上返回。 有关演示如何获取 **inUse** 属性的示例，请参阅 [示例 2：获取 Azure 网络连接的选定属性，包括 healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md)。 只读。|

### <a name="cloudpcmanagementservice-values"></a>cloudPcManagementService 值

|成员| 值 |说明|
|:---|:---|:---|
|windows365|1| Azure 网络连接是通过 Windows365 成功创建的。|
|devBox|2| Azure 网络连接是通过 Project Fidalgo 成功创建的。|
|unknownFutureValue|4| 可变枚举 sentinel 值。 请勿使用。|

### <a name="cloudpconpremisesconnectiontype-values"></a>cloudPcOnPremisesConnectionType 值

|成员|说明|
|:---|:---|
|hybridAzureADJoin|已加入本地 Active Directory和Azure AD。 只能分配混合用户并登录到云电脑。|
|azureADJoin|仅加入Azure AD。 可以分配仅限云的和混合用户并登录到云电脑。|
|unknownFutureValue|可变枚举 sentinel 值。 请勿使用。|

### <a name="cloudpconpremisesconnectionstatus-values"></a>cloudPcOnPremisesConnectionStatus 值

|成员|说明|
|:---|:---|
|等待|创建并等待运行状况检查。|
|运行|运行运行状况检查。|
|通过|运行状况检查已通过。|
|失败|运行状况检查失败。|
|警告|使用警告传递的运行状况检查。|
|unknownFutureValue|未知的未来状态 (保留，目前) 未使用。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false,
  "optionalProperties": ["healthCheckStatusDetails"]
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "String (identifier)",
  "managedBy": "String",
  "type": "String",
  "displayName": "String",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "adDomainName": "String",
  "adDomainUsername": "String",
  "adDomainPassword": "String",
  "organizationalUnit": "String",
  "resourceGroupId": "String",
  "virtualNetworkId": "String",
  "subnetId": "String",
  "healthCheckStatus": "string",
  "healthCheckStatusDetails": {
    "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "healthChecks": [
      {
        "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
        "displayName": "String",
        "status": "String",
        "startDateTime": "String (timestamp)",
        "endDateTime": "String (timestamp)",
        "errorType": "String",
        "recommendedAction": "String",
        "additionalDetails": "String"
      }
    ]
  },
  "inUse": "Boolean"
}
```
