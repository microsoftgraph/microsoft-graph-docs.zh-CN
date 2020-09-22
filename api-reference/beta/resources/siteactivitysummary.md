---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: ce2d4806dd8c2e8367bf5a9c075fab84e3c17900
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985690"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="9ee22-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ee22-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="9ee22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ee22-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="9ee22-105">属性</span><span class="sxs-lookup"><span data-stu-id="9ee22-105">Properties</span></span>

| <span data-ttu-id="9ee22-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ee22-106">Property</span></span>          | <span data-ttu-id="9ee22-107">类型</span><span class="sxs-lookup"><span data-stu-id="9ee22-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9ee22-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9ee22-108">reportRefreshDate</span></span> | <span data-ttu-id="9ee22-109">日期</span><span class="sxs-lookup"><span data-stu-id="9ee22-109">Date</span></span>   |
| <span data-ttu-id="9ee22-110">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="9ee22-110">viewedOrEdited</span></span>    | <span data-ttu-id="9ee22-111">Int64</span><span class="sxs-lookup"><span data-stu-id="9ee22-111">Int64</span></span>  |
| <span data-ttu-id="9ee22-112">保持</span><span class="sxs-lookup"><span data-stu-id="9ee22-112">synced</span></span>            | <span data-ttu-id="9ee22-113">Int64</span><span class="sxs-lookup"><span data-stu-id="9ee22-113">Int64</span></span>  |
| <span data-ttu-id="9ee22-114">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="9ee22-114">sharedInternally</span></span>  | <span data-ttu-id="9ee22-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9ee22-115">Int64</span></span>  |
| <span data-ttu-id="9ee22-116">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="9ee22-116">sharedExternally</span></span>  | <span data-ttu-id="9ee22-117">Int64</span><span class="sxs-lookup"><span data-stu-id="9ee22-117">Int64</span></span>  |
| <span data-ttu-id="9ee22-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="9ee22-118">reportDate</span></span>        | <span data-ttu-id="9ee22-119">日期</span><span class="sxs-lookup"><span data-stu-id="9ee22-119">Date</span></span>   |
| <span data-ttu-id="9ee22-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9ee22-120">reportPeriod</span></span>      | <span data-ttu-id="9ee22-121">String</span><span class="sxs-lookup"><span data-stu-id="9ee22-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9ee22-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ee22-122">JSON representation</span></span>

<span data-ttu-id="9ee22-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ee22-123">The following is a JSON representation of the resource.</span></span>

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


