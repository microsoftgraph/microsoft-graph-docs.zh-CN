---
title: authorizationPolicy 资源类型
description: 表示可以控制用户授权设置Azure Active Directory。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cb35f7745a22a4a2eda43c48b3fc870ba1a88cce
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231586"
---
# <a name="authorizationpolicy-resource-type"></a>authorizationPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可以控制授权Azure Active Directory的策略。 它是从基本策略类型继承的单一对象，并且始终存在于租户中。 

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | 读取 authorizationPolicy 对象。 |
| [更新 authorizationPolicy](../api/authorizationpolicy-update.md) | 无 | 更新 authorizationPolicy 对象。 |

## <a name="properties"></a>属性  
| 属性 | 类型 | 说明 | 
|-|-|-|
|allowedToSignUpEmailBasedSubscriptions|Boolean| 指示用户是否可以注册基于电子邮件的订阅。 | 
|allowedToUseSSPR|Boolean| 指示租户Self-Serve是否可以使用密码重置功能。 | 
|allowEmailVerifiedUsersToJoinOrganization|Boolean| 指示用户是否可以通过电子邮件验证加入租户。 | 
|allowInvitesFrom|allowInvitesFrom|指示谁可以邀请外部用户加入组织。 可取值为：`none`、`adminsAndGuestInviters`、`adminsGuestInvitersAndAllMembers`、`everyone`。  `everyone` 是除美国政府以外的所有云环境的默认设置。 请参阅下表中的 [，了解](#allowinvitesfrom-values)。|
|blockMsolPowerShell|Boolean| 若要禁止使用 MSOL PowerShell，将此属性设置为 `true` 。 这还将禁止基于用户对 MSOL PowerShell 使用的旧服务终结点的访问。 这不会影响 Azure AD 连接 或 Microsoft Graph。 | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| 指定默认用户角色的某些可自定义权限。 | 
|说明|String| 此策略的说明。|  
|displayName|String| 此策略的显示名称。 |  
|enabledPreviewFeatures|String collection| 租户上启用专用预览的功能列表。 | 
|guestUserRoleId|Guid| 表示应授予来宾用户的角色的角色 templateId。 请参阅 [列出 unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) 以查找可用角色模板的列表。 当前支持以下角色：用户角色 () 、来宾用户 `a0b1b346-4d3e-4e8b-98f8-753987be4970` `10dae51f-b6af-4016-8d66-8c2a99b929b3` () 和受限来宾 `2af84b1e-32c8-42b7-82bc-daa82404023b` () 。 | 
|id|String| 授权策略的 ID。 必需。 只读。| 
|permissionGrantPolicyIdsAssignedToDefaultUserRole|String collection|指示是否允许用户同意应用，如果是，哪个应用许可策略 (permissionGrantPolicy) 管理用户授予同意的权限。 值的格式应为 ，其中 是内置或自定义应用同意策略 `managePermissionGrantsForSelf.{id}` `{id}` 的[ID。](/azure/active-directory/manage-apps/manage-app-consent-policies)  空列表表示已禁用用户对应用的同意。 |

### <a name="allowinvitesfrom-values"></a>allowInvitesFrom 值

|成员|说明|
|:---|:---|
|无|阻止包括管理员在内的所有人邀请外部用户。 美国政府的默认设置。|
|adminsAndGuestInviters|允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。|
|adminsGuestInvitersAndAllMembers|允许上述管理员角色和所有其他用户角色成员邀请外部用户。|
|everyone|允许组织中的每个人（包括来宾用户）邀请外部用户。 除美国政府以外的所有云环境的默认设置。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "keyProperty": "id"
}-->

```json
{
   "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String",
  "permissionGrantPolicyIdsAssignedToDefaultUserRole": "[String]"
}
```
