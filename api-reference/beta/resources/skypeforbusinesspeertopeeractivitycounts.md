---
title: skypeForBusinessPeerToPeerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 6bdcd96a8c6eb3dff29304bf8dc1dd8956d9063d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811040"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="f6840-103">skypeForBusinessPeerToPeerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6840-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

<span data-ttu-id="f6840-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6840-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f6840-105">属性</span><span class="sxs-lookup"><span data-stu-id="f6840-105">Properties</span></span>

| <span data-ttu-id="f6840-106">属性</span><span class="sxs-lookup"><span data-stu-id="f6840-106">Property</span></span>          | <span data-ttu-id="f6840-107">类型</span><span class="sxs-lookup"><span data-stu-id="f6840-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f6840-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="f6840-108">im</span></span>                | <span data-ttu-id="f6840-109">Int64</span><span class="sxs-lookup"><span data-stu-id="f6840-109">Int64</span></span>  |
| <span data-ttu-id="f6840-110">audio</span><span class="sxs-lookup"><span data-stu-id="f6840-110">audio</span></span>             | <span data-ttu-id="f6840-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f6840-111">Int64</span></span>  |
| <span data-ttu-id="f6840-112">video</span><span class="sxs-lookup"><span data-stu-id="f6840-112">video</span></span>             | <span data-ttu-id="f6840-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f6840-113">Int64</span></span>  |
| <span data-ttu-id="f6840-114">appSharing</span><span class="sxs-lookup"><span data-stu-id="f6840-114">appSharing</span></span>        | <span data-ttu-id="f6840-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f6840-115">Int64</span></span>  |
| <span data-ttu-id="f6840-116">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="f6840-116">fileTransfer</span></span>      | <span data-ttu-id="f6840-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f6840-117">Int64</span></span>  |
| <span data-ttu-id="f6840-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f6840-118">reportRefreshDate</span></span> | <span data-ttu-id="f6840-119">日期</span><span class="sxs-lookup"><span data-stu-id="f6840-119">Date</span></span>   |
| <span data-ttu-id="f6840-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="f6840-120">reportDate</span></span>        | <span data-ttu-id="f6840-121">日期</span><span class="sxs-lookup"><span data-stu-id="f6840-121">Date</span></span>   |
| <span data-ttu-id="f6840-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f6840-122">reportPeriod</span></span>      | <span data-ttu-id="f6840-123">String</span><span class="sxs-lookup"><span data-stu-id="f6840-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f6840-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6840-124">JSON representation</span></span>

<span data-ttu-id="f6840-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6840-125">The following is a JSON representation of the resource.</span></span>

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
