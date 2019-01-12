---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957135"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="52177-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="52177-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="52177-104">属性</span><span class="sxs-lookup"><span data-stu-id="52177-104">Properties</span></span>

| <span data-ttu-id="52177-105">属性</span><span class="sxs-lookup"><span data-stu-id="52177-105">Property</span></span>          | <span data-ttu-id="52177-106">类型</span><span class="sxs-lookup"><span data-stu-id="52177-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="52177-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="52177-107">reportRefreshDate</span></span> | <span data-ttu-id="52177-108">日期</span><span class="sxs-lookup"><span data-stu-id="52177-108">Date</span></span>   |
| <span data-ttu-id="52177-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="52177-109">viewedOrEdited</span></span>    | <span data-ttu-id="52177-110">Int64</span><span class="sxs-lookup"><span data-stu-id="52177-110">Int64</span></span>  |
| <span data-ttu-id="52177-111">同步</span><span class="sxs-lookup"><span data-stu-id="52177-111">synced</span></span>            | <span data-ttu-id="52177-112">Int64</span><span class="sxs-lookup"><span data-stu-id="52177-112">Int64</span></span>  |
| <span data-ttu-id="52177-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="52177-113">sharedInternally</span></span>  | <span data-ttu-id="52177-114">Int64</span><span class="sxs-lookup"><span data-stu-id="52177-114">Int64</span></span>  |
| <span data-ttu-id="52177-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="52177-115">sharedExternally</span></span>  | <span data-ttu-id="52177-116">Int64</span><span class="sxs-lookup"><span data-stu-id="52177-116">Int64</span></span>  |
| <span data-ttu-id="52177-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="52177-117">reportDate</span></span>        | <span data-ttu-id="52177-118">日期</span><span class="sxs-lookup"><span data-stu-id="52177-118">Date</span></span>   |
| <span data-ttu-id="52177-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="52177-119">reportPeriod</span></span>      | <span data-ttu-id="52177-120">String</span><span class="sxs-lookup"><span data-stu-id="52177-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52177-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52177-121">JSON representation</span></span>

<span data-ttu-id="52177-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52177-122">The following is a JSON representation of the resource.</span></span>

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
