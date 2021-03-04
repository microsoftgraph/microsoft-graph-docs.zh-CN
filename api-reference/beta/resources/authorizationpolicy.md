---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e9ad1a67a2aae2c1af4ffa45dcd85228a4c95f25
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433171"
---
# <a name="authorizationpolicy-resource-type"></a>authorizationPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可控制 Azure Active Directory 授权设置的策略。 它是从基本策略类型继承的单一对象，并且始终存在于租户中。 

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | 读取 authorizationPolicy 对象。 |
| [更新 authorizationPolicy](../api/authorizationpolicy-update.md) | 无 | 更新 authorizationPolicy 对象。 |

## <a name="properties"></a>属性  
| 属性 | 类型 | 说明 | 
|-|-|-|
|id|String| 授权策略的 ID。 必需。 只读。| 
|displayName|String| 此策略的显示名称。 |  
|说明|String| 此策略的说明。|  
|guestUserRoleId|Guid| 表示应授予来宾用户的角色的角色 templateId。 请参阅 [List unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) 查找可用角色模板的列表。 当前支持以下角色：用户 (a0b1b346-4d3e-4e8b-98f8-753987be4970) ， 来宾用户 (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。 | 
|enabledPreviewFeatures|字符串集合| 为租户上的专用预览启用的功能列表。 | 
|blockMsolPowerShell|布尔| 若要禁止使用 MSOL PowerShell，请设置此属性为 true。 设置为 true 还将禁用对 MSOL PowerShell 使用的旧服务终结点的基于用户的访问。 这不会影响 Azure AD Connect 或 Microsoft Graph。 | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| 指定默认用户角色的某些可自定义权限。 | 
|allowedToUseSSPR|布尔| 指示租户Self-Serve密码重置功能是否可以使用。 | 
|allowedToSignUpEmailBasedSubscriptions|布尔| 指示用户是否可以注册基于电子邮件的订阅。 | 
|allowEmailVerifiedUsersToJoinOrganization|布尔| 指示用户是否可以通过电子邮件验证加入租户。 | 
|allowInvitesFrom|String|指示可以邀请外部用户加入组织的用户。 可能的值是：<ul><li>`none` - 阻止包括管理员在内的所有人邀请外部用户。 美国政府的默认设置。</li><li>`adminsAndGuestInviters` - 允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</li><li>`adminsGuestInvitersAndAllMembers` - 允许上述管理员角色和所有其他用户角色成员邀请外部用户。</li><li>`everyone` - 允许组织中的每个人（包括来宾用户）邀请外部用户。 除美国政府以外的所有云环境的默认设置。</li></ul> |
|permissionGrantPolicyIdsAssignedToDefaultUserRole|字符串集合|指示是否允许用户同意应用，如果是，则哪个应用同意策略 (permissionGrantPolicy) 管理用户授予同意的权限。 值的格式应为，其中是内置或自定义应用同意策略 `managePermissionGrantsForSelf.{id}` `{id}` 的[ID。](/azure/active-directory/manage-apps/manage-app-consent-policies)  空列表表示已禁用用户对应用的同意。 |

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
