---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的抽象基类。 派生的类定义同步标识的行为。 以下是派生的类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 59dca28f82de0340aa289c6ea96ef5e252f60e85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412903"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

所有学校数据配置文件标识同步配置的抽象基类。 派生的类定义同步标识的行为。 以下是派生的类型。

## <a name="derived-types"></a>派生的类型
| 类型 | 说明 | 
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | 使用此类型来匹配 Azure Active Directory (Azure AD) 中的现有用户帐户。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | 使用此类型在 Azure AD 中创建新的用户帐户。 |

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```
