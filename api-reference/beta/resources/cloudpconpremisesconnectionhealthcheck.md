---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云电脑本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e79f73bbe1a493e581a35db5fec396d752ff08d1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844604"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>cloudPcOnPremisesConnectionHealthCheck 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

云电脑本地连接运行状况检查的结果。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[CloudPcOnPremisesConnection 的 RunHealthChecks](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|运行 [cloudPcOnPremisesConnection 的运行状况检查](../resources/cloudpconpremisesconnection.md)。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|此显示名称检查项目的详细信息。|
|status|cloudPcOnPremisesConnectionStatus|运行状况检查项目的状态。 只读。 可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。|
|startDateTime|DateTimeOffset|运行状况检查项目的开始时间。 只读。|
|endDateTime|DateTimeOffset|运行状况检查项目的结束时间。 只读。|
|errorType|cloudPcOnPremisesConnectionHealthCheckErrorType|在此运行状况检查期间发生的错误类型。 可能的值是： `DnsCheckFqdnNotFound` ， `DnsCheckUnknownError` `AdJoinCheckFqdnNotFound` `AdJoinCheckIncorrectCredentials` `AdJoinCheckOrganizationalUnitNotFound` `AdJoinCheckOrganizationalUnitIncorrectFormat` `AdJoinCheckUnknownError` `EndpointConnectivityCheckUrlNotWhitelisted` `EndpointConnectivityCheckUnknownError` `AadConnectivityCheckUnknownError` `ResourceAvailabilityCheckNoSubnetIP` `resourceAvailabilityCheckSubscriptionDisabled` `resourceAvailabilityCheckUnknownError` `permissionCheckNoSubscriptionReaderRole` `permissionCheckNoResourceGroupOwnerRole` `permissionCheckNoVNetContributorRole` `permissionCheckUnknownError` `internalServerUnknownError` 。|
|recommendedAction|String|修复相应错误的建议操作。|
|additionalDetails|String|有关运行状况检查或建议操作的其他详细信息。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
  "displayName": "String",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "errorType": "String",
  "recommendedAction": "String",
  "additionalDetails": "String"
}
```
