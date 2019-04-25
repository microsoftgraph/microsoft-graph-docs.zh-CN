---
title: skypeForBusinessPeerToPeerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 4baf218ed9398a8f208c4d1d44a28579773dea6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523453"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="7c4eb-103">skypeForBusinessPeerToPeerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c4eb-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7c4eb-104">属性</span><span class="sxs-lookup"><span data-stu-id="7c4eb-104">Properties</span></span>

| <span data-ttu-id="7c4eb-105">属性</span><span class="sxs-lookup"><span data-stu-id="7c4eb-105">Property</span></span>          | <span data-ttu-id="7c4eb-106">类型</span><span class="sxs-lookup"><span data-stu-id="7c4eb-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7c4eb-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="7c4eb-107">im</span></span>                | <span data-ttu-id="7c4eb-108">Int64</span><span class="sxs-lookup"><span data-stu-id="7c4eb-108">Int64</span></span>  |
| <span data-ttu-id="7c4eb-109">audio</span><span class="sxs-lookup"><span data-stu-id="7c4eb-109">audio</span></span>             | <span data-ttu-id="7c4eb-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7c4eb-110">Int64</span></span>  |
| <span data-ttu-id="7c4eb-111">video</span><span class="sxs-lookup"><span data-stu-id="7c4eb-111">video</span></span>             | <span data-ttu-id="7c4eb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7c4eb-112">Int64</span></span>  |
| <span data-ttu-id="7c4eb-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="7c4eb-113">appSharing</span></span>        | <span data-ttu-id="7c4eb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7c4eb-114">Int64</span></span>  |
| <span data-ttu-id="7c4eb-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="7c4eb-115">fileTransfer</span></span>      | <span data-ttu-id="7c4eb-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7c4eb-116">Int64</span></span>  |
| <span data-ttu-id="7c4eb-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7c4eb-117">reportRefreshDate</span></span> | <span data-ttu-id="7c4eb-118">Date</span><span class="sxs-lookup"><span data-stu-id="7c4eb-118">Date</span></span>   |
| <span data-ttu-id="7c4eb-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="7c4eb-119">reportDate</span></span>        | <span data-ttu-id="7c4eb-120">Date</span><span class="sxs-lookup"><span data-stu-id="7c4eb-120">Date</span></span>   |
| <span data-ttu-id="7c4eb-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7c4eb-121">reportPeriod</span></span>      | <span data-ttu-id="7c4eb-122">String</span><span class="sxs-lookup"><span data-stu-id="7c4eb-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c4eb-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c4eb-123">JSON representation</span></span>

<span data-ttu-id="7c4eb-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c4eb-124">The following is a JSON representation of the resource.</span></span>

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
