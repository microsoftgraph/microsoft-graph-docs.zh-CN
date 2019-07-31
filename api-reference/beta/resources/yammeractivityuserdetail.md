---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 960945d72db1cc347228983b9567968dfcfc52d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963785"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="e0cba-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0cba-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e0cba-104">属性</span><span class="sxs-lookup"><span data-stu-id="e0cba-104">Properties</span></span>

| <span data-ttu-id="e0cba-105">属性</span><span class="sxs-lookup"><span data-stu-id="e0cba-105">Property</span></span>          | <span data-ttu-id="e0cba-106">类型</span><span class="sxs-lookup"><span data-stu-id="e0cba-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="e0cba-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e0cba-107">reportRefreshDate</span></span> | <span data-ttu-id="e0cba-108">日期</span><span class="sxs-lookup"><span data-stu-id="e0cba-108">Date</span></span>              |
| <span data-ttu-id="e0cba-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e0cba-109">userPrincipalName</span></span> | <span data-ttu-id="e0cba-110">String</span><span class="sxs-lookup"><span data-stu-id="e0cba-110">String</span></span>            |
| <span data-ttu-id="e0cba-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e0cba-111">displayName</span></span>       | <span data-ttu-id="e0cba-112">String</span><span class="sxs-lookup"><span data-stu-id="e0cba-112">String</span></span>            |
| <span data-ttu-id="e0cba-113">userState</span><span class="sxs-lookup"><span data-stu-id="e0cba-113">userState</span></span>         | <span data-ttu-id="e0cba-114">String</span><span class="sxs-lookup"><span data-stu-id="e0cba-114">String</span></span>            |
| <span data-ttu-id="e0cba-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="e0cba-115">stateChangeDate</span></span>   | <span data-ttu-id="e0cba-116">日期</span><span class="sxs-lookup"><span data-stu-id="e0cba-116">Date</span></span>              |
| <span data-ttu-id="e0cba-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e0cba-117">lastActivityDate</span></span>  | <span data-ttu-id="e0cba-118">日期</span><span class="sxs-lookup"><span data-stu-id="e0cba-118">Date</span></span>              |
| <span data-ttu-id="e0cba-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="e0cba-119">postedCount</span></span>       | <span data-ttu-id="e0cba-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e0cba-120">Int64</span></span>             |
| <span data-ttu-id="e0cba-121">readCount</span><span class="sxs-lookup"><span data-stu-id="e0cba-121">readCount</span></span>         | <span data-ttu-id="e0cba-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e0cba-122">Int64</span></span>             |
| <span data-ttu-id="e0cba-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="e0cba-123">likedCount</span></span>        | <span data-ttu-id="e0cba-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e0cba-124">Int64</span></span>             |
| <span data-ttu-id="e0cba-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="e0cba-125">assignedProducts</span></span>  | <span data-ttu-id="e0cba-126">String collection</span><span class="sxs-lookup"><span data-stu-id="e0cba-126">String collection</span></span> |
| <span data-ttu-id="e0cba-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e0cba-127">reportPeriod</span></span>      | <span data-ttu-id="e0cba-128">String</span><span class="sxs-lookup"><span data-stu-id="e0cba-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e0cba-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0cba-129">JSON representation</span></span>

<span data-ttu-id="e0cba-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0cba-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
