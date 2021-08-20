---
title: office365ActivationsUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: adbefd4a160ba00e9478abebec5932f97464328a633bb26719eaed4818bf3f22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239026"
---
# <a name="office365activationsuserdetail-resource-type"></a>office365ActivationsUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性             | 类型                                     | 说明                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | 日期                                     | 内容的最新日期。          |
| userPrincipalName    | String                                   | 用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 |
| displayName          | String                                   | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 |
| userActivationCounts | [userActivationCounts](../resources/useractivationcounts.md) 集合 | 对于所有分配的产品类型，用户的最新产品激活计数在所有平台上。 |

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


