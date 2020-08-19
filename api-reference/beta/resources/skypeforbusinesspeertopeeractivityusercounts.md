---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 47e5597971c5b1417151ae202bb1e0fade17597a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810970"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="32fb4-103">skypeForBusinessPeerToPeerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="32fb4-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

<span data-ttu-id="32fb4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32fb4-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="32fb4-105">属性</span><span class="sxs-lookup"><span data-stu-id="32fb4-105">Properties</span></span>

| <span data-ttu-id="32fb4-106">属性</span><span class="sxs-lookup"><span data-stu-id="32fb4-106">Property</span></span>          | <span data-ttu-id="32fb4-107">类型</span><span class="sxs-lookup"><span data-stu-id="32fb4-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="32fb4-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="32fb4-108">im</span></span>                | <span data-ttu-id="32fb4-109">Int64</span><span class="sxs-lookup"><span data-stu-id="32fb4-109">Int64</span></span>  |
| <span data-ttu-id="32fb4-110">audio</span><span class="sxs-lookup"><span data-stu-id="32fb4-110">audio</span></span>             | <span data-ttu-id="32fb4-111">Int64</span><span class="sxs-lookup"><span data-stu-id="32fb4-111">Int64</span></span>  |
| <span data-ttu-id="32fb4-112">video</span><span class="sxs-lookup"><span data-stu-id="32fb4-112">video</span></span>             | <span data-ttu-id="32fb4-113">Int64</span><span class="sxs-lookup"><span data-stu-id="32fb4-113">Int64</span></span>  |
| <span data-ttu-id="32fb4-114">appSharing</span><span class="sxs-lookup"><span data-stu-id="32fb4-114">appSharing</span></span>        | <span data-ttu-id="32fb4-115">Int64</span><span class="sxs-lookup"><span data-stu-id="32fb4-115">Int64</span></span>  |
| <span data-ttu-id="32fb4-116">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="32fb4-116">fileTransfer</span></span>      | <span data-ttu-id="32fb4-117">Int64</span><span class="sxs-lookup"><span data-stu-id="32fb4-117">Int64</span></span>  |
| <span data-ttu-id="32fb4-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="32fb4-118">reportRefreshDate</span></span> | <span data-ttu-id="32fb4-119">日期</span><span class="sxs-lookup"><span data-stu-id="32fb4-119">Date</span></span>   |
| <span data-ttu-id="32fb4-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="32fb4-120">reportDate</span></span>        | <span data-ttu-id="32fb4-121">日期</span><span class="sxs-lookup"><span data-stu-id="32fb4-121">Date</span></span>   |
| <span data-ttu-id="32fb4-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="32fb4-122">reportPeriod</span></span>      | <span data-ttu-id="32fb4-123">String</span><span class="sxs-lookup"><span data-stu-id="32fb4-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32fb4-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32fb4-124">JSON representation</span></span>

<span data-ttu-id="32fb4-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32fb4-125">The following is a JSON representation of the resource.</span></span>

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
