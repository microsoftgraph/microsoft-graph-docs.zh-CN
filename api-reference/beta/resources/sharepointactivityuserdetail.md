---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: d7d030bbfaff939da4be645d8003984e5dde0a7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520693"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="efaa7-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="efaa7-103">sharePointActivityUserDetail resource type</span></span>

<span data-ttu-id="efaa7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="efaa7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="efaa7-105">属性</span><span class="sxs-lookup"><span data-stu-id="efaa7-105">Properties</span></span>

| <span data-ttu-id="efaa7-106">属性</span><span class="sxs-lookup"><span data-stu-id="efaa7-106">Property</span></span>                  | <span data-ttu-id="efaa7-107">类型</span><span class="sxs-lookup"><span data-stu-id="efaa7-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="efaa7-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="efaa7-108">reportRefreshDate</span></span>         | <span data-ttu-id="efaa7-109">日期</span><span class="sxs-lookup"><span data-stu-id="efaa7-109">Date</span></span>              |
| <span data-ttu-id="efaa7-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="efaa7-110">userPrincipalName</span></span>         | <span data-ttu-id="efaa7-111">String</span><span class="sxs-lookup"><span data-stu-id="efaa7-111">String</span></span>            |
| <span data-ttu-id="efaa7-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="efaa7-112">isDeleted</span></span>                 | <span data-ttu-id="efaa7-113">布尔</span><span class="sxs-lookup"><span data-stu-id="efaa7-113">Boolean</span></span>           |
| <span data-ttu-id="efaa7-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="efaa7-114">deletedDate</span></span>               | <span data-ttu-id="efaa7-115">日期</span><span class="sxs-lookup"><span data-stu-id="efaa7-115">Date</span></span>              |
| <span data-ttu-id="efaa7-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="efaa7-116">lastActivityDate</span></span>          | <span data-ttu-id="efaa7-117">日期</span><span class="sxs-lookup"><span data-stu-id="efaa7-117">Date</span></span>              |
| <span data-ttu-id="efaa7-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="efaa7-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="efaa7-119">Int64</span><span class="sxs-lookup"><span data-stu-id="efaa7-119">Int64</span></span>             |
| <span data-ttu-id="efaa7-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="efaa7-120">syncedFileCount</span></span>           | <span data-ttu-id="efaa7-121">Int64</span><span class="sxs-lookup"><span data-stu-id="efaa7-121">Int64</span></span>             |
| <span data-ttu-id="efaa7-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="efaa7-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="efaa7-123">Int64</span><span class="sxs-lookup"><span data-stu-id="efaa7-123">Int64</span></span>             |
| <span data-ttu-id="efaa7-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="efaa7-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="efaa7-125">Int64</span><span class="sxs-lookup"><span data-stu-id="efaa7-125">Int64</span></span>             |
| <span data-ttu-id="efaa7-126">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="efaa7-126">visitedPageCount</span></span>          | <span data-ttu-id="efaa7-127">Int64</span><span class="sxs-lookup"><span data-stu-id="efaa7-127">Int64</span></span>             |
| <span data-ttu-id="efaa7-128">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="efaa7-128">assignedProducts</span></span>          | <span data-ttu-id="efaa7-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="efaa7-129">String collection</span></span> |
| <span data-ttu-id="efaa7-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="efaa7-130">reportPeriod</span></span>              | <span data-ttu-id="efaa7-131">String</span><span class="sxs-lookup"><span data-stu-id="efaa7-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="efaa7-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efaa7-132">JSON representation</span></span>

<span data-ttu-id="efaa7-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efaa7-133">The following is a JSON representation of the resource.</span></span>

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
