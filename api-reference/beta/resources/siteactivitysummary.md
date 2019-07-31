---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1258530aea56f7ec26a2f48274935afc809f2fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965017"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="791f7-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="791f7-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="791f7-104">属性</span><span class="sxs-lookup"><span data-stu-id="791f7-104">Properties</span></span>

| <span data-ttu-id="791f7-105">属性</span><span class="sxs-lookup"><span data-stu-id="791f7-105">Property</span></span>          | <span data-ttu-id="791f7-106">类型</span><span class="sxs-lookup"><span data-stu-id="791f7-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="791f7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="791f7-107">reportRefreshDate</span></span> | <span data-ttu-id="791f7-108">日期</span><span class="sxs-lookup"><span data-stu-id="791f7-108">Date</span></span>   |
| <span data-ttu-id="791f7-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="791f7-109">viewedOrEdited</span></span>    | <span data-ttu-id="791f7-110">Int64</span><span class="sxs-lookup"><span data-stu-id="791f7-110">Int64</span></span>  |
| <span data-ttu-id="791f7-111">保持</span><span class="sxs-lookup"><span data-stu-id="791f7-111">synced</span></span>            | <span data-ttu-id="791f7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="791f7-112">Int64</span></span>  |
| <span data-ttu-id="791f7-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="791f7-113">sharedInternally</span></span>  | <span data-ttu-id="791f7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="791f7-114">Int64</span></span>  |
| <span data-ttu-id="791f7-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="791f7-115">sharedExternally</span></span>  | <span data-ttu-id="791f7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="791f7-116">Int64</span></span>  |
| <span data-ttu-id="791f7-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="791f7-117">reportDate</span></span>        | <span data-ttu-id="791f7-118">日期</span><span class="sxs-lookup"><span data-stu-id="791f7-118">Date</span></span>   |
| <span data-ttu-id="791f7-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="791f7-119">reportPeriod</span></span>      | <span data-ttu-id="791f7-120">String</span><span class="sxs-lookup"><span data-stu-id="791f7-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="791f7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="791f7-121">JSON representation</span></span>

<span data-ttu-id="791f7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="791f7-122">The following is a JSON representation of the resource.</span></span>

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
