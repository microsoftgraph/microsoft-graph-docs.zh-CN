---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 9e4ac61f2af69b4229c2e9c3df7c653428cc2033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832030"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="7ecf7-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ecf7-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7ecf7-104">属性</span><span class="sxs-lookup"><span data-stu-id="7ecf7-104">Properties</span></span>

| <span data-ttu-id="7ecf7-105">属性</span><span class="sxs-lookup"><span data-stu-id="7ecf7-105">Property</span></span>           | <span data-ttu-id="7ecf7-106">类型</span><span class="sxs-lookup"><span data-stu-id="7ecf7-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="7ecf7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7ecf7-107">reportRefreshDate</span></span>  | <span data-ttu-id="7ecf7-108">日期</span><span class="sxs-lookup"><span data-stu-id="7ecf7-108">Date</span></span>    |
| <span data-ttu-id="7ecf7-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="7ecf7-109">groupDisplayName</span></span>   | <span data-ttu-id="7ecf7-110">字符串</span><span class="sxs-lookup"><span data-stu-id="7ecf7-110">String</span></span>  |
| <span data-ttu-id="7ecf7-111">被</span><span class="sxs-lookup"><span data-stu-id="7ecf7-111">isDeleted</span></span>          | <span data-ttu-id="7ecf7-112">布尔</span><span class="sxs-lookup"><span data-stu-id="7ecf7-112">Boolean</span></span> |
| <span data-ttu-id="7ecf7-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7ecf7-113">ownerPrincipalName</span></span> | <span data-ttu-id="7ecf7-114">字符串</span><span class="sxs-lookup"><span data-stu-id="7ecf7-114">String</span></span>  |
| <span data-ttu-id="7ecf7-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7ecf7-115">lastActivityDate</span></span>   | <span data-ttu-id="7ecf7-116">日期</span><span class="sxs-lookup"><span data-stu-id="7ecf7-116">Date</span></span>    |
| <span data-ttu-id="7ecf7-117">groupType</span><span class="sxs-lookup"><span data-stu-id="7ecf7-117">groupType</span></span>          | <span data-ttu-id="7ecf7-118">字符串</span><span class="sxs-lookup"><span data-stu-id="7ecf7-118">String</span></span>  |
| <span data-ttu-id="7ecf7-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="7ecf7-119">office365Connected</span></span> | <span data-ttu-id="7ecf7-120">布尔</span><span class="sxs-lookup"><span data-stu-id="7ecf7-120">Boolean</span></span> |
| <span data-ttu-id="7ecf7-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="7ecf7-121">memberCount</span></span>        | <span data-ttu-id="7ecf7-122">Int64</span><span class="sxs-lookup"><span data-stu-id="7ecf7-122">Int64</span></span>   |
| <span data-ttu-id="7ecf7-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="7ecf7-123">postedCount</span></span>        | <span data-ttu-id="7ecf7-124">Int64</span><span class="sxs-lookup"><span data-stu-id="7ecf7-124">Int64</span></span>   |
| <span data-ttu-id="7ecf7-125">readCount</span><span class="sxs-lookup"><span data-stu-id="7ecf7-125">readCount</span></span>          | <span data-ttu-id="7ecf7-126">Int64</span><span class="sxs-lookup"><span data-stu-id="7ecf7-126">Int64</span></span>   |
| <span data-ttu-id="7ecf7-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="7ecf7-127">likedCount</span></span>         | <span data-ttu-id="7ecf7-128">Int64</span><span class="sxs-lookup"><span data-stu-id="7ecf7-128">Int64</span></span>   |
| <span data-ttu-id="7ecf7-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7ecf7-129">reportPeriod</span></span>       | <span data-ttu-id="7ecf7-130">String</span><span class="sxs-lookup"><span data-stu-id="7ecf7-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7ecf7-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ecf7-131">JSON representation</span></span>

<span data-ttu-id="7ecf7-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ecf7-132">The following is a JSON representation of the resource.</span></span>

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
