---
title: skypeForBusinessPeerToPeerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 4baf218ed9398a8f208c4d1d44a28579773dea6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874471"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="65e1a-103">skypeForBusinessPeerToPeerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="65e1a-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="65e1a-104">属性</span><span class="sxs-lookup"><span data-stu-id="65e1a-104">Properties</span></span>

| <span data-ttu-id="65e1a-105">属性</span><span class="sxs-lookup"><span data-stu-id="65e1a-105">Property</span></span>          | <span data-ttu-id="65e1a-106">类型</span><span class="sxs-lookup"><span data-stu-id="65e1a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="65e1a-107">im</span><span class="sxs-lookup"><span data-stu-id="65e1a-107">im</span></span>                | <span data-ttu-id="65e1a-108">Int64</span><span class="sxs-lookup"><span data-stu-id="65e1a-108">Int64</span></span>  |
| <span data-ttu-id="65e1a-109">audio</span><span class="sxs-lookup"><span data-stu-id="65e1a-109">audio</span></span>             | <span data-ttu-id="65e1a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="65e1a-110">Int64</span></span>  |
| <span data-ttu-id="65e1a-111">video</span><span class="sxs-lookup"><span data-stu-id="65e1a-111">video</span></span>             | <span data-ttu-id="65e1a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="65e1a-112">Int64</span></span>  |
| <span data-ttu-id="65e1a-113">的</span><span class="sxs-lookup"><span data-stu-id="65e1a-113">appSharing</span></span>        | <span data-ttu-id="65e1a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="65e1a-114">Int64</span></span>  |
| <span data-ttu-id="65e1a-115">文件传输</span><span class="sxs-lookup"><span data-stu-id="65e1a-115">fileTransfer</span></span>      | <span data-ttu-id="65e1a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="65e1a-116">Int64</span></span>  |
| <span data-ttu-id="65e1a-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="65e1a-117">reportRefreshDate</span></span> | <span data-ttu-id="65e1a-118">日期</span><span class="sxs-lookup"><span data-stu-id="65e1a-118">Date</span></span>   |
| <span data-ttu-id="65e1a-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="65e1a-119">reportDate</span></span>        | <span data-ttu-id="65e1a-120">日期</span><span class="sxs-lookup"><span data-stu-id="65e1a-120">Date</span></span>   |
| <span data-ttu-id="65e1a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="65e1a-121">reportPeriod</span></span>      | <span data-ttu-id="65e1a-122">String</span><span class="sxs-lookup"><span data-stu-id="65e1a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65e1a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65e1a-123">JSON representation</span></span>

<span data-ttu-id="65e1a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65e1a-124">The following is a JSON representation of the resource.</span></span>

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
