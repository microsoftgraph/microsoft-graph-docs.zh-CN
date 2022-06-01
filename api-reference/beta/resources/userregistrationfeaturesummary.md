---
title: userRegistrationFeatureSummary 资源类型
description: 能够进行多重身份验证、Self-Service密码重置和无密码身份验证的用户摘要。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b058276eaa3bc9f12dbe46ddc33afbe06b0bc2f2
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820145"
---
# <a name="userregistrationfeaturesummary-resource-type"></a>userRegistrationFeatureSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示组织中能够进行多重身份验证、自助密码重置和无密码身份验证的用户数量的当前状态。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [usersRegisteredByFeature](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | userRegistrationFeatureSummary | 获取能够进行多重身份验证、Self-Service密码重置和无密码身份验证的用户数。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|totalUserCount|Int64|用户帐户总数，不包括被阻止的帐户|
|userRegistrationFeatureCounts|[userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md) 集合|注册或支持多重身份验证、Self-Service密码重置和无密码身份验证的用户数。|
|userRoles|includedUserRoles|用户角色类型。 可能的值是：`all`、`privilegedAdmin`、`admin`、`user`。|
|userTypes|includedUserTypes|用户类型。 可取值为：`all`、`member`、`guest`。|

该值 `privilegedAdmin` 由以下特权管理员角色组成：

* 全局管理员
* 安全管理员
* 条件访问管理员
* Exchange 管理员
* SharePoint 管理员
* 支持管理员
* 帐务管理员
* 用户管理员
* 身份验证管理员

该值 `admin` 包括所有 Azure AD 管理员角色。 

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationFeatureCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
    }
  ]
}
```
