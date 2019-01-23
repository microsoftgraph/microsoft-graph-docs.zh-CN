---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb9ededd9d1a2bb93f970f9f0da0c41a248e840
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425797"
---
# <a name="auditactor-resource-type"></a>auditActor 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含审核主角的属性的类。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|type|String|主角类型。|
|userPermissions|String collection|执行审核时的用户权限列表。|
|applicationId|String|AAD 应用程序 ID。|
|applicationDisplayName|String|应用程序的名称。|
|userPrincipalName|String|用户主体名称 (UPN)。|
|servicePrincipalName|String|服务主体名称 (SPN)。|
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




