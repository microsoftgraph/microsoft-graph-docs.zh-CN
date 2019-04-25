---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583975"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="e73e3-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e73e3-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e73e3-104">属性</span><span class="sxs-lookup"><span data-stu-id="e73e3-104">Properties</span></span>

| <span data-ttu-id="e73e3-105">属性</span><span class="sxs-lookup"><span data-stu-id="e73e3-105">Property</span></span>                  | <span data-ttu-id="e73e3-106">类型</span><span class="sxs-lookup"><span data-stu-id="e73e3-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="e73e3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e73e3-107">reportRefreshDate</span></span>         | <span data-ttu-id="e73e3-108">Date</span><span class="sxs-lookup"><span data-stu-id="e73e3-108">Date</span></span>              |
| <span data-ttu-id="e73e3-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e73e3-109">userPrincipalName</span></span>         | <span data-ttu-id="e73e3-110">String</span><span class="sxs-lookup"><span data-stu-id="e73e3-110">String</span></span>            |
| <span data-ttu-id="e73e3-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e73e3-111">isDeleted</span></span>                 | <span data-ttu-id="e73e3-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73e3-112">Boolean</span></span>           |
| <span data-ttu-id="e73e3-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="e73e3-113">deletedDate</span></span>               | <span data-ttu-id="e73e3-114">Date</span><span class="sxs-lookup"><span data-stu-id="e73e3-114">Date</span></span>              |
| <span data-ttu-id="e73e3-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e73e3-115">lastActivityDate</span></span>          | <span data-ttu-id="e73e3-116">Date</span><span class="sxs-lookup"><span data-stu-id="e73e3-116">Date</span></span>              |
| <span data-ttu-id="e73e3-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="e73e3-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="e73e3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e73e3-118">Int64</span></span>             |
| <span data-ttu-id="e73e3-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="e73e3-119">syncedFileCount</span></span>           | <span data-ttu-id="e73e3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e73e3-120">Int64</span></span>             |
| <span data-ttu-id="e73e3-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="e73e3-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="e73e3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e73e3-122">Int64</span></span>             |
| <span data-ttu-id="e73e3-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="e73e3-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="e73e3-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e73e3-124">Int64</span></span>             |
| <span data-ttu-id="e73e3-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="e73e3-125">visitedPageCount</span></span>          | <span data-ttu-id="e73e3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e73e3-126">Int64</span></span>             |
| <span data-ttu-id="e73e3-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="e73e3-127">assignedProducts</span></span>          | <span data-ttu-id="e73e3-128">String collection</span><span class="sxs-lookup"><span data-stu-id="e73e3-128">String collection</span></span> |
| <span data-ttu-id="e73e3-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e73e3-129">reportPeriod</span></span>              | <span data-ttu-id="e73e3-130">String</span><span class="sxs-lookup"><span data-stu-id="e73e3-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e73e3-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e73e3-131">JSON representation</span></span>

<span data-ttu-id="e73e3-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e73e3-132">The following is a JSON representation of the resource.</span></span>

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
