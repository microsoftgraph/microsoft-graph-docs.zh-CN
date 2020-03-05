---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 21690f1fa42da4bfa0e2a9c2df48691f00a9595c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520700"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="a155e-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a155e-103">sharePointActivityUserCounts resource type</span></span>

<span data-ttu-id="a155e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a155e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a155e-105">属性</span><span class="sxs-lookup"><span data-stu-id="a155e-105">Properties</span></span>

| <span data-ttu-id="a155e-106">属性</span><span class="sxs-lookup"><span data-stu-id="a155e-106">Property</span></span>          | <span data-ttu-id="a155e-107">类型</span><span class="sxs-lookup"><span data-stu-id="a155e-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a155e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a155e-108">reportRefreshDate</span></span> | <span data-ttu-id="a155e-109">日期</span><span class="sxs-lookup"><span data-stu-id="a155e-109">Date</span></span>   |
| <span data-ttu-id="a155e-110">visitedPage</span><span class="sxs-lookup"><span data-stu-id="a155e-110">visitedPage</span></span>       | <span data-ttu-id="a155e-111">Int64</span><span class="sxs-lookup"><span data-stu-id="a155e-111">Int64</span></span>  |
| <span data-ttu-id="a155e-112">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="a155e-112">viewedOrEdited</span></span>    | <span data-ttu-id="a155e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a155e-113">Int64</span></span>  |
| <span data-ttu-id="a155e-114">保持</span><span class="sxs-lookup"><span data-stu-id="a155e-114">synced</span></span>            | <span data-ttu-id="a155e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="a155e-115">Int64</span></span>  |
| <span data-ttu-id="a155e-116">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="a155e-116">sharedInternally</span></span>  | <span data-ttu-id="a155e-117">Int64</span><span class="sxs-lookup"><span data-stu-id="a155e-117">Int64</span></span>  |
| <span data-ttu-id="a155e-118">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="a155e-118">sharedExternally</span></span>  | <span data-ttu-id="a155e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="a155e-119">Int64</span></span>  |
| <span data-ttu-id="a155e-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="a155e-120">reportDate</span></span>        | <span data-ttu-id="a155e-121">日期</span><span class="sxs-lookup"><span data-stu-id="a155e-121">Date</span></span>   |
| <span data-ttu-id="a155e-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a155e-122">reportPeriod</span></span>      | <span data-ttu-id="a155e-123">String</span><span class="sxs-lookup"><span data-stu-id="a155e-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a155e-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a155e-124">JSON representation</span></span>

<span data-ttu-id="a155e-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a155e-125">The following is a JSON representation of the resource.</span></span>

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
