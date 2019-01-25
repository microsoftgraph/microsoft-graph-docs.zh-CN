---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515494"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
