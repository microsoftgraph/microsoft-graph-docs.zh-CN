---
title: cloudPcAuditActor 资源类型
description: 由 Azure AD 用户和与审核事件关联的应用程序表示的审核参与者。
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5cd851d22d20eb5d0e466cae7b799ad70bd390a2
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766311"
---
# <a name="cloudpcauditactor-resource-type"></a>cloudPcAuditActor 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

由 Azure AD 用户和与审核事件关联的应用程序表示的审核参与者。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|类型|[cloudPcAuditActorType](#cloudpcauditactortype-values)|主角类型。 可能的值包括 `ItPro` 、 `Application` 和 `Partner` `Unknown` 。|
|userPermissions|String collection|执行审核事件时的用户权限和应用程序权限列表。|
|applicationId|String|Azure AD 应用程序 ID。|
|applicationDisplayName|String|应用程序的名称。|
|userPrincipalName|String|用户主体名称 (UPN)。|
|servicePrincipalName|String|服务主体名称 (SPN)。|
|ipAddress|String|IP 地址。|
|userId|String|Azure AD 用户 ID。|
|userRoleScopeTags|[cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md) 集合|角色范围标记的列表。|
|remoteTenantId|String|委派的合作伙伴租户 ID。|
|remoteUserId|String|委派的合作伙伴用户 ID。|

### <a name="cloudpcauditactortype-values"></a>cloudPcAuditActorType 值

|成员|说明|
|:---|:---|
|itPro|该操作由 IT 专业人员执行。|
|应用程序|操作由应用程序执行。|
|partner|操作由合作伙伴执行。|
|unknown|未知主角。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditActor"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditActor",
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
      "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```
