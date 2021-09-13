---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 258624d97663da9b25ee6552e7eb3430191c135b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146798"
---
# <a name="auditactor-resource-type"></a>auditActor 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|userRoleScopeTags|[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) 集合|执行审核时的用户范围标记列表。|
|remoteTenantId|String|远程租户 ID|
|remoteUserId|String|远程用户 ID|

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
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.roleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```



