---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e93fe5e751cfde883a867305ad7a984a840a91c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034089"
---
# <a name="authorizationpolicy-resource-type"></a>authorizationPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可控制 Azure Active Directory 授权设置的策略。 它是从基本策略类型继承的单一实例，并且对于租户始终存在。 

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | 读取 authorizationPolicy 对象。 |
| [更新 authorizationPolicy](../api/authorizationpolicy-update.md) | 无 | 更新 authorizationPolicy 对象。 |

## <a name="properties"></a>属性  
| 属性 | 类型 | 说明 | 
|-|-|-|
|id|String| 授权策略的 ID。 必需。 只读。| 
|displayName|String| 此策略的显示名称。 |  
|description|String| 此策略的说明。|  
|guestUserRoleId|Guid| 表示应向来宾用户授予的角色的角色 templateId。 若要查找可用角色模板的列表，请参阅 [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) 。 当前以下角色受支持： User (a0b1b346-4d3e-4e8b-98f8-753987be4970) 、Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限制的来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。 | 
|enabledPreviewFeatures|集合 (字符串) | 租户上启用了专用预览的功能列表。 | 
|blockMsolPowerShell|Boolean| 若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。 如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。 这不会影响 Azure AD Connect 或 Microsoft Graph。 | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| 指定默认用户角色的某些可自定义权限。 | 
|allowedToUseSSPR|Boolean| 指示租户上的用户是否可以使用自助服务密码重置功能。 | 
|allowedToSignUpEmailBasedSubscriptions|Boolean| 指示用户是否可以注册基于电子邮件的订阅。 | 
|allowEmailVerifiedUsersToJoinOrganization|Boolean| 指示用户是否可以通过电子邮件验证加入租户。 | 


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
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true
}
```


