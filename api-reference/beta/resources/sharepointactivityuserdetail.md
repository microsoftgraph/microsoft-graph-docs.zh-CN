---
title: sharePointActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 20b99e3c6431d945200db868cc02302600e0e76c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807113"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="c750b-103">sharePointActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c750b-103">sharePointActivityUserDetail resource type</span></span>

<span data-ttu-id="c750b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c750b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c750b-105">属性</span><span class="sxs-lookup"><span data-stu-id="c750b-105">Properties</span></span>

| <span data-ttu-id="c750b-106">属性</span><span class="sxs-lookup"><span data-stu-id="c750b-106">Property</span></span>                  | <span data-ttu-id="c750b-107">类型</span><span class="sxs-lookup"><span data-stu-id="c750b-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="c750b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c750b-108">reportRefreshDate</span></span>         | <span data-ttu-id="c750b-109">日期</span><span class="sxs-lookup"><span data-stu-id="c750b-109">Date</span></span>              |
| <span data-ttu-id="c750b-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c750b-110">userPrincipalName</span></span>         | <span data-ttu-id="c750b-111">String</span><span class="sxs-lookup"><span data-stu-id="c750b-111">String</span></span>            |
| <span data-ttu-id="c750b-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c750b-112">isDeleted</span></span>                 | <span data-ttu-id="c750b-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="c750b-113">Boolean</span></span>           |
| <span data-ttu-id="c750b-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c750b-114">deletedDate</span></span>               | <span data-ttu-id="c750b-115">日期</span><span class="sxs-lookup"><span data-stu-id="c750b-115">Date</span></span>              |
| <span data-ttu-id="c750b-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c750b-116">lastActivityDate</span></span>          | <span data-ttu-id="c750b-117">日期</span><span class="sxs-lookup"><span data-stu-id="c750b-117">Date</span></span>              |
| <span data-ttu-id="c750b-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="c750b-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="c750b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c750b-119">Int64</span></span>             |
| <span data-ttu-id="c750b-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="c750b-120">syncedFileCount</span></span>           | <span data-ttu-id="c750b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c750b-121">Int64</span></span>             |
| <span data-ttu-id="c750b-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c750b-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="c750b-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c750b-123">Int64</span></span>             |
| <span data-ttu-id="c750b-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c750b-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="c750b-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c750b-125">Int64</span></span>             |
| <span data-ttu-id="c750b-126">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="c750b-126">visitedPageCount</span></span>          | <span data-ttu-id="c750b-127">Int64</span><span class="sxs-lookup"><span data-stu-id="c750b-127">Int64</span></span>             |
| <span data-ttu-id="c750b-128">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c750b-128">assignedProducts</span></span>          | <span data-ttu-id="c750b-129">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c750b-129">String collection</span></span> |
| <span data-ttu-id="c750b-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c750b-130">reportPeriod</span></span>              | <span data-ttu-id="c750b-131">String</span><span class="sxs-lookup"><span data-stu-id="c750b-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c750b-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c750b-132">JSON representation</span></span>

<span data-ttu-id="c750b-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c750b-133">The following is a JSON representation of the resource.</span></span>

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
