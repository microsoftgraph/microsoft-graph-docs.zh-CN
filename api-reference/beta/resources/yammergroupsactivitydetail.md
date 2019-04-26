---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551419"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="fc8f4-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc8f4-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fc8f4-104">属性</span><span class="sxs-lookup"><span data-stu-id="fc8f4-104">Properties</span></span>

| <span data-ttu-id="fc8f4-105">属性</span><span class="sxs-lookup"><span data-stu-id="fc8f4-105">Property</span></span>           | <span data-ttu-id="fc8f4-106">类型</span><span class="sxs-lookup"><span data-stu-id="fc8f4-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="fc8f4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fc8f4-107">reportRefreshDate</span></span>  | <span data-ttu-id="fc8f4-108">Date</span><span class="sxs-lookup"><span data-stu-id="fc8f4-108">Date</span></span>    |
| <span data-ttu-id="fc8f4-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="fc8f4-109">groupDisplayName</span></span>   | <span data-ttu-id="fc8f4-110">String</span><span class="sxs-lookup"><span data-stu-id="fc8f4-110">String</span></span>  |
| <span data-ttu-id="fc8f4-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="fc8f4-111">isDeleted</span></span>          | <span data-ttu-id="fc8f4-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="fc8f4-112">Boolean</span></span> |
| <span data-ttu-id="fc8f4-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fc8f4-113">ownerPrincipalName</span></span> | <span data-ttu-id="fc8f4-114">String</span><span class="sxs-lookup"><span data-stu-id="fc8f4-114">String</span></span>  |
| <span data-ttu-id="fc8f4-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="fc8f4-115">lastActivityDate</span></span>   | <span data-ttu-id="fc8f4-116">Date</span><span class="sxs-lookup"><span data-stu-id="fc8f4-116">Date</span></span>    |
| <span data-ttu-id="fc8f4-117">groupType</span><span class="sxs-lookup"><span data-stu-id="fc8f4-117">groupType</span></span>          | <span data-ttu-id="fc8f4-118">String</span><span class="sxs-lookup"><span data-stu-id="fc8f4-118">String</span></span>  |
| <span data-ttu-id="fc8f4-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="fc8f4-119">office365Connected</span></span> | <span data-ttu-id="fc8f4-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="fc8f4-120">Boolean</span></span> |
| <span data-ttu-id="fc8f4-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="fc8f4-121">memberCount</span></span>        | <span data-ttu-id="fc8f4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fc8f4-122">Int64</span></span>   |
| <span data-ttu-id="fc8f4-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="fc8f4-123">postedCount</span></span>        | <span data-ttu-id="fc8f4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="fc8f4-124">Int64</span></span>   |
| <span data-ttu-id="fc8f4-125">readCount</span><span class="sxs-lookup"><span data-stu-id="fc8f4-125">readCount</span></span>          | <span data-ttu-id="fc8f4-126">Int64</span><span class="sxs-lookup"><span data-stu-id="fc8f4-126">Int64</span></span>   |
| <span data-ttu-id="fc8f4-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="fc8f4-127">likedCount</span></span>         | <span data-ttu-id="fc8f4-128">Int64</span><span class="sxs-lookup"><span data-stu-id="fc8f4-128">Int64</span></span>   |
| <span data-ttu-id="fc8f4-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fc8f4-129">reportPeriod</span></span>       | <span data-ttu-id="fc8f4-130">String</span><span class="sxs-lookup"><span data-stu-id="fc8f4-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="fc8f4-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc8f4-131">JSON representation</span></span>

<span data-ttu-id="fc8f4-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc8f4-132">The following is a JSON representation of the resource.</span></span>

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
