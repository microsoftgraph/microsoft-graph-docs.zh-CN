---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9363bd711900cc6211e995c112581d3a91e08a04
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518985"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="36748-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="36748-103">yammerGroupsActivityDetail resource type</span></span>

<span data-ttu-id="36748-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="36748-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="36748-105">属性</span><span class="sxs-lookup"><span data-stu-id="36748-105">Properties</span></span>

| <span data-ttu-id="36748-106">属性</span><span class="sxs-lookup"><span data-stu-id="36748-106">Property</span></span>           | <span data-ttu-id="36748-107">类型</span><span class="sxs-lookup"><span data-stu-id="36748-107">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="36748-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="36748-108">reportRefreshDate</span></span>  | <span data-ttu-id="36748-109">日期</span><span class="sxs-lookup"><span data-stu-id="36748-109">Date</span></span>    |
| <span data-ttu-id="36748-110">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="36748-110">groupDisplayName</span></span>   | <span data-ttu-id="36748-111">String</span><span class="sxs-lookup"><span data-stu-id="36748-111">String</span></span>  |
| <span data-ttu-id="36748-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="36748-112">isDeleted</span></span>          | <span data-ttu-id="36748-113">布尔</span><span class="sxs-lookup"><span data-stu-id="36748-113">Boolean</span></span> |
| <span data-ttu-id="36748-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="36748-114">ownerPrincipalName</span></span> | <span data-ttu-id="36748-115">String</span><span class="sxs-lookup"><span data-stu-id="36748-115">String</span></span>  |
| <span data-ttu-id="36748-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="36748-116">lastActivityDate</span></span>   | <span data-ttu-id="36748-117">日期</span><span class="sxs-lookup"><span data-stu-id="36748-117">Date</span></span>    |
| <span data-ttu-id="36748-118">groupType</span><span class="sxs-lookup"><span data-stu-id="36748-118">groupType</span></span>          | <span data-ttu-id="36748-119">String</span><span class="sxs-lookup"><span data-stu-id="36748-119">String</span></span>  |
| <span data-ttu-id="36748-120">office365Connected</span><span class="sxs-lookup"><span data-stu-id="36748-120">office365Connected</span></span> | <span data-ttu-id="36748-121">布尔</span><span class="sxs-lookup"><span data-stu-id="36748-121">Boolean</span></span> |
| <span data-ttu-id="36748-122">memberCount</span><span class="sxs-lookup"><span data-stu-id="36748-122">memberCount</span></span>        | <span data-ttu-id="36748-123">Int64</span><span class="sxs-lookup"><span data-stu-id="36748-123">Int64</span></span>   |
| <span data-ttu-id="36748-124">postedCount</span><span class="sxs-lookup"><span data-stu-id="36748-124">postedCount</span></span>        | <span data-ttu-id="36748-125">Int64</span><span class="sxs-lookup"><span data-stu-id="36748-125">Int64</span></span>   |
| <span data-ttu-id="36748-126">readCount</span><span class="sxs-lookup"><span data-stu-id="36748-126">readCount</span></span>          | <span data-ttu-id="36748-127">Int64</span><span class="sxs-lookup"><span data-stu-id="36748-127">Int64</span></span>   |
| <span data-ttu-id="36748-128">likedCount</span><span class="sxs-lookup"><span data-stu-id="36748-128">likedCount</span></span>         | <span data-ttu-id="36748-129">Int64</span><span class="sxs-lookup"><span data-stu-id="36748-129">Int64</span></span>   |
| <span data-ttu-id="36748-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="36748-130">reportPeriod</span></span>       | <span data-ttu-id="36748-131">String</span><span class="sxs-lookup"><span data-stu-id="36748-131">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="36748-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36748-132">JSON representation</span></span>

<span data-ttu-id="36748-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36748-133">The following is a JSON representation of the resource.</span></span>

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
