---
title: educationIdentityCreationConfiguration 资源类型
description: 定义有关创建学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中创建用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 80c564999ca0e414c6475f858c5d3ebe5e037e4b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336020"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义有关创建学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中创建用户。

> **注意：** 如果你打开了目录同步以在本地 Active Directory 和 Azure Active Directory （Azure AD）之间同步，请改用[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)资源。

派生自[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-|:-|:-|
| **userDomains** | [educationIdentityDomain](educationidentitydomain.md)集合 |  设置要使用的每个用户类型的域的列表。  |


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
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
