---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云 PC 本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 188d9db2dbef3b3e731e0c95a48f6637e3e00101
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378286"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>cloudPcOnPremisesConnectionHealthCheck 资源类型

命名空间：microsoft.graph

云 PC 本地连接运行状况检查的结果。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[RunHealthChecks of cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|运行 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的运行状况检查。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|此运行状况检查项的显示名称。|
|status|cloudPcOnPremisesConnectionStatus|运行状况检查项的状态。 只读。 可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。|
|startDateTime|DateTimeOffset|运行状况检查项的开始时间。 只读。|
|endDateTime|DateTimeOffset|运行状况检查项的结束时间。 只读。|
|errorType|cloudPcOnPremisesConnectionHealthCheckErrorType|在此运行状况检查过程中发生的错误的类型。 可取值为：`DnsCheckFqdnNotFound`、`DnsCheckUnknownError`、`AdJoinCheckFqdnNotFound`、`AdJoinCheckIncorrectCredentials`、`AdJoinCheckOrganizationalUnitNotFound`、`AdJoinCheckOrganizationalUnitIncorrectFormat`、`AdJoinCheckUnknownError`、`EndpointConnectivityCheckUrlNotWhitelisted`、`EndpointConnectivityCheckUnknownError`、`AadConnectivityCheckUnknownError`。|
|recommendedAction|字符串|建议用于修复相应错误的操作。|
|additionalDetails|字符串|有关运行状况检查或建议操作的其他详细信息。|

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
