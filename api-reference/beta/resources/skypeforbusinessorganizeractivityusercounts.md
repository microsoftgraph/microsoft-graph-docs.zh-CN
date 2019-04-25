---
title: skypeForBusinessOrganizerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 39ab5844adb9525b4e0f100892927d200609040c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534862"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="a643e-103">skypeForBusinessOrganizerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a643e-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a643e-104">属性</span><span class="sxs-lookup"><span data-stu-id="a643e-104">Properties</span></span>

| <span data-ttu-id="a643e-105">属性</span><span class="sxs-lookup"><span data-stu-id="a643e-105">Property</span></span>           | <span data-ttu-id="a643e-106">类型</span><span class="sxs-lookup"><span data-stu-id="a643e-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="a643e-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="a643e-107">im</span></span>                 | <span data-ttu-id="a643e-108">Int64</span><span class="sxs-lookup"><span data-stu-id="a643e-108">Int64</span></span>  |
| <span data-ttu-id="a643e-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="a643e-109">audioVideo</span></span>         | <span data-ttu-id="a643e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a643e-110">Int64</span></span>  |
| <span data-ttu-id="a643e-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="a643e-111">appSharing</span></span>         | <span data-ttu-id="a643e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a643e-112">Int64</span></span>  |
| <span data-ttu-id="a643e-113">web</span><span class="sxs-lookup"><span data-stu-id="a643e-113">web</span></span>                | <span data-ttu-id="a643e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a643e-114">Int64</span></span>  |
| <span data-ttu-id="a643e-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="a643e-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="a643e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a643e-116">Int64</span></span>  |
| <span data-ttu-id="a643e-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="a643e-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="a643e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a643e-118">Int64</span></span>  |
| <span data-ttu-id="a643e-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a643e-119">reportRefreshDate</span></span>  | <span data-ttu-id="a643e-120">Date</span><span class="sxs-lookup"><span data-stu-id="a643e-120">Date</span></span>   |
| <span data-ttu-id="a643e-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="a643e-121">reportDate</span></span>         | <span data-ttu-id="a643e-122">Date</span><span class="sxs-lookup"><span data-stu-id="a643e-122">Date</span></span>   |
| <span data-ttu-id="a643e-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a643e-123">reportPeriod</span></span>       | <span data-ttu-id="a643e-124">String</span><span class="sxs-lookup"><span data-stu-id="a643e-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a643e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a643e-125">JSON representation</span></span>

<span data-ttu-id="a643e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a643e-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
