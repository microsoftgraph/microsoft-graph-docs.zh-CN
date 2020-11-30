---
title: cloudPcOnPremisesConnection 资源类型
description: 表示可用于为云电脑建立本地网络连接的 Azure 资源信息的已定义集合。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a8ac0dea68aaac8c1f720948041cfd1eddc048f6
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378289"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>cloudPcOnPremisesConnection 资源类型

命名空间：microsoft.graph

表示可用于为云电脑建立本地网络连接的 Azure 资源信息的已定义集合。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。|
|[获取 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。|
|[创建 cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。|
|[更新 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|更新 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性。|
|[删除 cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|无|删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。 无法删除正在使用的连接。|
|[RunHealthChecks of cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|对 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)运行运行状况检查。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|本地连接的唯一标识符。 只读。|
|displayName|字符串|本地连接的显示名称。|
|subscriptionId|字符串|与你的租户关联的目标 Azure 订阅的 ID。|
|subscriptionName|字符串|目标 Azure 订阅的名称。 只读。|
|adDomainName|字符串|要加入的 Active Directory 域 (FQDN) 的完全限定的域名称。|
|adDomainUsername|字符串|Active Directory 帐户的用户名 (用户或服务帐户) 具有在 Active Directory 中创建计算机对象的权限。 必需的格式： contoso@microsoft.com。|
|adDomainPassword|字符串|与 adDomainUsername 相关联的密码。|
|organizationalUnit|字符串|在其中创建计算机帐户的组织单位 (OU) 。 如果为 null，则在使用 Active Directory 域 (OU) 中) 的已知计算机对象容器中配置为默认 (的 OU。 可选。|
|resourceGroupId|字符串|目标资源组的 ID。 必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。|
|virtualNetworkId|字符串|目标虚拟网络的 ID。 必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。|
|subnetId|字符串|目标子网的 ID。 必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。|
|healthCheckStatus|cloudPcOnPremisesConnectionStatus|对本地连接执行的最新运行状况检查的状态。 例如，如果状态为 "已传递"，则本地连接已通过该服务运行的所有检查。 只读。 可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|连接的运行状况检查和相应结果的详细信息。 仅在 `$select` 上返回。 请参阅获取 healthCheckStatusDetails 属性的 [示例](../api/cloudpconpremisesconnection-get.md) 。只读。|
|inUse|Boolean|如果为 true，则使用内部部署连接。 如果为 false，则表示未使用该连接。 无法删除正在使用的连接。 只读。|

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
