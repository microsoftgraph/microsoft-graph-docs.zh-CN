---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f16eda3f28556a18c47c68d532ace4244edfad19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963750"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="bcc94-103">yammerGroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="bcc94-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bcc94-104">属性</span><span class="sxs-lookup"><span data-stu-id="bcc94-104">Properties</span></span>

| <span data-ttu-id="bcc94-105">属性</span><span class="sxs-lookup"><span data-stu-id="bcc94-105">Property</span></span>           | <span data-ttu-id="bcc94-106">类型</span><span class="sxs-lookup"><span data-stu-id="bcc94-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="bcc94-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bcc94-107">reportRefreshDate</span></span>  | <span data-ttu-id="bcc94-108">日期</span><span class="sxs-lookup"><span data-stu-id="bcc94-108">Date</span></span>    |
| <span data-ttu-id="bcc94-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="bcc94-109">groupDisplayName</span></span>   | <span data-ttu-id="bcc94-110">String</span><span class="sxs-lookup"><span data-stu-id="bcc94-110">String</span></span>  |
| <span data-ttu-id="bcc94-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bcc94-111">isDeleted</span></span>          | <span data-ttu-id="bcc94-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcc94-112">Boolean</span></span> |
| <span data-ttu-id="bcc94-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bcc94-113">ownerPrincipalName</span></span> | <span data-ttu-id="bcc94-114">String</span><span class="sxs-lookup"><span data-stu-id="bcc94-114">String</span></span>  |
| <span data-ttu-id="bcc94-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bcc94-115">lastActivityDate</span></span>   | <span data-ttu-id="bcc94-116">日期</span><span class="sxs-lookup"><span data-stu-id="bcc94-116">Date</span></span>    |
| <span data-ttu-id="bcc94-117">groupType</span><span class="sxs-lookup"><span data-stu-id="bcc94-117">groupType</span></span>          | <span data-ttu-id="bcc94-118">String</span><span class="sxs-lookup"><span data-stu-id="bcc94-118">String</span></span>  |
| <span data-ttu-id="bcc94-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="bcc94-119">office365Connected</span></span> | <span data-ttu-id="bcc94-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcc94-120">Boolean</span></span> |
| <span data-ttu-id="bcc94-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="bcc94-121">memberCount</span></span>        | <span data-ttu-id="bcc94-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc94-122">Int64</span></span>   |
| <span data-ttu-id="bcc94-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="bcc94-123">postedCount</span></span>        | <span data-ttu-id="bcc94-124">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc94-124">Int64</span></span>   |
| <span data-ttu-id="bcc94-125">readCount</span><span class="sxs-lookup"><span data-stu-id="bcc94-125">readCount</span></span>          | <span data-ttu-id="bcc94-126">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc94-126">Int64</span></span>   |
| <span data-ttu-id="bcc94-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="bcc94-127">likedCount</span></span>         | <span data-ttu-id="bcc94-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc94-128">Int64</span></span>   |
| <span data-ttu-id="bcc94-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bcc94-129">reportPeriod</span></span>       | <span data-ttu-id="bcc94-130">String</span><span class="sxs-lookup"><span data-stu-id="bcc94-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="bcc94-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcc94-131">JSON representation</span></span>

<span data-ttu-id="bcc94-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcc94-132">The following is a JSON representation of the resource.</span></span>

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
