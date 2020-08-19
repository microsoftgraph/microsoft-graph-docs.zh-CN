---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: f629d8b60179e83515af1e9fa5d86e55e7681f17
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807904"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="e38c2-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e38c2-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="e38c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e38c2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e38c2-105">属性</span><span class="sxs-lookup"><span data-stu-id="e38c2-105">Properties</span></span>

| <span data-ttu-id="e38c2-106">属性</span><span class="sxs-lookup"><span data-stu-id="e38c2-106">Property</span></span>          | <span data-ttu-id="e38c2-107">类型</span><span class="sxs-lookup"><span data-stu-id="e38c2-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e38c2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e38c2-108">reportRefreshDate</span></span> | <span data-ttu-id="e38c2-109">日期</span><span class="sxs-lookup"><span data-stu-id="e38c2-109">Date</span></span>   |
| <span data-ttu-id="e38c2-110">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="e38c2-110">viewedOrEdited</span></span>    | <span data-ttu-id="e38c2-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e38c2-111">Int64</span></span>  |
| <span data-ttu-id="e38c2-112">保持</span><span class="sxs-lookup"><span data-stu-id="e38c2-112">synced</span></span>            | <span data-ttu-id="e38c2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e38c2-113">Int64</span></span>  |
| <span data-ttu-id="e38c2-114">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="e38c2-114">sharedInternally</span></span>  | <span data-ttu-id="e38c2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e38c2-115">Int64</span></span>  |
| <span data-ttu-id="e38c2-116">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="e38c2-116">sharedExternally</span></span>  | <span data-ttu-id="e38c2-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e38c2-117">Int64</span></span>  |
| <span data-ttu-id="e38c2-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="e38c2-118">reportDate</span></span>        | <span data-ttu-id="e38c2-119">日期</span><span class="sxs-lookup"><span data-stu-id="e38c2-119">Date</span></span>   |
| <span data-ttu-id="e38c2-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e38c2-120">reportPeriod</span></span>      | <span data-ttu-id="e38c2-121">String</span><span class="sxs-lookup"><span data-stu-id="e38c2-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e38c2-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e38c2-122">JSON representation</span></span>

<span data-ttu-id="e38c2-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e38c2-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date",
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
