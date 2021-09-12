---
title: deviceManagementIntentUserState 资源类型
description: 表示意图的用户状态的实体
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4eb108729302eab007eed5b04b2ea8fc584ce284
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009054"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>deviceManagementIntentUserState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示意图的用户状态的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementIntentUserStates](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 集合|列出 [deviceManagementIntentUserState 对象的属性和](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 关系。|
|[获取 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|读取 [deviceManagementIntentUserState 对象的属性和](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 关系。|
|[创建 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|创建新的 [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 对象。|
|[删除 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|None|删除 [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)。|
|[更新 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|更新 [deviceManagementIntentUserState 对象](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|The ID|
|userPrincipalName|String|在设备上报告的用户主体名称|
|userName|String|在设备上报告的用户名|
|deviceCount|Int32|出于意图而属于用户的设备的计数|
|lastReportedDateTime|DateTimeOffset|意图报告的上次修改日期时间|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|意图的用户状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```



