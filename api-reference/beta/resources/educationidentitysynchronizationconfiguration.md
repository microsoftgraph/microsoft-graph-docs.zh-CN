---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1ffa1bbcd3f96c86818c68d350236086d0975187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501792"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。

## <a name="derived-types"></a>派生类型
| 类型 | 说明 |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | 使用此类型可匹配 Azure Active Directory （Azure AD）中的现有用户帐户。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | 使用此类型在 Azure AD 中创建新用户帐户。 |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

