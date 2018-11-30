---
title: skypeForBusinessParticipantActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: d65d7fd9c2c3389e47a8b1f94538be158efd2642
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045214"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="5faea-103">skypeForBusinessParticipantActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5faea-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5faea-104">属性</span><span class="sxs-lookup"><span data-stu-id="5faea-104">Properties</span></span>

| <span data-ttu-id="5faea-105">属性</span><span class="sxs-lookup"><span data-stu-id="5faea-105">Property</span></span>          | <span data-ttu-id="5faea-106">类型</span><span class="sxs-lookup"><span data-stu-id="5faea-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5faea-107">im</span><span class="sxs-lookup"><span data-stu-id="5faea-107">im</span></span>                | <span data-ttu-id="5faea-108">Int64</span><span class="sxs-lookup"><span data-stu-id="5faea-108">Int64</span></span>  |
| <span data-ttu-id="5faea-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="5faea-109">audioVideo</span></span>        | <span data-ttu-id="5faea-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5faea-110">Int64</span></span>  |
| <span data-ttu-id="5faea-111">的</span><span class="sxs-lookup"><span data-stu-id="5faea-111">appSharing</span></span>        | <span data-ttu-id="5faea-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5faea-112">Int64</span></span>  |
| <span data-ttu-id="5faea-113">web</span><span class="sxs-lookup"><span data-stu-id="5faea-113">web</span></span>               | <span data-ttu-id="5faea-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5faea-114">Int64</span></span>  |
| <span data-ttu-id="5faea-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="5faea-115">dialInOut3rdParty</span></span> | <span data-ttu-id="5faea-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5faea-116">Int64</span></span>  |
| <span data-ttu-id="5faea-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5faea-117">reportRefreshDate</span></span> | <span data-ttu-id="5faea-118">日期</span><span class="sxs-lookup"><span data-stu-id="5faea-118">Date</span></span>   |
| <span data-ttu-id="5faea-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="5faea-119">reportDate</span></span>        | <span data-ttu-id="5faea-120">日期</span><span class="sxs-lookup"><span data-stu-id="5faea-120">Date</span></span>   |
| <span data-ttu-id="5faea-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5faea-121">reportPeriod</span></span>      | <span data-ttu-id="5faea-122">String</span><span class="sxs-lookup"><span data-stu-id="5faea-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5faea-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5faea-123">JSON representation</span></span>

<span data-ttu-id="5faea-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5faea-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 196, 
  "appSharing": 196, 
  "web": 196, 
  "dialInOut3rdParty": 196, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
