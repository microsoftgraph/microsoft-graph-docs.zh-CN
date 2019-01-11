---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: d7869869466dc785b92db23f8b574eb2e77dd786
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816399"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="7d9e2-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d9e2-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7d9e2-104">属性</span><span class="sxs-lookup"><span data-stu-id="7d9e2-104">Properties</span></span>

| <span data-ttu-id="7d9e2-105">属性</span><span class="sxs-lookup"><span data-stu-id="7d9e2-105">Property</span></span>          | <span data-ttu-id="7d9e2-106">类型</span><span class="sxs-lookup"><span data-stu-id="7d9e2-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="7d9e2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7d9e2-107">reportRefreshDate</span></span> | <span data-ttu-id="7d9e2-108">日期</span><span class="sxs-lookup"><span data-stu-id="7d9e2-108">Date</span></span>              |
| <span data-ttu-id="7d9e2-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7d9e2-109">userPrincipalName</span></span> | <span data-ttu-id="7d9e2-110">字符串</span><span class="sxs-lookup"><span data-stu-id="7d9e2-110">String</span></span>            |
| <span data-ttu-id="7d9e2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7d9e2-111">displayName</span></span>       | <span data-ttu-id="7d9e2-112">字符串</span><span class="sxs-lookup"><span data-stu-id="7d9e2-112">String</span></span>            |
| <span data-ttu-id="7d9e2-113">userState</span><span class="sxs-lookup"><span data-stu-id="7d9e2-113">userState</span></span>         | <span data-ttu-id="7d9e2-114">字符串</span><span class="sxs-lookup"><span data-stu-id="7d9e2-114">String</span></span>            |
| <span data-ttu-id="7d9e2-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="7d9e2-115">stateChangeDate</span></span>   | <span data-ttu-id="7d9e2-116">日期</span><span class="sxs-lookup"><span data-stu-id="7d9e2-116">Date</span></span>              |
| <span data-ttu-id="7d9e2-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7d9e2-117">lastActivityDate</span></span>  | <span data-ttu-id="7d9e2-118">日期</span><span class="sxs-lookup"><span data-stu-id="7d9e2-118">Date</span></span>              |
| <span data-ttu-id="7d9e2-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="7d9e2-119">postedCount</span></span>       | <span data-ttu-id="7d9e2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="7d9e2-120">Int64</span></span>             |
| <span data-ttu-id="7d9e2-121">readCount</span><span class="sxs-lookup"><span data-stu-id="7d9e2-121">readCount</span></span>         | <span data-ttu-id="7d9e2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="7d9e2-122">Int64</span></span>             |
| <span data-ttu-id="7d9e2-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="7d9e2-123">likedCount</span></span>        | <span data-ttu-id="7d9e2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="7d9e2-124">Int64</span></span>             |
| <span data-ttu-id="7d9e2-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="7d9e2-125">assignedProducts</span></span>  | <span data-ttu-id="7d9e2-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="7d9e2-126">String collection</span></span> |
| <span data-ttu-id="7d9e2-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7d9e2-127">reportPeriod</span></span>      | <span data-ttu-id="7d9e2-128">String</span><span class="sxs-lookup"><span data-stu-id="7d9e2-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="7d9e2-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d9e2-129">JSON representation</span></span>

<span data-ttu-id="7d9e2-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d9e2-130">The following is a JSON representation of the resource.</span></span>

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
