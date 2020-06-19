---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 Azure Active Directory （Azure AD）架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f0691a7157fb189e75e862448069ff8ebdeee9f7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790920"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="417cc-104">educationSynchronizationDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="417cc-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="417cc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="417cc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="417cc-106">表示要用作[educationSynchronizationProfile]的同步源的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="417cc-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> <span data-ttu-id="417cc-107">**注意：** 此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="417cc-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="417cc-108">请参阅列出的特定类型的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="417cc-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="417cc-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="417cc-109">Providers</span></span>

| <span data-ttu-id="417cc-110">Data Provider</span><span class="sxs-lookup"><span data-stu-id="417cc-110">Data Provider</span></span>                       | <span data-ttu-id="417cc-111">说明</span><span class="sxs-lookup"><span data-stu-id="417cc-111">Description</span></span>                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="417cc-112">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="417cc-112">[educationCsvDataProvider]</span></span>          | <span data-ttu-id="417cc-113">上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件</span><span class="sxs-lookup"><span data-stu-id="417cc-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="417cc-114">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="417cc-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="417cc-115">OneRoster v1.1 API</span><span class="sxs-lookup"><span data-stu-id="417cc-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="417cc-116">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="417cc-116">[educationPowerSchoolDataProvider]</span></span>  | <span data-ttu-id="417cc-117">PowerSchool API</span><span class="sxs-lookup"><span data-stu-id="417cc-117">PowerSchool API</span></span>                                                                                    |

## <a name="properties"></a><span data-ttu-id="417cc-118">属性</span><span class="sxs-lookup"><span data-stu-id="417cc-118">Properties</span></span>

<span data-ttu-id="417cc-119">此类型不公开任何属性。</span><span class="sxs-lookup"><span data-stu-id="417cc-119">No properties are exposed by this type.</span></span>

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
