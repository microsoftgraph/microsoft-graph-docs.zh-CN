---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 79ce924fff5d1ce9ca861c3d48589a0ecad149dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939166"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="343af-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="343af-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="343af-104">属性</span><span class="sxs-lookup"><span data-stu-id="343af-104">Properties</span></span>

| <span data-ttu-id="343af-105">属性</span><span class="sxs-lookup"><span data-stu-id="343af-105">Property</span></span>           | <span data-ttu-id="343af-106">类型</span><span class="sxs-lookup"><span data-stu-id="343af-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="343af-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="343af-107">reportRefreshDate</span></span>  | <span data-ttu-id="343af-108">日期</span><span class="sxs-lookup"><span data-stu-id="343af-108">Date</span></span>    |
| <span data-ttu-id="343af-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="343af-109">groupDisplayName</span></span>   | <span data-ttu-id="343af-110">字符串</span><span class="sxs-lookup"><span data-stu-id="343af-110">String</span></span>  |
| <span data-ttu-id="343af-111">被</span><span class="sxs-lookup"><span data-stu-id="343af-111">isDeleted</span></span>          | <span data-ttu-id="343af-112">布尔</span><span class="sxs-lookup"><span data-stu-id="343af-112">Boolean</span></span> |
| <span data-ttu-id="343af-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="343af-113">ownerPrincipalName</span></span> | <span data-ttu-id="343af-114">字符串</span><span class="sxs-lookup"><span data-stu-id="343af-114">String</span></span>  |
| <span data-ttu-id="343af-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="343af-115">lastActivityDate</span></span>   | <span data-ttu-id="343af-116">日期</span><span class="sxs-lookup"><span data-stu-id="343af-116">Date</span></span>    |
| <span data-ttu-id="343af-117">groupType</span><span class="sxs-lookup"><span data-stu-id="343af-117">groupType</span></span>          | <span data-ttu-id="343af-118">字符串</span><span class="sxs-lookup"><span data-stu-id="343af-118">String</span></span>  |
| <span data-ttu-id="343af-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="343af-119">office365Connected</span></span> | <span data-ttu-id="343af-120">布尔</span><span class="sxs-lookup"><span data-stu-id="343af-120">Boolean</span></span> |
| <span data-ttu-id="343af-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="343af-121">memberCount</span></span>        | <span data-ttu-id="343af-122">Int64</span><span class="sxs-lookup"><span data-stu-id="343af-122">Int64</span></span>   |
| <span data-ttu-id="343af-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="343af-123">postedCount</span></span>        | <span data-ttu-id="343af-124">Int64</span><span class="sxs-lookup"><span data-stu-id="343af-124">Int64</span></span>   |
| <span data-ttu-id="343af-125">readCount</span><span class="sxs-lookup"><span data-stu-id="343af-125">readCount</span></span>          | <span data-ttu-id="343af-126">Int64</span><span class="sxs-lookup"><span data-stu-id="343af-126">Int64</span></span>   |
| <span data-ttu-id="343af-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="343af-127">likedCount</span></span>         | <span data-ttu-id="343af-128">Int64</span><span class="sxs-lookup"><span data-stu-id="343af-128">Int64</span></span>   |
| <span data-ttu-id="343af-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="343af-129">reportPeriod</span></span>       | <span data-ttu-id="343af-130">String</span><span class="sxs-lookup"><span data-stu-id="343af-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="343af-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="343af-131">JSON representation</span></span>

<span data-ttu-id="343af-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="343af-132">The following is a JSON representation of the resource.</span></span>

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
