---
title: skypeForBusinessPeerToPeerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4075af51edb747146a764f8337e3ab2e4734caa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964863"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="07e0a-103">skypeForBusinessPeerToPeerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="07e0a-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="07e0a-104">属性</span><span class="sxs-lookup"><span data-stu-id="07e0a-104">Properties</span></span>

| <span data-ttu-id="07e0a-105">属性</span><span class="sxs-lookup"><span data-stu-id="07e0a-105">Property</span></span>          | <span data-ttu-id="07e0a-106">类型</span><span class="sxs-lookup"><span data-stu-id="07e0a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="07e0a-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="07e0a-107">im</span></span>                | <span data-ttu-id="07e0a-108">Int64</span><span class="sxs-lookup"><span data-stu-id="07e0a-108">Int64</span></span>  |
| <span data-ttu-id="07e0a-109">audio</span><span class="sxs-lookup"><span data-stu-id="07e0a-109">audio</span></span>             | <span data-ttu-id="07e0a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="07e0a-110">Int64</span></span>  |
| <span data-ttu-id="07e0a-111">video</span><span class="sxs-lookup"><span data-stu-id="07e0a-111">video</span></span>             | <span data-ttu-id="07e0a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="07e0a-112">Int64</span></span>  |
| <span data-ttu-id="07e0a-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="07e0a-113">appSharing</span></span>        | <span data-ttu-id="07e0a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="07e0a-114">Int64</span></span>  |
| <span data-ttu-id="07e0a-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="07e0a-115">fileTransfer</span></span>      | <span data-ttu-id="07e0a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="07e0a-116">Int64</span></span>  |
| <span data-ttu-id="07e0a-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="07e0a-117">reportRefreshDate</span></span> | <span data-ttu-id="07e0a-118">日期</span><span class="sxs-lookup"><span data-stu-id="07e0a-118">Date</span></span>   |
| <span data-ttu-id="07e0a-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="07e0a-119">reportDate</span></span>        | <span data-ttu-id="07e0a-120">日期</span><span class="sxs-lookup"><span data-stu-id="07e0a-120">Date</span></span>   |
| <span data-ttu-id="07e0a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="07e0a-121">reportPeriod</span></span>      | <span data-ttu-id="07e0a-122">String</span><span class="sxs-lookup"><span data-stu-id="07e0a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="07e0a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07e0a-123">JSON representation</span></span>

<span data-ttu-id="07e0a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07e0a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
