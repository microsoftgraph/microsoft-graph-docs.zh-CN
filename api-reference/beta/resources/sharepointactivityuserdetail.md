---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 4503739a7b2e13cade72951ae56ab410f22608b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880694"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="6277b-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="6277b-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6277b-104">属性</span><span class="sxs-lookup"><span data-stu-id="6277b-104">Properties</span></span>

| <span data-ttu-id="6277b-105">属性</span><span class="sxs-lookup"><span data-stu-id="6277b-105">Property</span></span>                  | <span data-ttu-id="6277b-106">类型</span><span class="sxs-lookup"><span data-stu-id="6277b-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="6277b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6277b-107">reportRefreshDate</span></span>         | <span data-ttu-id="6277b-108">日期</span><span class="sxs-lookup"><span data-stu-id="6277b-108">Date</span></span>              |
| <span data-ttu-id="6277b-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6277b-109">userPrincipalName</span></span>         | <span data-ttu-id="6277b-110">字符串</span><span class="sxs-lookup"><span data-stu-id="6277b-110">String</span></span>            |
| <span data-ttu-id="6277b-111">被</span><span class="sxs-lookup"><span data-stu-id="6277b-111">isDeleted</span></span>                 | <span data-ttu-id="6277b-112">布尔</span><span class="sxs-lookup"><span data-stu-id="6277b-112">Boolean</span></span>           |
| <span data-ttu-id="6277b-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6277b-113">deletedDate</span></span>               | <span data-ttu-id="6277b-114">日期</span><span class="sxs-lookup"><span data-stu-id="6277b-114">Date</span></span>              |
| <span data-ttu-id="6277b-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6277b-115">lastActivityDate</span></span>          | <span data-ttu-id="6277b-116">日期</span><span class="sxs-lookup"><span data-stu-id="6277b-116">Date</span></span>              |
| <span data-ttu-id="6277b-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="6277b-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="6277b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6277b-118">Int64</span></span>             |
| <span data-ttu-id="6277b-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="6277b-119">syncedFileCount</span></span>           | <span data-ttu-id="6277b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6277b-120">Int64</span></span>             |
| <span data-ttu-id="6277b-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="6277b-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="6277b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6277b-122">Int64</span></span>             |
| <span data-ttu-id="6277b-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="6277b-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="6277b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6277b-124">Int64</span></span>             |
| <span data-ttu-id="6277b-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="6277b-125">visitedPageCount</span></span>          | <span data-ttu-id="6277b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="6277b-126">Int64</span></span>             |
| <span data-ttu-id="6277b-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="6277b-127">assignedProducts</span></span>          | <span data-ttu-id="6277b-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="6277b-128">String collection</span></span> |
| <span data-ttu-id="6277b-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6277b-129">reportPeriod</span></span>              | <span data-ttu-id="6277b-130">String</span><span class="sxs-lookup"><span data-stu-id="6277b-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="6277b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6277b-131">JSON representation</span></span>

<span data-ttu-id="6277b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6277b-132">The following is a JSON representation of the resource.</span></span>

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
