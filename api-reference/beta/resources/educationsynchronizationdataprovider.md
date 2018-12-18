---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
ms.openlocfilehash: 04cbd38a158475c3a039a755ff885a6796ae3bf1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339884"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 

> **注意：** 此复杂类型是抽象类。 引用的特定类型的数据提供程序列出。

## <a name="derived-types"></a>派生的类型
| Type | 说明 | 
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | 作为输入源用于 CSV 文件。 |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | 用于 PowerSchool 作为输入源。 |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | 作为输入源用于 OneRoster API。 |

## <a name="properties"></a>Properties

此类型不公开的任何属性。
