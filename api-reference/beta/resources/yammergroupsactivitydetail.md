---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 2188cf1ad583ba66fffb1d7b86009f49fba3f8fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046072"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="ac8ff-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac8ff-103">yammerGroupsActivityDetail resource type</span></span>

<span data-ttu-id="ac8ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac8ff-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ac8ff-105">属性</span><span class="sxs-lookup"><span data-stu-id="ac8ff-105">Properties</span></span>

| <span data-ttu-id="ac8ff-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac8ff-106">Property</span></span>           | <span data-ttu-id="ac8ff-107">类型</span><span class="sxs-lookup"><span data-stu-id="ac8ff-107">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="ac8ff-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ac8ff-108">reportRefreshDate</span></span>  | <span data-ttu-id="ac8ff-109">日期</span><span class="sxs-lookup"><span data-stu-id="ac8ff-109">Date</span></span>    |
| <span data-ttu-id="ac8ff-110">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="ac8ff-110">groupDisplayName</span></span>   | <span data-ttu-id="ac8ff-111">String</span><span class="sxs-lookup"><span data-stu-id="ac8ff-111">String</span></span>  |
| <span data-ttu-id="ac8ff-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ac8ff-112">isDeleted</span></span>          | <span data-ttu-id="ac8ff-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac8ff-113">Boolean</span></span> |
| <span data-ttu-id="ac8ff-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ac8ff-114">ownerPrincipalName</span></span> | <span data-ttu-id="ac8ff-115">String</span><span class="sxs-lookup"><span data-stu-id="ac8ff-115">String</span></span>  |
| <span data-ttu-id="ac8ff-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ac8ff-116">lastActivityDate</span></span>   | <span data-ttu-id="ac8ff-117">日期</span><span class="sxs-lookup"><span data-stu-id="ac8ff-117">Date</span></span>    |
| <span data-ttu-id="ac8ff-118">groupType</span><span class="sxs-lookup"><span data-stu-id="ac8ff-118">groupType</span></span>          | <span data-ttu-id="ac8ff-119">String</span><span class="sxs-lookup"><span data-stu-id="ac8ff-119">String</span></span>  |
| <span data-ttu-id="ac8ff-120">office365Connected</span><span class="sxs-lookup"><span data-stu-id="ac8ff-120">office365Connected</span></span> | <span data-ttu-id="ac8ff-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac8ff-121">Boolean</span></span> |
| <span data-ttu-id="ac8ff-122">memberCount</span><span class="sxs-lookup"><span data-stu-id="ac8ff-122">memberCount</span></span>        | <span data-ttu-id="ac8ff-123">Int64</span><span class="sxs-lookup"><span data-stu-id="ac8ff-123">Int64</span></span>   |
| <span data-ttu-id="ac8ff-124">postedCount</span><span class="sxs-lookup"><span data-stu-id="ac8ff-124">postedCount</span></span>        | <span data-ttu-id="ac8ff-125">Int64</span><span class="sxs-lookup"><span data-stu-id="ac8ff-125">Int64</span></span>   |
| <span data-ttu-id="ac8ff-126">readCount</span><span class="sxs-lookup"><span data-stu-id="ac8ff-126">readCount</span></span>          | <span data-ttu-id="ac8ff-127">Int64</span><span class="sxs-lookup"><span data-stu-id="ac8ff-127">Int64</span></span>   |
| <span data-ttu-id="ac8ff-128">likedCount</span><span class="sxs-lookup"><span data-stu-id="ac8ff-128">likedCount</span></span>         | <span data-ttu-id="ac8ff-129">Int64</span><span class="sxs-lookup"><span data-stu-id="ac8ff-129">Int64</span></span>   |
| <span data-ttu-id="ac8ff-130">networkDisplayName</span><span class="sxs-lookup"><span data-stu-id="ac8ff-130">networkDisplayName</span></span> | <span data-ttu-id="ac8ff-131">String</span><span class="sxs-lookup"><span data-stu-id="ac8ff-131">String</span></span>  |
| <span data-ttu-id="ac8ff-132">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ac8ff-132">reportPeriod</span></span>       | <span data-ttu-id="ac8ff-133">String</span><span class="sxs-lookup"><span data-stu-id="ac8ff-133">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ac8ff-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac8ff-134">JSON representation</span></span>

<span data-ttu-id="ac8ff-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac8ff-135">The following is a JSON representation of the resource.</span></span>

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
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```


