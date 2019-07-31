---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c28238cf35858745979a4d9659b1f649dbab7061
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972423"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 Azure Active Directory (Azure AD) 架构。

> **注意:** 此复杂类型是抽象的。 请参阅列出的特定类型的数据提供程序。

## <a name="derived-types"></a>派生类型
| 类型 | 说明 |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | 将 CSV 文件用作输入源。 |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | 与 PowerSchool 用作输入源。 |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | 与 OneRoster API 一起用于输入源。 |

## <a name="properties"></a>属性

此类型不公开任何属性。
