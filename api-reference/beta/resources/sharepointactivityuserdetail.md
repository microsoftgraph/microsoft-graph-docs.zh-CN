---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: a5b6de8a4a9b82d9e6d34a2ae289f0c7589798ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042141"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="e47c6-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e47c6-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e47c6-104">属性</span><span class="sxs-lookup"><span data-stu-id="e47c6-104">Properties</span></span>

| <span data-ttu-id="e47c6-105">属性</span><span class="sxs-lookup"><span data-stu-id="e47c6-105">Property</span></span>                  | <span data-ttu-id="e47c6-106">类型</span><span class="sxs-lookup"><span data-stu-id="e47c6-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="e47c6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e47c6-107">reportRefreshDate</span></span>         | <span data-ttu-id="e47c6-108">日期</span><span class="sxs-lookup"><span data-stu-id="e47c6-108">Date</span></span>              |
| <span data-ttu-id="e47c6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e47c6-109">userPrincipalName</span></span>         | <span data-ttu-id="e47c6-110">字符串</span><span class="sxs-lookup"><span data-stu-id="e47c6-110">String</span></span>            |
| <span data-ttu-id="e47c6-111">被</span><span class="sxs-lookup"><span data-stu-id="e47c6-111">isDeleted</span></span>                 | <span data-ttu-id="e47c6-112">布尔</span><span class="sxs-lookup"><span data-stu-id="e47c6-112">Boolean</span></span>           |
| <span data-ttu-id="e47c6-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="e47c6-113">deletedDate</span></span>               | <span data-ttu-id="e47c6-114">日期</span><span class="sxs-lookup"><span data-stu-id="e47c6-114">Date</span></span>              |
| <span data-ttu-id="e47c6-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e47c6-115">lastActivityDate</span></span>          | <span data-ttu-id="e47c6-116">日期</span><span class="sxs-lookup"><span data-stu-id="e47c6-116">Date</span></span>              |
| <span data-ttu-id="e47c6-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="e47c6-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="e47c6-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e47c6-118">Int64</span></span>             |
| <span data-ttu-id="e47c6-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="e47c6-119">syncedFileCount</span></span>           | <span data-ttu-id="e47c6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e47c6-120">Int64</span></span>             |
| <span data-ttu-id="e47c6-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="e47c6-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="e47c6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e47c6-122">Int64</span></span>             |
| <span data-ttu-id="e47c6-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="e47c6-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="e47c6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e47c6-124">Int64</span></span>             |
| <span data-ttu-id="e47c6-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="e47c6-125">visitedPageCount</span></span>          | <span data-ttu-id="e47c6-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e47c6-126">Int64</span></span>             |
| <span data-ttu-id="e47c6-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="e47c6-127">assignedProducts</span></span>          | <span data-ttu-id="e47c6-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="e47c6-128">String collection</span></span> |
| <span data-ttu-id="e47c6-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e47c6-129">reportPeriod</span></span>              | <span data-ttu-id="e47c6-130">String</span><span class="sxs-lookup"><span data-stu-id="e47c6-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e47c6-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e47c6-131">JSON representation</span></span>

<span data-ttu-id="e47c6-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e47c6-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
