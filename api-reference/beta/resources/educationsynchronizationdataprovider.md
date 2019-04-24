---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SIS 架构。 这使系统可以了解如何将传入数据映射到 azure Active Directory (azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507037"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="49874-104">educationSynchronizationDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="49874-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49874-105">代表源 SIS 架构。</span><span class="sxs-lookup"><span data-stu-id="49874-105">Represents the source SIS schema.</span></span> <span data-ttu-id="49874-106">这使系统可以了解如何将传入数据映射到 azure Active Directory (azure AD) 架构。</span><span class="sxs-lookup"><span data-stu-id="49874-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="49874-107">**注意:** 此复杂类型是抽象的。</span><span class="sxs-lookup"><span data-stu-id="49874-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="49874-108">请参阅列出的特定类型的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="49874-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="49874-109">派生类型</span><span class="sxs-lookup"><span data-stu-id="49874-109">Derived types</span></span>
| <span data-ttu-id="49874-110">类型</span><span class="sxs-lookup"><span data-stu-id="49874-110">Type</span></span> | <span data-ttu-id="49874-111">说明</span><span class="sxs-lookup"><span data-stu-id="49874-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="49874-112">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="49874-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="49874-113">将 CSV 文件用作输入源。</span><span class="sxs-lookup"><span data-stu-id="49874-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="49874-114">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="49874-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="49874-115">与 PowerSchool 用作输入源。</span><span class="sxs-lookup"><span data-stu-id="49874-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="49874-116">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="49874-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="49874-117">与 OneRoster API 一起用于输入源。</span><span class="sxs-lookup"><span data-stu-id="49874-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="49874-118">属性</span><span class="sxs-lookup"><span data-stu-id="49874-118">Properties</span></span>

<span data-ttu-id="49874-119">此类型不公开任何属性。</span><span class="sxs-lookup"><span data-stu-id="49874-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
