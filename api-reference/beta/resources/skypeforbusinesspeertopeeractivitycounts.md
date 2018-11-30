---
title: skypeForBusinessPeerToPeerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: cdc8ec2a63c4a03ac8b77bedba06c6addfba4584
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044800"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="eb273-103">skypeForBusinessPeerToPeerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb273-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="eb273-104">属性</span><span class="sxs-lookup"><span data-stu-id="eb273-104">Properties</span></span>

| <span data-ttu-id="eb273-105">属性</span><span class="sxs-lookup"><span data-stu-id="eb273-105">Property</span></span>          | <span data-ttu-id="eb273-106">类型</span><span class="sxs-lookup"><span data-stu-id="eb273-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="eb273-107">im</span><span class="sxs-lookup"><span data-stu-id="eb273-107">im</span></span>                | <span data-ttu-id="eb273-108">Int64</span><span class="sxs-lookup"><span data-stu-id="eb273-108">Int64</span></span>  |
| <span data-ttu-id="eb273-109">audio</span><span class="sxs-lookup"><span data-stu-id="eb273-109">audio</span></span>             | <span data-ttu-id="eb273-110">Int64</span><span class="sxs-lookup"><span data-stu-id="eb273-110">Int64</span></span>  |
| <span data-ttu-id="eb273-111">video</span><span class="sxs-lookup"><span data-stu-id="eb273-111">video</span></span>             | <span data-ttu-id="eb273-112">Int64</span><span class="sxs-lookup"><span data-stu-id="eb273-112">Int64</span></span>  |
| <span data-ttu-id="eb273-113">的</span><span class="sxs-lookup"><span data-stu-id="eb273-113">appSharing</span></span>        | <span data-ttu-id="eb273-114">Int64</span><span class="sxs-lookup"><span data-stu-id="eb273-114">Int64</span></span>  |
| <span data-ttu-id="eb273-115">文件传输</span><span class="sxs-lookup"><span data-stu-id="eb273-115">fileTransfer</span></span>      | <span data-ttu-id="eb273-116">Int64</span><span class="sxs-lookup"><span data-stu-id="eb273-116">Int64</span></span>  |
| <span data-ttu-id="eb273-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="eb273-117">reportRefreshDate</span></span> | <span data-ttu-id="eb273-118">日期</span><span class="sxs-lookup"><span data-stu-id="eb273-118">Date</span></span>   |
| <span data-ttu-id="eb273-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="eb273-119">reportDate</span></span>        | <span data-ttu-id="eb273-120">日期</span><span class="sxs-lookup"><span data-stu-id="eb273-120">Date</span></span>   |
| <span data-ttu-id="eb273-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="eb273-121">reportPeriod</span></span>      | <span data-ttu-id="eb273-122">String</span><span class="sxs-lookup"><span data-stu-id="eb273-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb273-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb273-123">JSON representation</span></span>

<span data-ttu-id="eb273-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb273-124">The following is a JSON representation of the resource.</span></span>

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
