---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583947"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="701de-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="701de-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="701de-104">属性</span><span class="sxs-lookup"><span data-stu-id="701de-104">Properties</span></span>

| <span data-ttu-id="701de-105">属性</span><span class="sxs-lookup"><span data-stu-id="701de-105">Property</span></span>          | <span data-ttu-id="701de-106">类型</span><span class="sxs-lookup"><span data-stu-id="701de-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="701de-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="701de-107">reportRefreshDate</span></span> | <span data-ttu-id="701de-108">Date</span><span class="sxs-lookup"><span data-stu-id="701de-108">Date</span></span>   |
| <span data-ttu-id="701de-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="701de-109">visitedPage</span></span>       | <span data-ttu-id="701de-110">Int64</span><span class="sxs-lookup"><span data-stu-id="701de-110">Int64</span></span>  |
| <span data-ttu-id="701de-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="701de-111">viewedOrEdited</span></span>    | <span data-ttu-id="701de-112">Int64</span><span class="sxs-lookup"><span data-stu-id="701de-112">Int64</span></span>  |
| <span data-ttu-id="701de-113">保持</span><span class="sxs-lookup"><span data-stu-id="701de-113">synced</span></span>            | <span data-ttu-id="701de-114">Int64</span><span class="sxs-lookup"><span data-stu-id="701de-114">Int64</span></span>  |
| <span data-ttu-id="701de-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="701de-115">sharedInternally</span></span>  | <span data-ttu-id="701de-116">Int64</span><span class="sxs-lookup"><span data-stu-id="701de-116">Int64</span></span>  |
| <span data-ttu-id="701de-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="701de-117">sharedExternally</span></span>  | <span data-ttu-id="701de-118">Int64</span><span class="sxs-lookup"><span data-stu-id="701de-118">Int64</span></span>  |
| <span data-ttu-id="701de-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="701de-119">reportDate</span></span>        | <span data-ttu-id="701de-120">Date</span><span class="sxs-lookup"><span data-stu-id="701de-120">Date</span></span>   |
| <span data-ttu-id="701de-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="701de-121">reportPeriod</span></span>      | <span data-ttu-id="701de-122">String</span><span class="sxs-lookup"><span data-stu-id="701de-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="701de-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="701de-123">JSON representation</span></span>

<span data-ttu-id="701de-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="701de-124">The following is a JSON representation of the resource.</span></span>

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
