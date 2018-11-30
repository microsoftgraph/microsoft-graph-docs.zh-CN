---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: ad3b409f3abc4cc9e7476825f9dbf5b7c2120d92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046475"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="c8a02-103">skypeForBusinessPeerToPeerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8a02-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c8a02-104">属性</span><span class="sxs-lookup"><span data-stu-id="c8a02-104">Properties</span></span>

| <span data-ttu-id="c8a02-105">属性</span><span class="sxs-lookup"><span data-stu-id="c8a02-105">Property</span></span>          | <span data-ttu-id="c8a02-106">类型</span><span class="sxs-lookup"><span data-stu-id="c8a02-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c8a02-107">im</span><span class="sxs-lookup"><span data-stu-id="c8a02-107">im</span></span>                | <span data-ttu-id="c8a02-108">Int64</span><span class="sxs-lookup"><span data-stu-id="c8a02-108">Int64</span></span>  |
| <span data-ttu-id="c8a02-109">audio</span><span class="sxs-lookup"><span data-stu-id="c8a02-109">audio</span></span>             | <span data-ttu-id="c8a02-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c8a02-110">Int64</span></span>  |
| <span data-ttu-id="c8a02-111">video</span><span class="sxs-lookup"><span data-stu-id="c8a02-111">video</span></span>             | <span data-ttu-id="c8a02-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c8a02-112">Int64</span></span>  |
| <span data-ttu-id="c8a02-113">的</span><span class="sxs-lookup"><span data-stu-id="c8a02-113">appSharing</span></span>        | <span data-ttu-id="c8a02-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c8a02-114">Int64</span></span>  |
| <span data-ttu-id="c8a02-115">文件传输</span><span class="sxs-lookup"><span data-stu-id="c8a02-115">fileTransfer</span></span>      | <span data-ttu-id="c8a02-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c8a02-116">Int64</span></span>  |
| <span data-ttu-id="c8a02-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c8a02-117">reportRefreshDate</span></span> | <span data-ttu-id="c8a02-118">日期</span><span class="sxs-lookup"><span data-stu-id="c8a02-118">Date</span></span>   |
| <span data-ttu-id="c8a02-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="c8a02-119">reportDate</span></span>        | <span data-ttu-id="c8a02-120">日期</span><span class="sxs-lookup"><span data-stu-id="c8a02-120">Date</span></span>   |
| <span data-ttu-id="c8a02-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c8a02-121">reportPeriod</span></span>      | <span data-ttu-id="c8a02-122">String</span><span class="sxs-lookup"><span data-stu-id="c8a02-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c8a02-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8a02-123">JSON representation</span></span>

<span data-ttu-id="c8a02-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8a02-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
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
