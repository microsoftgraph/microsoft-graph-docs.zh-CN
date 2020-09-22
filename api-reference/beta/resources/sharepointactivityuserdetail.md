---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 7394e2fab0604286e8066b64e86f413f421472cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997793"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="385f9-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="385f9-103">sharePointActivityUserDetail resource type</span></span>

<span data-ttu-id="385f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="385f9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="385f9-105">属性</span><span class="sxs-lookup"><span data-stu-id="385f9-105">Properties</span></span>

| <span data-ttu-id="385f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="385f9-106">Property</span></span>                  | <span data-ttu-id="385f9-107">类型</span><span class="sxs-lookup"><span data-stu-id="385f9-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="385f9-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="385f9-108">reportRefreshDate</span></span>         | <span data-ttu-id="385f9-109">日期</span><span class="sxs-lookup"><span data-stu-id="385f9-109">Date</span></span>              |
| <span data-ttu-id="385f9-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="385f9-110">userPrincipalName</span></span>         | <span data-ttu-id="385f9-111">String</span><span class="sxs-lookup"><span data-stu-id="385f9-111">String</span></span>            |
| <span data-ttu-id="385f9-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="385f9-112">isDeleted</span></span>                 | <span data-ttu-id="385f9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="385f9-113">Boolean</span></span>           |
| <span data-ttu-id="385f9-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="385f9-114">deletedDate</span></span>               | <span data-ttu-id="385f9-115">日期</span><span class="sxs-lookup"><span data-stu-id="385f9-115">Date</span></span>              |
| <span data-ttu-id="385f9-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="385f9-116">lastActivityDate</span></span>          | <span data-ttu-id="385f9-117">日期</span><span class="sxs-lookup"><span data-stu-id="385f9-117">Date</span></span>              |
| <span data-ttu-id="385f9-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="385f9-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="385f9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="385f9-119">Int64</span></span>             |
| <span data-ttu-id="385f9-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="385f9-120">syncedFileCount</span></span>           | <span data-ttu-id="385f9-121">Int64</span><span class="sxs-lookup"><span data-stu-id="385f9-121">Int64</span></span>             |
| <span data-ttu-id="385f9-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="385f9-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="385f9-123">Int64</span><span class="sxs-lookup"><span data-stu-id="385f9-123">Int64</span></span>             |
| <span data-ttu-id="385f9-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="385f9-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="385f9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="385f9-125">Int64</span></span>             |
| <span data-ttu-id="385f9-126">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="385f9-126">visitedPageCount</span></span>          | <span data-ttu-id="385f9-127">Int64</span><span class="sxs-lookup"><span data-stu-id="385f9-127">Int64</span></span>             |
| <span data-ttu-id="385f9-128">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="385f9-128">assignedProducts</span></span>          | <span data-ttu-id="385f9-129">String collection</span><span class="sxs-lookup"><span data-stu-id="385f9-129">String collection</span></span> |
| <span data-ttu-id="385f9-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="385f9-130">reportPeriod</span></span>              | <span data-ttu-id="385f9-131">String</span><span class="sxs-lookup"><span data-stu-id="385f9-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="385f9-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="385f9-132">JSON representation</span></span>

<span data-ttu-id="385f9-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="385f9-133">The following is a JSON representation of the resource.</span></span>

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


