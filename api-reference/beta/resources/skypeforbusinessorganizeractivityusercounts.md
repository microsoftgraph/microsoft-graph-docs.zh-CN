---
title: skypeForBusinessOrganizerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b6fcb2114e78bd9aabb170795b49d80bb58e6844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964870"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="0683f-103">skypeForBusinessOrganizerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="0683f-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0683f-104">属性</span><span class="sxs-lookup"><span data-stu-id="0683f-104">Properties</span></span>

| <span data-ttu-id="0683f-105">属性</span><span class="sxs-lookup"><span data-stu-id="0683f-105">Property</span></span>           | <span data-ttu-id="0683f-106">类型</span><span class="sxs-lookup"><span data-stu-id="0683f-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="0683f-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="0683f-107">im</span></span>                 | <span data-ttu-id="0683f-108">Int64</span><span class="sxs-lookup"><span data-stu-id="0683f-108">Int64</span></span>  |
| <span data-ttu-id="0683f-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="0683f-109">audioVideo</span></span>         | <span data-ttu-id="0683f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="0683f-110">Int64</span></span>  |
| <span data-ttu-id="0683f-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="0683f-111">appSharing</span></span>         | <span data-ttu-id="0683f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0683f-112">Int64</span></span>  |
| <span data-ttu-id="0683f-113">web</span><span class="sxs-lookup"><span data-stu-id="0683f-113">web</span></span>                | <span data-ttu-id="0683f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0683f-114">Int64</span></span>  |
| <span data-ttu-id="0683f-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="0683f-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="0683f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0683f-116">Int64</span></span>  |
| <span data-ttu-id="0683f-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="0683f-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="0683f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0683f-118">Int64</span></span>  |
| <span data-ttu-id="0683f-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0683f-119">reportRefreshDate</span></span>  | <span data-ttu-id="0683f-120">日期</span><span class="sxs-lookup"><span data-stu-id="0683f-120">Date</span></span>   |
| <span data-ttu-id="0683f-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="0683f-121">reportDate</span></span>         | <span data-ttu-id="0683f-122">日期</span><span class="sxs-lookup"><span data-stu-id="0683f-122">Date</span></span>   |
| <span data-ttu-id="0683f-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0683f-123">reportPeriod</span></span>       | <span data-ttu-id="0683f-124">String</span><span class="sxs-lookup"><span data-stu-id="0683f-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0683f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0683f-125">JSON representation</span></span>

<span data-ttu-id="0683f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0683f-126">The following is a JSON representation of the resource.</span></span>

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
