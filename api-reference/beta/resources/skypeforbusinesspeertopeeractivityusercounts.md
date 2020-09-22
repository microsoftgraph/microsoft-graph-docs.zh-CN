---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 4218caf632c553735c6139bbcf7cd46f64144915
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087500"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="e0e88-103">skypeForBusinessPeerToPeerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0e88-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

<span data-ttu-id="e0e88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0e88-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e0e88-105">属性</span><span class="sxs-lookup"><span data-stu-id="e0e88-105">Properties</span></span>

| <span data-ttu-id="e0e88-106">属性</span><span class="sxs-lookup"><span data-stu-id="e0e88-106">Property</span></span>          | <span data-ttu-id="e0e88-107">类型</span><span class="sxs-lookup"><span data-stu-id="e0e88-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e0e88-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="e0e88-108">im</span></span>                | <span data-ttu-id="e0e88-109">Int64</span><span class="sxs-lookup"><span data-stu-id="e0e88-109">Int64</span></span>  |
| <span data-ttu-id="e0e88-110">audio</span><span class="sxs-lookup"><span data-stu-id="e0e88-110">audio</span></span>             | <span data-ttu-id="e0e88-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e0e88-111">Int64</span></span>  |
| <span data-ttu-id="e0e88-112">video</span><span class="sxs-lookup"><span data-stu-id="e0e88-112">video</span></span>             | <span data-ttu-id="e0e88-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e0e88-113">Int64</span></span>  |
| <span data-ttu-id="e0e88-114">appSharing</span><span class="sxs-lookup"><span data-stu-id="e0e88-114">appSharing</span></span>        | <span data-ttu-id="e0e88-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e0e88-115">Int64</span></span>  |
| <span data-ttu-id="e0e88-116">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="e0e88-116">fileTransfer</span></span>      | <span data-ttu-id="e0e88-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e0e88-117">Int64</span></span>  |
| <span data-ttu-id="e0e88-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e0e88-118">reportRefreshDate</span></span> | <span data-ttu-id="e0e88-119">日期</span><span class="sxs-lookup"><span data-stu-id="e0e88-119">Date</span></span>   |
| <span data-ttu-id="e0e88-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="e0e88-120">reportDate</span></span>        | <span data-ttu-id="e0e88-121">日期</span><span class="sxs-lookup"><span data-stu-id="e0e88-121">Date</span></span>   |
| <span data-ttu-id="e0e88-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e0e88-122">reportPeriod</span></span>      | <span data-ttu-id="e0e88-123">字符串</span><span class="sxs-lookup"><span data-stu-id="e0e88-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e0e88-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0e88-124">JSON representation</span></span>

<span data-ttu-id="e0e88-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0e88-125">The following is a JSON representation of the resource.</span></span>

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


