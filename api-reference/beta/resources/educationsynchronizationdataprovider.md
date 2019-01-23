---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f1e51bd0039b28aa08fa71956efc5143df77651c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420967"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 

> **注意：** 此复杂类型是抽象类。 引用的特定类型的数据提供程序列出。

## <a name="derived-types"></a>派生的类型
| 类型 | 说明 | 
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | 作为输入源用于 CSV 文件。 |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | 用于 PowerSchool 作为输入源。 |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | 作为输入源用于 OneRoster API。 |

## <a name="properties"></a>属性

此类型不公开的任何属性。



<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationDataProvider "
}-->

```json
{
}
```
