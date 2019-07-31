---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 3d1c1f1b2bcf919769009bbb65a917c4b9cb84f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008430"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="8f2a0-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f2a0-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8f2a0-104">属性</span><span class="sxs-lookup"><span data-stu-id="8f2a0-104">Properties</span></span>

| <span data-ttu-id="8f2a0-105">属性</span><span class="sxs-lookup"><span data-stu-id="8f2a0-105">Property</span></span>                  | <span data-ttu-id="8f2a0-106">类型</span><span class="sxs-lookup"><span data-stu-id="8f2a0-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="8f2a0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8f2a0-107">reportRefreshDate</span></span>         | <span data-ttu-id="8f2a0-108">日期</span><span class="sxs-lookup"><span data-stu-id="8f2a0-108">Date</span></span>              |
| <span data-ttu-id="8f2a0-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f2a0-109">userPrincipalName</span></span>         | <span data-ttu-id="8f2a0-110">String</span><span class="sxs-lookup"><span data-stu-id="8f2a0-110">String</span></span>            |
| <span data-ttu-id="8f2a0-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8f2a0-111">isDeleted</span></span>                 | <span data-ttu-id="8f2a0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f2a0-112">Boolean</span></span>           |
| <span data-ttu-id="8f2a0-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8f2a0-113">deletedDate</span></span>               | <span data-ttu-id="8f2a0-114">日期</span><span class="sxs-lookup"><span data-stu-id="8f2a0-114">Date</span></span>              |
| <span data-ttu-id="8f2a0-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8f2a0-115">lastActivityDate</span></span>          | <span data-ttu-id="8f2a0-116">日期</span><span class="sxs-lookup"><span data-stu-id="8f2a0-116">Date</span></span>              |
| <span data-ttu-id="8f2a0-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="8f2a0-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="8f2a0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8f2a0-118">Int64</span></span>             |
| <span data-ttu-id="8f2a0-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="8f2a0-119">syncedFileCount</span></span>           | <span data-ttu-id="8f2a0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8f2a0-120">Int64</span></span>             |
| <span data-ttu-id="8f2a0-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="8f2a0-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="8f2a0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8f2a0-122">Int64</span></span>             |
| <span data-ttu-id="8f2a0-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="8f2a0-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="8f2a0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8f2a0-124">Int64</span></span>             |
| <span data-ttu-id="8f2a0-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="8f2a0-125">visitedPageCount</span></span>          | <span data-ttu-id="8f2a0-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8f2a0-126">Int64</span></span>             |
| <span data-ttu-id="8f2a0-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8f2a0-127">assignedProducts</span></span>          | <span data-ttu-id="8f2a0-128">String collection</span><span class="sxs-lookup"><span data-stu-id="8f2a0-128">String collection</span></span> |
| <span data-ttu-id="8f2a0-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8f2a0-129">reportPeriod</span></span>              | <span data-ttu-id="8f2a0-130">String</span><span class="sxs-lookup"><span data-stu-id="8f2a0-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="8f2a0-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f2a0-131">JSON representation</span></span>

<span data-ttu-id="8f2a0-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f2a0-132">The following is a JSON representation of the resource.</span></span>

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
