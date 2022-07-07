---
title: remoteAssistanceReporting 资源类型
description: RemoteAssistanceReporting 资源表示给定远程协助报告有效负载的元数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 65ca73ed17e70e9d4a86439a1daea490b84b30bc
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668648"
---
# <a name="remoteassistancereporting-resource-type"></a>remoteAssistanceReporting 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

RemoteAssistanceReporting 资源表示给定远程协助报告有效负载的元数据

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|会话和每个会话的报告有效负载的唯一标识符|
|startDateTime|DateTimeOffset|会话的开始时间|
|endDateTime|DateTimeOffset|会话的结束时间|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|所举行的远程协助会话的类型。 可取值为：`viewOnly`、`fullControl`、`elevation`。 可取值为：`viewOnly`、`fullControl`、`elevation`。|
|helperEmail|String|帮助程序用于建立会话的登录电子邮件|
|helperTenantId|String|帮助程序的租户 ID|
|helperFirstName|String|帮助程序的名字|
|helperLastName|字符串|帮助程序的姓氏|
|helperOs|String|帮助程序的操作系统|
|helperDeviceAadId|String|帮助程序的设备 AAD ID|
|helperDeviceName|字符串|帮助程序的设备名称|
|helperEnrollmentState|[enrollmentState](../resources/intune-remoteassistance-enrollmentstate.md)|Intune帮助程序设备的注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|sharerEmail|String|共享程序用于建立会话的登录电子邮件|
|sharerTenantId|String|共享程序的租户 ID|
|sharerFirstName|String|Sharer 的名字|
|sharerLastName|String|Sharer 的姓氏|
|sharerDeviceAadId|String|Sharer 的设备 AAD ID|
|sharerDeviceName|String|Sharer 的设备名称|
|sharerOs|String|Sharer 的操作系统|
|sharerEnrollmentState|[enrollmentState](../resources/intune-remoteassistance-enrollmentstate.md)|Intune sharer 设备的注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteAssistanceReporting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistanceReporting",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "remoteAssistanceSessionType": "String",
  "helperEmail": "String",
  "helperTenantId": "String",
  "helperFirstName": "String",
  "helperLastName": "String",
  "helperOs": "String",
  "helperDeviceAadId": "String",
  "helperDeviceName": "String",
  "helperEnrollmentState": "String",
  "sharerEmail": "String",
  "sharerTenantId": "String",
  "sharerFirstName": "String",
  "sharerLastName": "String",
  "sharerDeviceAadId": "String",
  "sharerDeviceName": "String",
  "sharerOs": "String",
  "sharerEnrollmentState": "String"
}
```




