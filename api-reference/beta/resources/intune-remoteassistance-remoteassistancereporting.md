---
title: remoteAssistanceReporting 资源类型
description: RemoteAssistanceReporting 资源表示给定远程协助报告有效负载的元数据
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7793b8ef8bffa33e5d2e77de9fd102b9d0c59288
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039460"
---
# <a name="remoteassistancereporting-resource-type"></a>remoteAssistanceReporting 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

RemoteAssistanceReporting 资源表示给定远程协助报告有效负载的元数据

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|会话和每个会话的报告有效负载的唯一标识符|
|startDateTime|DateTimeOffset|会话的开始时间|
|endDateTime|DateTimeOffset|会话的结束时间|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|已召开的远程协助会话的类型。 可取值为：`viewOnly`、`fullControl`、`elevation`。 可取值为：`viewOnly`、`fullControl`、`elevation`。|
|helperEmail|String|帮助程序用来建立会话的登录电子邮件|
|helperTenantId|String|帮助程序租户 ID|
|helperFirstName|String|帮助程序的名字|
|helperLastName|String|帮助程序姓氏|
|helperDeviceAadId|String|帮助程序的设备 AAD ID|
|helperDeviceName|String|帮助程序的设备名称|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|帮助程序设备的 Intune 注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|sharerEmail|String|共享者用于建立会话的登录电子邮件|
|sharerTenantId|String|共享者租户 ID|
|sharerFirstName|String|Sharer 的名字|
|sharerLastName|String|Sharer 的姓氏|
|sharerDeviceAadId|String|Sharer 的设备 AAD ID|
|sharerDeviceName|String|Sharer 的设备名称|
|sharerEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|共享者设备的 Intune 注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|

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
  "helperDeviceAadId": "String",
  "helperDeviceName": "String",
  "helperEnrollmentState": "String",
  "sharerEmail": "String",
  "sharerTenantId": "String",
  "sharerFirstName": "String",
  "sharerLastName": "String",
  "sharerDeviceAadId": "String",
  "sharerDeviceName": "String",
  "sharerEnrollmentState": "String"
}
```



