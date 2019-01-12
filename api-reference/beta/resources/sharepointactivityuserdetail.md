---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979941"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="52882-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="52882-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="52882-104">属性</span><span class="sxs-lookup"><span data-stu-id="52882-104">Properties</span></span>

| <span data-ttu-id="52882-105">属性</span><span class="sxs-lookup"><span data-stu-id="52882-105">Property</span></span>                  | <span data-ttu-id="52882-106">类型</span><span class="sxs-lookup"><span data-stu-id="52882-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="52882-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="52882-107">reportRefreshDate</span></span>         | <span data-ttu-id="52882-108">日期</span><span class="sxs-lookup"><span data-stu-id="52882-108">Date</span></span>              |
| <span data-ttu-id="52882-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="52882-109">userPrincipalName</span></span>         | <span data-ttu-id="52882-110">字符串</span><span class="sxs-lookup"><span data-stu-id="52882-110">String</span></span>            |
| <span data-ttu-id="52882-111">被</span><span class="sxs-lookup"><span data-stu-id="52882-111">isDeleted</span></span>                 | <span data-ttu-id="52882-112">布尔</span><span class="sxs-lookup"><span data-stu-id="52882-112">Boolean</span></span>           |
| <span data-ttu-id="52882-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="52882-113">deletedDate</span></span>               | <span data-ttu-id="52882-114">日期</span><span class="sxs-lookup"><span data-stu-id="52882-114">Date</span></span>              |
| <span data-ttu-id="52882-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="52882-115">lastActivityDate</span></span>          | <span data-ttu-id="52882-116">日期</span><span class="sxs-lookup"><span data-stu-id="52882-116">Date</span></span>              |
| <span data-ttu-id="52882-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="52882-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="52882-118">Int64</span><span class="sxs-lookup"><span data-stu-id="52882-118">Int64</span></span>             |
| <span data-ttu-id="52882-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="52882-119">syncedFileCount</span></span>           | <span data-ttu-id="52882-120">Int64</span><span class="sxs-lookup"><span data-stu-id="52882-120">Int64</span></span>             |
| <span data-ttu-id="52882-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="52882-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="52882-122">Int64</span><span class="sxs-lookup"><span data-stu-id="52882-122">Int64</span></span>             |
| <span data-ttu-id="52882-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="52882-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="52882-124">Int64</span><span class="sxs-lookup"><span data-stu-id="52882-124">Int64</span></span>             |
| <span data-ttu-id="52882-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="52882-125">visitedPageCount</span></span>          | <span data-ttu-id="52882-126">Int64</span><span class="sxs-lookup"><span data-stu-id="52882-126">Int64</span></span>             |
| <span data-ttu-id="52882-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="52882-127">assignedProducts</span></span>          | <span data-ttu-id="52882-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="52882-128">String collection</span></span> |
| <span data-ttu-id="52882-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="52882-129">reportPeriod</span></span>              | <span data-ttu-id="52882-130">String</span><span class="sxs-lookup"><span data-stu-id="52882-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="52882-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52882-131">JSON representation</span></span>

<span data-ttu-id="52882-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52882-132">The following is a JSON representation of the resource.</span></span>

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
