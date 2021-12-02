---
title: cloudPcOnPremisesConnection 资源类型
description: 表示一个定义的 Azure 资源信息集合，可用于为云电脑建立本地网络连接。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: cb1b3dc86aa941720411db9f577e2b12a5817151
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266004"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>cloudPcOnPremisesConnection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个定义的 Azure 资源信息集合，可用于为云电脑建立本地网络连接。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。|
|[获取 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。|
|[创建 cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。|
|[更新 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|更新 [cloudPcOnPremisesConnection 对象](../resources/cloudpconpremisesconnection.md) 的属性。|
|[删除 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|无|删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。 不能删除使用的连接。|
|[cloudPcOnPremisesConnection 的 RunHealthChecks](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|对 [cloudPcOnPremisesConnection 运行运行状况检查](../resources/cloudpconpremisesconnection.md)。|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|无|更新成功 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的 Active Directory 域密码。 当 **onPremisesConnection** 的类型为 时，支持此 `hybridAzureADJoin` API。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|本地连接的唯一标识符。 只读。|
|类型|[cloudPcOnPremisesConnectionType](#cloudpconpremisesconnectiontype-values)|指定预配的云电脑如何加入 Azure Active Directory。 默认值为 `hybridAzureADJoin`。 可取值为：`azureADJoin`、`hybridAzureADJoin`、`unknownFutureValue`。|
|displayName|String|内部显示名称连接的连接。|
|subscriptionId|String|与租户关联的目标 Azure 订阅的 ID。|
|subscriptionName|String|目标 Azure 订阅的名称。 只读。|
|adDomainName|String|要加入的 Active Directory (完全限定) FQDN 的 FQDN。 可选。|
|adDomainUsername|String|Active Directory 帐户的用户名 (拥有在 Active Directory) 创建计算机对象的权限的用户或服务帐户。 所需格式：admin@contoso.com。 可选。|
|adDomainPassword|String|与 **adDomainUsername 关联的密码**。|
|organizationalUnit|String|组织单位 (OU) 创建计算机帐户的组织单位。 如果留空，则使用配置为默认 OU 的 OU (Active Directory 域) OU (已知的计算机) 容器。 可选。|
|resourceGroupId|String|目标资源组的 ID。 所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。|
|virtualNetworkId|String|目标虚拟网络的 ID。 所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。|
|subnetId|String|目标子网的 ID。 所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|在本地连接上完成的最新运行状况检查的状态。 例如，如果状态为"passed"，则本地连接已通过服务运行的所有检查。 可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。 只读。|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|连接运行状况检查的详细信息和相应结果。 仅在 上返回 `$select` 。有关演示如何获取 **inUse** 属性的示例，请参阅示例 2：获取本地连接的选定属性，包括 [healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md)。 只读。|
|inUse|布尔值|如果 `true` 为 ，则使用内部部署连接。 如果 `false` 为 ，则不使用连接。 不能删除使用的连接。 仅在 `$select` 上返回。 有关演示如何获取 **inUse** 属性的示例，请参阅示例 2：获取本地连接的选定属性，包括 [healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md)。 只读。|

### <a name="cloudpconpremisesconnectiontype-values"></a>cloudPcOnPremisesConnectionType 值

|成员|说明|
|:---|:---|
|hybridAzureADJoin|加入本地 Active Directory 并Azure AD。 只能分配混合用户并登录到云电脑。|
|azureADJoin|仅联接Azure AD。 可以分配仅云用户和混合用户并登录到云电脑。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

### <a name="cloudpconpremisesconnectionstatus-values"></a>cloudPcOnPremisesConnectionStatus 值

|成员|说明|
|:---|:---|
|pending|已创建并等待运行状况检查。|
|running|运行状况检查正在运行。|
|passed|运行状况检查通过。|
|failed|运行状况检查失败。|
|警告|运行状况检查通过，并发出警告。|
|unknownFutureValue|未知未来状态 (保留，当前未) 。|

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
