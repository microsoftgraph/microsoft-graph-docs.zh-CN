---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 azure Active Directory (azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 70c48e8d18191172be25046d8b1d60c0765c5187
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334025"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 azure Active Directory (azure AD) 架构。

> **注意:** 此复杂类型是抽象的。 请参阅列出的特定类型的数据提供程序。

## <a name="derived-types"></a>派生类型
| 类型 | 说明 |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | 将 CSV 文件用作输入源。 |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | 与 PowerSchool 用作输入源。 |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | 与 OneRoster API 一起用于输入源。 |

## <a name="properties"></a>属性

此类型不公开任何属性。
