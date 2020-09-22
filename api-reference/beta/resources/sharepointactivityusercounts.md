---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 7ca7a7dc047fff602cec25813faad14e95e63819
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973657"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="9daf2-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="9daf2-103">sharePointActivityUserCounts resource type</span></span>

<span data-ttu-id="9daf2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9daf2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="9daf2-105">属性</span><span class="sxs-lookup"><span data-stu-id="9daf2-105">Properties</span></span>

| <span data-ttu-id="9daf2-106">属性</span><span class="sxs-lookup"><span data-stu-id="9daf2-106">Property</span></span>          | <span data-ttu-id="9daf2-107">类型</span><span class="sxs-lookup"><span data-stu-id="9daf2-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9daf2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9daf2-108">reportRefreshDate</span></span> | <span data-ttu-id="9daf2-109">日期</span><span class="sxs-lookup"><span data-stu-id="9daf2-109">Date</span></span>   |
| <span data-ttu-id="9daf2-110">visitedPage</span><span class="sxs-lookup"><span data-stu-id="9daf2-110">visitedPage</span></span>       | <span data-ttu-id="9daf2-111">Int64</span><span class="sxs-lookup"><span data-stu-id="9daf2-111">Int64</span></span>  |
| <span data-ttu-id="9daf2-112">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="9daf2-112">viewedOrEdited</span></span>    | <span data-ttu-id="9daf2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="9daf2-113">Int64</span></span>  |
| <span data-ttu-id="9daf2-114">保持</span><span class="sxs-lookup"><span data-stu-id="9daf2-114">synced</span></span>            | <span data-ttu-id="9daf2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9daf2-115">Int64</span></span>  |
| <span data-ttu-id="9daf2-116">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="9daf2-116">sharedInternally</span></span>  | <span data-ttu-id="9daf2-117">Int64</span><span class="sxs-lookup"><span data-stu-id="9daf2-117">Int64</span></span>  |
| <span data-ttu-id="9daf2-118">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="9daf2-118">sharedExternally</span></span>  | <span data-ttu-id="9daf2-119">Int64</span><span class="sxs-lookup"><span data-stu-id="9daf2-119">Int64</span></span>  |
| <span data-ttu-id="9daf2-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="9daf2-120">reportDate</span></span>        | <span data-ttu-id="9daf2-121">日期</span><span class="sxs-lookup"><span data-stu-id="9daf2-121">Date</span></span>   |
| <span data-ttu-id="9daf2-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9daf2-122">reportPeriod</span></span>      | <span data-ttu-id="9daf2-123">String</span><span class="sxs-lookup"><span data-stu-id="9daf2-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9daf2-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9daf2-124">JSON representation</span></span>

<span data-ttu-id="9daf2-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9daf2-125">The following is a JSON representation of the resource.</span></span>

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


