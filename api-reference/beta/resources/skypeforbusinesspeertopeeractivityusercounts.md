---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 619e581fcdd25dda10be7210aefe5db8e4dcd8b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828635"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="c3e43-103">skypeForBusinessPeerToPeerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3e43-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c3e43-104">属性</span><span class="sxs-lookup"><span data-stu-id="c3e43-104">Properties</span></span>

| <span data-ttu-id="c3e43-105">属性</span><span class="sxs-lookup"><span data-stu-id="c3e43-105">Property</span></span>          | <span data-ttu-id="c3e43-106">类型</span><span class="sxs-lookup"><span data-stu-id="c3e43-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c3e43-107">im</span><span class="sxs-lookup"><span data-stu-id="c3e43-107">im</span></span>                | <span data-ttu-id="c3e43-108">Int64</span><span class="sxs-lookup"><span data-stu-id="c3e43-108">Int64</span></span>  |
| <span data-ttu-id="c3e43-109">audio</span><span class="sxs-lookup"><span data-stu-id="c3e43-109">audio</span></span>             | <span data-ttu-id="c3e43-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c3e43-110">Int64</span></span>  |
| <span data-ttu-id="c3e43-111">video</span><span class="sxs-lookup"><span data-stu-id="c3e43-111">video</span></span>             | <span data-ttu-id="c3e43-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c3e43-112">Int64</span></span>  |
| <span data-ttu-id="c3e43-113">的</span><span class="sxs-lookup"><span data-stu-id="c3e43-113">appSharing</span></span>        | <span data-ttu-id="c3e43-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c3e43-114">Int64</span></span>  |
| <span data-ttu-id="c3e43-115">文件传输</span><span class="sxs-lookup"><span data-stu-id="c3e43-115">fileTransfer</span></span>      | <span data-ttu-id="c3e43-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c3e43-116">Int64</span></span>  |
| <span data-ttu-id="c3e43-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c3e43-117">reportRefreshDate</span></span> | <span data-ttu-id="c3e43-118">日期</span><span class="sxs-lookup"><span data-stu-id="c3e43-118">Date</span></span>   |
| <span data-ttu-id="c3e43-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="c3e43-119">reportDate</span></span>        | <span data-ttu-id="c3e43-120">日期</span><span class="sxs-lookup"><span data-stu-id="c3e43-120">Date</span></span>   |
| <span data-ttu-id="c3e43-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c3e43-121">reportPeriod</span></span>      | <span data-ttu-id="c3e43-122">String</span><span class="sxs-lookup"><span data-stu-id="c3e43-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3e43-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3e43-123">JSON representation</span></span>

<span data-ttu-id="c3e43-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3e43-124">The following is a JSON representation of the resource.</span></span>

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
