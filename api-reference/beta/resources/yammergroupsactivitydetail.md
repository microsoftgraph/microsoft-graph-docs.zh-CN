---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 9a4bb00aecb2ae1d14b68a5388e0dedc7c41b1cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042442"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="962f2-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="962f2-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="962f2-104">属性</span><span class="sxs-lookup"><span data-stu-id="962f2-104">Properties</span></span>

| <span data-ttu-id="962f2-105">属性</span><span class="sxs-lookup"><span data-stu-id="962f2-105">Property</span></span>           | <span data-ttu-id="962f2-106">类型</span><span class="sxs-lookup"><span data-stu-id="962f2-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="962f2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="962f2-107">reportRefreshDate</span></span>  | <span data-ttu-id="962f2-108">日期</span><span class="sxs-lookup"><span data-stu-id="962f2-108">Date</span></span>    |
| <span data-ttu-id="962f2-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="962f2-109">groupDisplayName</span></span>   | <span data-ttu-id="962f2-110">字符串</span><span class="sxs-lookup"><span data-stu-id="962f2-110">String</span></span>  |
| <span data-ttu-id="962f2-111">被</span><span class="sxs-lookup"><span data-stu-id="962f2-111">isDeleted</span></span>          | <span data-ttu-id="962f2-112">布尔</span><span class="sxs-lookup"><span data-stu-id="962f2-112">Boolean</span></span> |
| <span data-ttu-id="962f2-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="962f2-113">ownerPrincipalName</span></span> | <span data-ttu-id="962f2-114">字符串</span><span class="sxs-lookup"><span data-stu-id="962f2-114">String</span></span>  |
| <span data-ttu-id="962f2-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="962f2-115">lastActivityDate</span></span>   | <span data-ttu-id="962f2-116">日期</span><span class="sxs-lookup"><span data-stu-id="962f2-116">Date</span></span>    |
| <span data-ttu-id="962f2-117">groupType</span><span class="sxs-lookup"><span data-stu-id="962f2-117">groupType</span></span>          | <span data-ttu-id="962f2-118">字符串</span><span class="sxs-lookup"><span data-stu-id="962f2-118">String</span></span>  |
| <span data-ttu-id="962f2-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="962f2-119">office365Connected</span></span> | <span data-ttu-id="962f2-120">布尔</span><span class="sxs-lookup"><span data-stu-id="962f2-120">Boolean</span></span> |
| <span data-ttu-id="962f2-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="962f2-121">memberCount</span></span>        | <span data-ttu-id="962f2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="962f2-122">Int64</span></span>   |
| <span data-ttu-id="962f2-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="962f2-123">postedCount</span></span>        | <span data-ttu-id="962f2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="962f2-124">Int64</span></span>   |
| <span data-ttu-id="962f2-125">readCount</span><span class="sxs-lookup"><span data-stu-id="962f2-125">readCount</span></span>          | <span data-ttu-id="962f2-126">Int64</span><span class="sxs-lookup"><span data-stu-id="962f2-126">Int64</span></span>   |
| <span data-ttu-id="962f2-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="962f2-127">likedCount</span></span>         | <span data-ttu-id="962f2-128">Int64</span><span class="sxs-lookup"><span data-stu-id="962f2-128">Int64</span></span>   |
| <span data-ttu-id="962f2-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="962f2-129">reportPeriod</span></span>       | <span data-ttu-id="962f2-130">String</span><span class="sxs-lookup"><span data-stu-id="962f2-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="962f2-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="962f2-131">JSON representation</span></span>

<span data-ttu-id="962f2-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="962f2-132">The following is a JSON representation of the resource.</span></span>

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
