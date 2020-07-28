---
title: educationIdentityCreationConfiguration 资源类型
description: 定义有关创建学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中创建用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 33f96eab7af8b35720afd5946d83c43db0f20c81
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435045"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义有关创建学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中创建用户。

> [!WARNING]
> 如果你打开了目录同步以在本地 Active Directory 和 Azure Active Directory （Azure AD）之间同步，请改用[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)资源。

派生自[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)。

## <a name="properties"></a>属性

| 属性    | 类型                                                             | 说明                                    |
| :---------- | :--------------------------------------------------------------- | :--------------------------------------------- |
| userDomains | [educationIdentityDomain](educationidentitydomain.md)集合 | 设置要使用的每个用户类型的域的列表。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
  "userDomains": [
    {
      "@odata.type": "microsoft.graph.educationIdentityDomain"
    }
  ]
}
```
