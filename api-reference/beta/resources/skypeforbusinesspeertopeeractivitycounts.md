---
title: skypeForBusinessPeerToPeerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 5d492f22672539613933ea94829495915848030c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063847"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="98d07-103">skypeForBusinessPeerToPeerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="98d07-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

<span data-ttu-id="98d07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d07-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="98d07-105">属性</span><span class="sxs-lookup"><span data-stu-id="98d07-105">Properties</span></span>

| <span data-ttu-id="98d07-106">属性</span><span class="sxs-lookup"><span data-stu-id="98d07-106">Property</span></span>          | <span data-ttu-id="98d07-107">类型</span><span class="sxs-lookup"><span data-stu-id="98d07-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="98d07-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="98d07-108">im</span></span>                | <span data-ttu-id="98d07-109">Int64</span><span class="sxs-lookup"><span data-stu-id="98d07-109">Int64</span></span>  |
| <span data-ttu-id="98d07-110">audio</span><span class="sxs-lookup"><span data-stu-id="98d07-110">audio</span></span>             | <span data-ttu-id="98d07-111">Int64</span><span class="sxs-lookup"><span data-stu-id="98d07-111">Int64</span></span>  |
| <span data-ttu-id="98d07-112">video</span><span class="sxs-lookup"><span data-stu-id="98d07-112">video</span></span>             | <span data-ttu-id="98d07-113">Int64</span><span class="sxs-lookup"><span data-stu-id="98d07-113">Int64</span></span>  |
| <span data-ttu-id="98d07-114">appSharing</span><span class="sxs-lookup"><span data-stu-id="98d07-114">appSharing</span></span>        | <span data-ttu-id="98d07-115">Int64</span><span class="sxs-lookup"><span data-stu-id="98d07-115">Int64</span></span>  |
| <span data-ttu-id="98d07-116">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="98d07-116">fileTransfer</span></span>      | <span data-ttu-id="98d07-117">Int64</span><span class="sxs-lookup"><span data-stu-id="98d07-117">Int64</span></span>  |
| <span data-ttu-id="98d07-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="98d07-118">reportRefreshDate</span></span> | <span data-ttu-id="98d07-119">日期</span><span class="sxs-lookup"><span data-stu-id="98d07-119">Date</span></span>   |
| <span data-ttu-id="98d07-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="98d07-120">reportDate</span></span>        | <span data-ttu-id="98d07-121">日期</span><span class="sxs-lookup"><span data-stu-id="98d07-121">Date</span></span>   |
| <span data-ttu-id="98d07-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="98d07-122">reportPeriod</span></span>      | <span data-ttu-id="98d07-123">String</span><span class="sxs-lookup"><span data-stu-id="98d07-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="98d07-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98d07-124">JSON representation</span></span>

<span data-ttu-id="98d07-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98d07-125">The following is a JSON representation of the resource.</span></span>

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


