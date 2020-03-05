---
title: skypeForBusinessOrganizerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 63bb5fe2464a20eae403e9eca165414f52417cde
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520385"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="6ec9d-103">skypeForBusinessOrganizerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ec9d-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

<span data-ttu-id="6ec9d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6ec9d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="6ec9d-105">属性</span><span class="sxs-lookup"><span data-stu-id="6ec9d-105">Properties</span></span>

| <span data-ttu-id="6ec9d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6ec9d-106">Property</span></span>           | <span data-ttu-id="6ec9d-107">类型</span><span class="sxs-lookup"><span data-stu-id="6ec9d-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="6ec9d-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="6ec9d-108">im</span></span>                 | <span data-ttu-id="6ec9d-109">Int64</span><span class="sxs-lookup"><span data-stu-id="6ec9d-109">Int64</span></span>  |
| <span data-ttu-id="6ec9d-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="6ec9d-110">audioVideo</span></span>         | <span data-ttu-id="6ec9d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="6ec9d-111">Int64</span></span>  |
| <span data-ttu-id="6ec9d-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="6ec9d-112">appSharing</span></span>         | <span data-ttu-id="6ec9d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="6ec9d-113">Int64</span></span>  |
| <span data-ttu-id="6ec9d-114">web</span><span class="sxs-lookup"><span data-stu-id="6ec9d-114">web</span></span>                | <span data-ttu-id="6ec9d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="6ec9d-115">Int64</span></span>  |
| <span data-ttu-id="6ec9d-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="6ec9d-116">dialInOut3rdParty</span></span>  | <span data-ttu-id="6ec9d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="6ec9d-117">Int64</span></span>  |
| <span data-ttu-id="6ec9d-118">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="6ec9d-118">dialInOutMicrosoft</span></span> | <span data-ttu-id="6ec9d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6ec9d-119">Int64</span></span>  |
| <span data-ttu-id="6ec9d-120">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6ec9d-120">reportRefreshDate</span></span>  | <span data-ttu-id="6ec9d-121">日期</span><span class="sxs-lookup"><span data-stu-id="6ec9d-121">Date</span></span>   |
| <span data-ttu-id="6ec9d-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="6ec9d-122">reportDate</span></span>         | <span data-ttu-id="6ec9d-123">日期</span><span class="sxs-lookup"><span data-stu-id="6ec9d-123">Date</span></span>   |
| <span data-ttu-id="6ec9d-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6ec9d-124">reportPeriod</span></span>       | <span data-ttu-id="6ec9d-125">String</span><span class="sxs-lookup"><span data-stu-id="6ec9d-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ec9d-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ec9d-126">JSON representation</span></span>

<span data-ttu-id="6ec9d-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ec9d-127">The following is a JSON representation of the resource.</span></span>

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
