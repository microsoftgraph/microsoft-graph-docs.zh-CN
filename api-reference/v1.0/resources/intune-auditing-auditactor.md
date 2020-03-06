---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c10ac0a18f5bfcf68be56edc402c83d9882a8ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532737"
---
# <a name="auditactor-resource-type"></a>auditActor 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含审核主角的属性的类。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|type|字符串|主角类型。|
|userPermissions|String collection|执行审核时的用户权限列表。|
|applicationId|字符串|AAD 应用程序 ID。|
|applicationDisplayName|字符串|应用程序的名称。|
|userPrincipalName|字符串|用户主体名称 (UPN)。|
|servicePrincipalName|字符串|服务主体名称 (SPN)。|
|ipAddress|String|IPAddress。|
|userId|String|用户 ID。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```




