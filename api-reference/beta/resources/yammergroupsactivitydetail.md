---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573261"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="e79da-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e79da-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e79da-104">属性</span><span class="sxs-lookup"><span data-stu-id="e79da-104">Properties</span></span>

| <span data-ttu-id="e79da-105">属性</span><span class="sxs-lookup"><span data-stu-id="e79da-105">Property</span></span>           | <span data-ttu-id="e79da-106">类型</span><span class="sxs-lookup"><span data-stu-id="e79da-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="e79da-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e79da-107">reportRefreshDate</span></span>  | <span data-ttu-id="e79da-108">Date</span><span class="sxs-lookup"><span data-stu-id="e79da-108">Date</span></span>    |
| <span data-ttu-id="e79da-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="e79da-109">groupDisplayName</span></span>   | <span data-ttu-id="e79da-110">String</span><span class="sxs-lookup"><span data-stu-id="e79da-110">String</span></span>  |
| <span data-ttu-id="e79da-111">被</span><span class="sxs-lookup"><span data-stu-id="e79da-111">isDeleted</span></span>          | <span data-ttu-id="e79da-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="e79da-112">Boolean</span></span> |
| <span data-ttu-id="e79da-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e79da-113">ownerPrincipalName</span></span> | <span data-ttu-id="e79da-114">String</span><span class="sxs-lookup"><span data-stu-id="e79da-114">String</span></span>  |
| <span data-ttu-id="e79da-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e79da-115">lastActivityDate</span></span>   | <span data-ttu-id="e79da-116">Date</span><span class="sxs-lookup"><span data-stu-id="e79da-116">Date</span></span>    |
| <span data-ttu-id="e79da-117">groupType</span><span class="sxs-lookup"><span data-stu-id="e79da-117">groupType</span></span>          | <span data-ttu-id="e79da-118">String</span><span class="sxs-lookup"><span data-stu-id="e79da-118">String</span></span>  |
| <span data-ttu-id="e79da-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="e79da-119">office365Connected</span></span> | <span data-ttu-id="e79da-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="e79da-120">Boolean</span></span> |
| <span data-ttu-id="e79da-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="e79da-121">memberCount</span></span>        | <span data-ttu-id="e79da-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e79da-122">Int64</span></span>   |
| <span data-ttu-id="e79da-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="e79da-123">postedCount</span></span>        | <span data-ttu-id="e79da-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e79da-124">Int64</span></span>   |
| <span data-ttu-id="e79da-125">readCount</span><span class="sxs-lookup"><span data-stu-id="e79da-125">readCount</span></span>          | <span data-ttu-id="e79da-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e79da-126">Int64</span></span>   |
| <span data-ttu-id="e79da-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="e79da-127">likedCount</span></span>         | <span data-ttu-id="e79da-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e79da-128">Int64</span></span>   |
| <span data-ttu-id="e79da-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e79da-129">reportPeriod</span></span>       | <span data-ttu-id="e79da-130">String</span><span class="sxs-lookup"><span data-stu-id="e79da-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e79da-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e79da-131">JSON representation</span></span>

<span data-ttu-id="e79da-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e79da-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
