---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 922ebf14f59d60a988fe77ee36ce04d9c76befec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519027"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="e1539-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1539-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="e1539-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e1539-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e1539-105">属性</span><span class="sxs-lookup"><span data-stu-id="e1539-105">Properties</span></span>

| <span data-ttu-id="e1539-106">属性</span><span class="sxs-lookup"><span data-stu-id="e1539-106">Property</span></span>          | <span data-ttu-id="e1539-107">类型</span><span class="sxs-lookup"><span data-stu-id="e1539-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="e1539-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e1539-108">reportRefreshDate</span></span> | <span data-ttu-id="e1539-109">日期</span><span class="sxs-lookup"><span data-stu-id="e1539-109">Date</span></span>              |
| <span data-ttu-id="e1539-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1539-110">userPrincipalName</span></span> | <span data-ttu-id="e1539-111">String</span><span class="sxs-lookup"><span data-stu-id="e1539-111">String</span></span>            |
| <span data-ttu-id="e1539-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e1539-112">displayName</span></span>       | <span data-ttu-id="e1539-113">String</span><span class="sxs-lookup"><span data-stu-id="e1539-113">String</span></span>            |
| <span data-ttu-id="e1539-114">userState</span><span class="sxs-lookup"><span data-stu-id="e1539-114">userState</span></span>         | <span data-ttu-id="e1539-115">String</span><span class="sxs-lookup"><span data-stu-id="e1539-115">String</span></span>            |
| <span data-ttu-id="e1539-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="e1539-116">stateChangeDate</span></span>   | <span data-ttu-id="e1539-117">日期</span><span class="sxs-lookup"><span data-stu-id="e1539-117">Date</span></span>              |
| <span data-ttu-id="e1539-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e1539-118">lastActivityDate</span></span>  | <span data-ttu-id="e1539-119">日期</span><span class="sxs-lookup"><span data-stu-id="e1539-119">Date</span></span>              |
| <span data-ttu-id="e1539-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="e1539-120">postedCount</span></span>       | <span data-ttu-id="e1539-121">Int64</span><span class="sxs-lookup"><span data-stu-id="e1539-121">Int64</span></span>             |
| <span data-ttu-id="e1539-122">readCount</span><span class="sxs-lookup"><span data-stu-id="e1539-122">readCount</span></span>         | <span data-ttu-id="e1539-123">Int64</span><span class="sxs-lookup"><span data-stu-id="e1539-123">Int64</span></span>             |
| <span data-ttu-id="e1539-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="e1539-124">likedCount</span></span>        | <span data-ttu-id="e1539-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e1539-125">Int64</span></span>             |
| <span data-ttu-id="e1539-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="e1539-126">assignedProducts</span></span>  | <span data-ttu-id="e1539-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="e1539-127">String collection</span></span> |
| <span data-ttu-id="e1539-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e1539-128">reportPeriod</span></span>      | <span data-ttu-id="e1539-129">String</span><span class="sxs-lookup"><span data-stu-id="e1539-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e1539-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1539-130">JSON representation</span></span>

<span data-ttu-id="e1539-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1539-131">The following is a JSON representation of the resource.</span></span>

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
