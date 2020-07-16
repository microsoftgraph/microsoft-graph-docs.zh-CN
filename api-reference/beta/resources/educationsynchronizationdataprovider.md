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
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="ca913-104">educationSynchronizationDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca913-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="ca913-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca913-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca913-106">表示要用作[educationSynchronizationProfile]的同步源的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="ca913-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> <span data-ttu-id="ca913-107">**注意：** 此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="ca913-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="ca913-108">请参阅列出的特定类型的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="ca913-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="ca913-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="ca913-109">Providers</span></span>

| <span data-ttu-id="ca913-110">Data Provider</span><span class="sxs-lookup"><span data-stu-id="ca913-110">Data Provider</span></span>                                                             | <span data-ttu-id="ca913-111">Description</span><span class="sxs-lookup"><span data-stu-id="ca913-111">Description</span></span>                                                                                        |
|:--------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ca913-112">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="ca913-112">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="ca913-113">上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件</span><span class="sxs-lookup"><span data-stu-id="ca913-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="ca913-114">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="ca913-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="ca913-115">OneRoster v1.1 API</span><span class="sxs-lookup"><span data-stu-id="ca913-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="ca913-116">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="ca913-116">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="ca913-117">PowerSchool API</span><span class="sxs-lookup"><span data-stu-id="ca913-117">PowerSchool API</span></span>                                                                                    |

## <a name="properties"></a><span data-ttu-id="ca913-118">属性</span><span class="sxs-lookup"><span data-stu-id="ca913-118">Properties</span></span>

<span data-ttu-id="ca913-119">此类型不公开任何属性。</span><span class="sxs-lookup"><span data-stu-id="ca913-119">No properties are exposed by this type.</span></span>

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
