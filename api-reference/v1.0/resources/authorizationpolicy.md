---
title: authorizationPolicy 资源类型
description: 表示可以控制用户授权设置Azure Active Directory。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 52ff42f8ec45885d8effcd73095cb16ba2512bb7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025606"
---
# <a name="authorizationpolicy-resource-type"></a>authorizationPolicy 资源类型

命名空间：microsoft.graph

表示可以控制授权Azure Active Directory的策略。 它是从基本策略类型继承的单一对象，并且始终存在于租户中。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | 读取 authorizationPolicy 对象。 |
| [更新 authorizationPolicy](../api/authorizationpolicy-update.md) | None | 更新 authorizationPolicy 对象。 |

## <a name="properties"></a>属性  
| 属性 | 类型 | 说明 | 
|-|-|-|
|allowedToSignUpEmailBasedSubscriptions|布尔值| 指示用户是否可以注册基于电子邮件的订阅。 | 
|allowedToUseSSPR|布尔值| 指示租户Self-Serve是否可以使用密码重置功能。 | 
|allowEmailVerifiedUsersToJoinOrganization|布尔值| 指示用户是否可以通过电子邮件验证加入租户。 | 
|allowInvitesFrom|allowInvitesFrom|指示谁可以邀请外部用户加入组织。 可取值为：`none`、`adminsAndGuestInviters`、`adminsGuestInvitersAndAllMembers`、`everyone`。  `everyone` 是除美国政府以外的所有云环境的默认设置。 请参阅下表中的 [，了解](#allowinvitesfrom-values)。 |
|blockMsolPowerShell|布尔值| 若要禁止使用 MSOL PowerShell，将此属性设置为 `true` 。 这还将禁止基于用户对 MSOL PowerShell 使用的旧服务终结点的访问。 这不会影响 Azure AD 连接或 Microsoft Graph。 | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| 指定默认用户角色的某些可自定义权限。 | 
|说明|String| 此策略的说明。|
|displayName|String| 此策略的显示名称。 |    
|guestUserRoleId|Guid| 表示应授予来宾用户的角色的角色 templateId。 目前支持以下角色：用户 () 、来宾用户 () 和受限来宾 `a0b1b346-4d3e-4e8b-98f8-753987be4970` `10dae51f-b6af-4016-8d66-8c2a99b929b3` `2af84b1e-32c8-42b7-82bc-daa82404023b` () 。 |
|id|String| 授权策略的 ID。 必需。 只读。| 

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
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String",
  "guestUserRoleId": "Guid"
}
```
