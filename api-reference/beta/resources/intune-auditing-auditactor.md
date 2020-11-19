---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01dd1df7e273e9ef2bbd6fabb9a0ea0203e5347f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295535"
---
# <a name="auditactor-resource-type"></a>auditActor 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含审核主角的属性的类。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|type|字符串|主角类型。|
|userPermissions|String collection|执行审核时的用户权限列表。|
|applicationId|String|AAD 应用程序 ID。|
|applicationDisplayName|String|应用程序的名称。|
|userPrincipalName|字符串|用户主体名称 (UPN)。|
|servicePrincipalName|String|服务主体名称 (SPN)。|
|ipAddress|String|IPAddress。|
|userId|字符串|用户 ID。|
|userRoleScopeTags|[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) 集合|执行审核时的用户范围标记列表。|
|remoteTenantId|字符串|远程租户 Id|
|remoteUserId|字符串|远程用户 Id|

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




