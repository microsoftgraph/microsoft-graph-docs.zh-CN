---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 Azure Active Directory （Azure AD）架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f20bea087a23f14acd7184c5211d21687409897a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434968"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="65d34-104">educationSynchronizationDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="65d34-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="65d34-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d34-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65d34-106">表示要用作[educationSynchronizationProfile]的同步源的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="65d34-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> [!NOTE]
> <span data-ttu-id="65d34-107">此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="65d34-107">This complex type is abstract.</span></span> <span data-ttu-id="65d34-108">请参阅列出的特定类型的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="65d34-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="65d34-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="65d34-109">Providers</span></span>

| <span data-ttu-id="65d34-110">Data Provider</span><span class="sxs-lookup"><span data-stu-id="65d34-110">Data Provider</span></span>                                                             | <span data-ttu-id="65d34-111">说明</span><span class="sxs-lookup"><span data-stu-id="65d34-111">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="65d34-112">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="65d34-112">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="65d34-113">上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件</span><span class="sxs-lookup"><span data-stu-id="65d34-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="65d34-114">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="65d34-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="65d34-115">OneRoster v1.1 API</span><span class="sxs-lookup"><span data-stu-id="65d34-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="65d34-116">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="65d34-116">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="65d34-117">PowerSchool API</span><span class="sxs-lookup"><span data-stu-id="65d34-117">PowerSchool API</span></span>                                                                                    |

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
