---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f49d263703751b5dabd82ab904b6d572e5a7b263
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940720"
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
