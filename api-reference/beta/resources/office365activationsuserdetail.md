---
title: office365ActivationsUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3e2b7d5fb3c42db02407a187649544b2560f898a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982853"
---
# <a name="office365activationsuserdetail-resource-type"></a>office365ActivationsUserDetail 资源类型

## <a name="properties"></a>属性

| 属性             | 类型                                     | 说明                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | 日期                                     | 内容最晚日期。          |
| userPrincipalName    | 字符串                                   | 用户主体名称 (UPN) 的用户。 UPN 是基于 Internet 标准 RFC 822 用户 Internet 风格登录名。 按照惯例，这应映射到用户的电子邮件名称。 常规格式为 alias@domain，域必须存在于中的已验证域的租户的集合。 创建用户时此属性是必需的。 |
| displayName          | String                                   | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 |
| userActivationCounts | [userActivationCounts](../resources/useractivationcounts.md)集合 | 用户的最新的产品激活计算的所有已分配的产品类型的所有平台上。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
