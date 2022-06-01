---
title: userRegistrationMethodSummary 资源类型
description: 为每个身份验证方法注册的用户数的摘要。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e7c5288fb533f3b97ea5c69d7916e3cd3bc33d50
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820026"
---
# <a name="userregistrationmethodsummary-resource-type"></a>userRegistrationMethodSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为每个身份验证方法注册的用户数的摘要。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [usersRegisteredByMethod](../api/authenticationmethodsroot-usersregisteredbymethod.md) | userRegistrationMethodSummary | 获取为每个身份验证方法注册的用户数。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|totalUserCount|Int64|租户中的用户总数。|
|userRegistrationMethodCounts|[userRegistrationMethodCount](../resources/userregistrationmethodcount.md) 集合|为每个身份验证方法注册的用户数。|
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
  "@odata.type": "microsoft.graph.userRegistrationMethodSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationMethodCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationMethodCount"
    }
  ]
}
```
