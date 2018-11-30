---
title: skypeForBusinessOrganizerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: f11d303bd8737d9fb2870042ee93557343d44a2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047504"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a><span data-ttu-id="e8497-103">skypeForBusinessOrganizerActivityMinuteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8497-103">skypeForBusinessOrganizerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e8497-104">属性</span><span class="sxs-lookup"><span data-stu-id="e8497-104">Properties</span></span>

| <span data-ttu-id="e8497-105">属性</span><span class="sxs-lookup"><span data-stu-id="e8497-105">Property</span></span>           | <span data-ttu-id="e8497-106">类型</span><span class="sxs-lookup"><span data-stu-id="e8497-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="e8497-107">audioVideo</span><span class="sxs-lookup"><span data-stu-id="e8497-107">audioVideo</span></span>         | <span data-ttu-id="e8497-108">Int64</span><span class="sxs-lookup"><span data-stu-id="e8497-108">Int64</span></span>  |
| <span data-ttu-id="e8497-109">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="e8497-109">dialInOut3rdParty</span></span>  | <span data-ttu-id="e8497-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e8497-110">Int64</span></span>  |
| <span data-ttu-id="e8497-111">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="e8497-111">dialInOutMicrosoft</span></span> | <span data-ttu-id="e8497-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e8497-112">Int64</span></span>  |
| <span data-ttu-id="e8497-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e8497-113">reportRefreshDate</span></span>  | <span data-ttu-id="e8497-114">日期</span><span class="sxs-lookup"><span data-stu-id="e8497-114">Date</span></span>   |
| <span data-ttu-id="e8497-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="e8497-115">reportDate</span></span>         | <span data-ttu-id="e8497-116">日期</span><span class="sxs-lookup"><span data-stu-id="e8497-116">Date</span></span>   |
| <span data-ttu-id="e8497-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e8497-117">reportPeriod</span></span>       | <span data-ttu-id="e8497-118">String</span><span class="sxs-lookup"><span data-stu-id="e8497-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e8497-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8497-119">JSON representation</span></span>

<span data-ttu-id="e8497-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8497-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024, 
  "dialInMicrosoft": 1024, 
  "dialOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
