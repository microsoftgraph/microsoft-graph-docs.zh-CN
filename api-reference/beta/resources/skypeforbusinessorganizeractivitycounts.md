---
title: skypeForBusinessOrganizerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 688b9deb37412a939b94b7657946e5441dbe6de6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520399"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="b1777-103">skypeForBusinessOrganizerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1777-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

<span data-ttu-id="b1777-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b1777-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b1777-105">属性</span><span class="sxs-lookup"><span data-stu-id="b1777-105">Properties</span></span>

| <span data-ttu-id="b1777-106">属性</span><span class="sxs-lookup"><span data-stu-id="b1777-106">Property</span></span>           | <span data-ttu-id="b1777-107">类型</span><span class="sxs-lookup"><span data-stu-id="b1777-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="b1777-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="b1777-108">im</span></span>                 | <span data-ttu-id="b1777-109">Int64</span><span class="sxs-lookup"><span data-stu-id="b1777-109">Int64</span></span>  |
| <span data-ttu-id="b1777-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="b1777-110">audioVideo</span></span>         | <span data-ttu-id="b1777-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b1777-111">Int64</span></span>  |
| <span data-ttu-id="b1777-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="b1777-112">appSharing</span></span>         | <span data-ttu-id="b1777-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b1777-113">Int64</span></span>  |
| <span data-ttu-id="b1777-114">web</span><span class="sxs-lookup"><span data-stu-id="b1777-114">web</span></span>                | <span data-ttu-id="b1777-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b1777-115">Int64</span></span>  |
| <span data-ttu-id="b1777-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="b1777-116">dialInOut3rdParty</span></span>  | <span data-ttu-id="b1777-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b1777-117">Int64</span></span>  |
| <span data-ttu-id="b1777-118">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="b1777-118">dialInOutMicrosoft</span></span> | <span data-ttu-id="b1777-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b1777-119">Int64</span></span>  |
| <span data-ttu-id="b1777-120">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b1777-120">reportRefreshDate</span></span>  | <span data-ttu-id="b1777-121">日期</span><span class="sxs-lookup"><span data-stu-id="b1777-121">Date</span></span>   |
| <span data-ttu-id="b1777-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="b1777-122">reportDate</span></span>         | <span data-ttu-id="b1777-123">日期</span><span class="sxs-lookup"><span data-stu-id="b1777-123">Date</span></span>   |
| <span data-ttu-id="b1777-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b1777-124">reportPeriod</span></span>       | <span data-ttu-id="b1777-125">String</span><span class="sxs-lookup"><span data-stu-id="b1777-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1777-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1777-126">JSON representation</span></span>

<span data-ttu-id="b1777-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1777-127">The following is a JSON representation of the resource.</span></span>

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
