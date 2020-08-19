---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 70e56c30355620e1cc69f258d777e5040c9387e7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807120"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="0db77-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="0db77-103">sharePointActivityUserCounts resource type</span></span>

<span data-ttu-id="0db77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0db77-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0db77-105">属性</span><span class="sxs-lookup"><span data-stu-id="0db77-105">Properties</span></span>

| <span data-ttu-id="0db77-106">属性</span><span class="sxs-lookup"><span data-stu-id="0db77-106">Property</span></span>          | <span data-ttu-id="0db77-107">类型</span><span class="sxs-lookup"><span data-stu-id="0db77-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0db77-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0db77-108">reportRefreshDate</span></span> | <span data-ttu-id="0db77-109">日期</span><span class="sxs-lookup"><span data-stu-id="0db77-109">Date</span></span>   |
| <span data-ttu-id="0db77-110">visitedPage</span><span class="sxs-lookup"><span data-stu-id="0db77-110">visitedPage</span></span>       | <span data-ttu-id="0db77-111">Int64</span><span class="sxs-lookup"><span data-stu-id="0db77-111">Int64</span></span>  |
| <span data-ttu-id="0db77-112">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="0db77-112">viewedOrEdited</span></span>    | <span data-ttu-id="0db77-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0db77-113">Int64</span></span>  |
| <span data-ttu-id="0db77-114">保持</span><span class="sxs-lookup"><span data-stu-id="0db77-114">synced</span></span>            | <span data-ttu-id="0db77-115">Int64</span><span class="sxs-lookup"><span data-stu-id="0db77-115">Int64</span></span>  |
| <span data-ttu-id="0db77-116">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="0db77-116">sharedInternally</span></span>  | <span data-ttu-id="0db77-117">Int64</span><span class="sxs-lookup"><span data-stu-id="0db77-117">Int64</span></span>  |
| <span data-ttu-id="0db77-118">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="0db77-118">sharedExternally</span></span>  | <span data-ttu-id="0db77-119">Int64</span><span class="sxs-lookup"><span data-stu-id="0db77-119">Int64</span></span>  |
| <span data-ttu-id="0db77-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="0db77-120">reportDate</span></span>        | <span data-ttu-id="0db77-121">日期</span><span class="sxs-lookup"><span data-stu-id="0db77-121">Date</span></span>   |
| <span data-ttu-id="0db77-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0db77-122">reportPeriod</span></span>      | <span data-ttu-id="0db77-123">String</span><span class="sxs-lookup"><span data-stu-id="0db77-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0db77-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0db77-124">JSON representation</span></span>

<span data-ttu-id="0db77-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0db77-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "visitedPage": 1024,
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
