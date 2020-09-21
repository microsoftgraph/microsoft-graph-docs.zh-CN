---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 952d0a7f9a40f41ad87d632386d9d567036cfec7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989652"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="5b51e-104">educationSynchronizationDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b51e-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="5b51e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b51e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b51e-106">表示要用作 [educationSynchronizationProfile]的同步源的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="5b51e-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> [!NOTE]
> <span data-ttu-id="5b51e-107">此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="5b51e-107">This complex type is abstract.</span></span> <span data-ttu-id="5b51e-108">请参阅列出的特定类型的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="5b51e-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="5b51e-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="5b51e-109">Providers</span></span>

| <span data-ttu-id="5b51e-110">Data Provider</span><span class="sxs-lookup"><span data-stu-id="5b51e-110">Data Provider</span></span>                                                             | <span data-ttu-id="5b51e-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b51e-111">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5b51e-112">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="5b51e-112">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="5b51e-113">上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件</span><span class="sxs-lookup"><span data-stu-id="5b51e-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="5b51e-114">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="5b51e-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="5b51e-115">OneRoster v1.1 API</span><span class="sxs-lookup"><span data-stu-id="5b51e-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="5b51e-116">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="5b51e-116">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="5b51e-117">PowerSchool API</span><span class="sxs-lookup"><span data-stu-id="5b51e-117">PowerSchool API</span></span>                                                                                    |

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md


