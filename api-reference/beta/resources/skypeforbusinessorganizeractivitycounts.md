---
title: skypeForBusinessOrganizerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 9f6c77e86f76ac2e34fb87cf8ca5b6bded35a2a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461157"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="bc672-103">skypeForBusinessOrganizerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc672-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bc672-104">属性</span><span class="sxs-lookup"><span data-stu-id="bc672-104">Properties</span></span>

| <span data-ttu-id="bc672-105">属性</span><span class="sxs-lookup"><span data-stu-id="bc672-105">Property</span></span>           | <span data-ttu-id="bc672-106">类型</span><span class="sxs-lookup"><span data-stu-id="bc672-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="bc672-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="bc672-107">im</span></span>                 | <span data-ttu-id="bc672-108">Int64</span><span class="sxs-lookup"><span data-stu-id="bc672-108">Int64</span></span>  |
| <span data-ttu-id="bc672-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="bc672-109">audioVideo</span></span>         | <span data-ttu-id="bc672-110">Int64</span><span class="sxs-lookup"><span data-stu-id="bc672-110">Int64</span></span>  |
| <span data-ttu-id="bc672-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="bc672-111">appSharing</span></span>         | <span data-ttu-id="bc672-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bc672-112">Int64</span></span>  |
| <span data-ttu-id="bc672-113">web</span><span class="sxs-lookup"><span data-stu-id="bc672-113">web</span></span>                | <span data-ttu-id="bc672-114">Int64</span><span class="sxs-lookup"><span data-stu-id="bc672-114">Int64</span></span>  |
| <span data-ttu-id="bc672-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="bc672-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="bc672-116">Int64</span><span class="sxs-lookup"><span data-stu-id="bc672-116">Int64</span></span>  |
| <span data-ttu-id="bc672-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="bc672-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="bc672-118">Int64</span><span class="sxs-lookup"><span data-stu-id="bc672-118">Int64</span></span>  |
| <span data-ttu-id="bc672-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bc672-119">reportRefreshDate</span></span>  | <span data-ttu-id="bc672-120">Date</span><span class="sxs-lookup"><span data-stu-id="bc672-120">Date</span></span>   |
| <span data-ttu-id="bc672-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="bc672-121">reportDate</span></span>         | <span data-ttu-id="bc672-122">Date</span><span class="sxs-lookup"><span data-stu-id="bc672-122">Date</span></span>   |
| <span data-ttu-id="bc672-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bc672-123">reportPeriod</span></span>       | <span data-ttu-id="bc672-124">字符串</span><span class="sxs-lookup"><span data-stu-id="bc672-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc672-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc672-125">JSON representation</span></span>

<span data-ttu-id="bc672-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc672-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
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
