---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515494"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="96465-104">educationSynchronizationDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="96465-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96465-105">代表源 SI 架构。</span><span class="sxs-lookup"><span data-stu-id="96465-105">Represents the source SIS schema.</span></span> <span data-ttu-id="96465-106">这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。</span><span class="sxs-lookup"><span data-stu-id="96465-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="96465-107">**注意：** 此复杂类型是抽象类。</span><span class="sxs-lookup"><span data-stu-id="96465-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="96465-108">引用的特定类型的数据提供程序列出。</span><span class="sxs-lookup"><span data-stu-id="96465-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="96465-109">派生的类型</span><span class="sxs-lookup"><span data-stu-id="96465-109">Derived types</span></span>
| <span data-ttu-id="96465-110">类型</span><span class="sxs-lookup"><span data-stu-id="96465-110">Type</span></span> | <span data-ttu-id="96465-111">说明</span><span class="sxs-lookup"><span data-stu-id="96465-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="96465-112">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="96465-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="96465-113">作为输入源用于 CSV 文件。</span><span class="sxs-lookup"><span data-stu-id="96465-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="96465-114">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="96465-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="96465-115">用于 PowerSchool 作为输入源。</span><span class="sxs-lookup"><span data-stu-id="96465-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="96465-116">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="96465-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="96465-117">作为输入源用于 OneRoster API。</span><span class="sxs-lookup"><span data-stu-id="96465-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="96465-118">属性</span><span class="sxs-lookup"><span data-stu-id="96465-118">Properties</span></span>

<span data-ttu-id="96465-119">此类型不公开的任何属性。</span><span class="sxs-lookup"><span data-stu-id="96465-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
