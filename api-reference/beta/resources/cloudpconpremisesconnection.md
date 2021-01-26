---
title: cloudPcOnPremisesConnection 资源类型
description: 表示 Azure 资源信息的定义集合，可用于为云电脑建立本地网络连接。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 88143f58c070f7a359fab7bb0674fa6a39477d91
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982731"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>cloudPcOnPremisesConnection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure 资源信息的定义集合，可用于为云电脑建立本地网络连接。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|列出 [cloudPcOnPremisesConnection 对象的属性和](../resources/cloudpconpremisesconnection.md) 关系。|
|[获取 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。|
|[创建 cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。|
|[更新 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|更新 [cloudPcOnPremisesConnection 对象](../resources/cloudpconpremisesconnection.md) 的属性。|
|[删除 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|无|删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。 不能删除使用的连接。|
|[CloudPcOnPremisesConnection 的 RunHealthChecks](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|对 [cloudPcOnPremisesConnection 运行运行状况检查](../resources/cloudpconpremisesconnection.md)。|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|无|更新成功 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的 AD 域密码。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|本地连接的唯一标识符。 只读。|
|displayName|String|本地显示名称的基础结构。|
|subscriptionId|String|与租户关联的目标 Azure 订阅的 ID。|
|subscriptionName|String|目标 Azure 订阅的名称。 只读。|
|adDomainName|String|要加入的 Active Directory (的 FQDN) 完全限定域名。|
|adDomainUsername|String|Active Directory 帐户的用户名 (拥有在 Active Directory) 创建计算机对象的权限的用户或服务帐户。 所需格式：admin@contoso.com。|
|adDomainPassword|String|与 adDomainUsername 关联的密码。|
|organizationalUnit|String|创建计算机 (OU) 组织单位。 如果留空，则使用配置为默认 ou (Active Directory 域) OU (中的已知计算机对象容器) OU。 可选。|
|resourceGroupId|String|目标资源组的 ID。 必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。|
|virtualNetworkId|String|目标虚拟网络的 ID。 必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。|
|subnetId|String|目标子网的 ID。 必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。|
|healthCheckStatus|cloudPcOnPremisesConnectionStatus|在本地连接上完成的最新运行状况检查的状态。 例如，如果状态为"passed"，则本地连接已通过服务运行的所有检查。 只读。 可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|连接运行状况检查的详细信息和相应的结果。 仅在 `$select` 上返回。 请参阅 [获取](../api/cloudpconpremisesconnection-get.md) healthCheckStatusDetails 属性的示例。只读。|
|inUse|Boolean|如果为 true，则使用本地连接。 如果为 false，则不使用连接。 不能删除使用的连接。 只读。|

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
