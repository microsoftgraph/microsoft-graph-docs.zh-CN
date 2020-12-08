---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71e4d01ba54c9043ff827b3749be63442d06ac
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581198"
---
# <a name="authorizationpolicy-resource-type"></a>authorizationPolicy 资源类型

命名空间：microsoft.graph

表示可控制 Azure Active Directory 授权设置的策略。 它是从基本策略类型继承的单一实例，并且对于租户始终存在。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [获取 authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | 读取 authorizationPolicy 对象。 |
| [更新 authorizationPolicy](../api/authorizationpolicy-update.md) | 无 | 更新 authorizationPolicy 对象。 |

## <a name="properties"></a>属性  
| 属性 | 类型 | 说明 | 
|-|-|-|
|id|String| 授权策略的 ID。 必需。 只读。| 
|displayName|String| 此策略的显示名称。 |  
|说明|String| 此策略的说明。|  
|blockMsolPowerShell|布尔值| 若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。 如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。 这不会影响 Azure AD Connect 或 Microsoft Graph。 | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| 指定默认用户角色的某些可自定义权限。 | 
|allowedToUseSSPR|布尔值| 指示租户上的用户是否可以使用 Self-Serve 密码重置功能。 | 
|allowedToSignUpEmailBasedSubscriptions|布尔值| 指示用户是否可以注册基于电子邮件的订阅。 | 
|allowEmailVerifiedUsersToJoinOrganization|布尔值| 指示用户是否可以通过电子邮件验证加入租户。 | 
|allowInvitesFrom|String|指示谁可以邀请外部用户加入组织。 可能的值是：<ul><li>`none` -防止用户（包括管理员）邀请外部用户。 美国政府版的默认设置。</li><li>`adminsAndGuestInviters` -允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</li><li>`adminsGuestInvitersAndAllMembers` -允许上述管理员角色和所有其他用户角色成员邀请外部用户。</li><li>`everyone` -允许组织中的每个人（包括来宾用户）邀请外部用户。 除美国政府之外的所有云环境的默认设置。</li></ul> |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "",
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
  "allowInvitesFrom": "String"
}
```
