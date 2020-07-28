---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c3531999065abc22cc0ecb1870b4bd1bb5f45b7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435017"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。

## <a name="derived-types"></a>派生类型

| 类型                                                                                | 说明                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) | 使用此类型可**匹配**Azure Active Directory 中的现有用户帐户。 |
| [educationIdentityCreationConfiguration](educationidentitycreationconfiguration.md) | 使用此类型在 Azure Active Directory 中**创建新**用户帐户。                              |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{}
```
