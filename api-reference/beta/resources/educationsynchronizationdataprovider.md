---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 Azure Active Directory （Azure AD）架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: be0f50ec3cff0a8eec91cd43b4bb08371db806f3
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846161"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要用作[educationSynchronizationProfile]的同步源的数据提供程序。

> **注意：** 此复杂类型是抽象的。 请参阅列出的特定类型的数据提供程序。

## <a name="providers"></a>提供程序

| Data Provider                                                             | Description                                                                                        |
|:--------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [educationCsvDataProvider]                                                | 上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件 |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | PowerSchool API                                                                                    |

## <a name="properties"></a>属性

此类型不公开任何属性。

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
