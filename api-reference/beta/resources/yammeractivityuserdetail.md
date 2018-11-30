---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: a1ca33efe8327b1c1e52de25714df9c0bd45ee05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047464"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="9d4e4-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d4e4-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9d4e4-104">属性</span><span class="sxs-lookup"><span data-stu-id="9d4e4-104">Properties</span></span>

| <span data-ttu-id="9d4e4-105">属性</span><span class="sxs-lookup"><span data-stu-id="9d4e4-105">Property</span></span>          | <span data-ttu-id="9d4e4-106">类型</span><span class="sxs-lookup"><span data-stu-id="9d4e4-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="9d4e4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9d4e4-107">reportRefreshDate</span></span> | <span data-ttu-id="9d4e4-108">日期</span><span class="sxs-lookup"><span data-stu-id="9d4e4-108">Date</span></span>              |
| <span data-ttu-id="9d4e4-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9d4e4-109">userPrincipalName</span></span> | <span data-ttu-id="9d4e4-110">字符串</span><span class="sxs-lookup"><span data-stu-id="9d4e4-110">String</span></span>            |
| <span data-ttu-id="9d4e4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9d4e4-111">displayName</span></span>       | <span data-ttu-id="9d4e4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9d4e4-112">String</span></span>            |
| <span data-ttu-id="9d4e4-113">userState</span><span class="sxs-lookup"><span data-stu-id="9d4e4-113">userState</span></span>         | <span data-ttu-id="9d4e4-114">字符串</span><span class="sxs-lookup"><span data-stu-id="9d4e4-114">String</span></span>            |
| <span data-ttu-id="9d4e4-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="9d4e4-115">stateChangeDate</span></span>   | <span data-ttu-id="9d4e4-116">日期</span><span class="sxs-lookup"><span data-stu-id="9d4e4-116">Date</span></span>              |
| <span data-ttu-id="9d4e4-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="9d4e4-117">lastActivityDate</span></span>  | <span data-ttu-id="9d4e4-118">日期</span><span class="sxs-lookup"><span data-stu-id="9d4e4-118">Date</span></span>              |
| <span data-ttu-id="9d4e4-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="9d4e4-119">postedCount</span></span>       | <span data-ttu-id="9d4e4-120">Int64</span><span class="sxs-lookup"><span data-stu-id="9d4e4-120">Int64</span></span>             |
| <span data-ttu-id="9d4e4-121">readCount</span><span class="sxs-lookup"><span data-stu-id="9d4e4-121">readCount</span></span>         | <span data-ttu-id="9d4e4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9d4e4-122">Int64</span></span>             |
| <span data-ttu-id="9d4e4-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="9d4e4-123">likedCount</span></span>        | <span data-ttu-id="9d4e4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="9d4e4-124">Int64</span></span>             |
| <span data-ttu-id="9d4e4-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="9d4e4-125">assignedProducts</span></span>  | <span data-ttu-id="9d4e4-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="9d4e4-126">String collection</span></span> |
| <span data-ttu-id="9d4e4-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9d4e4-127">reportPeriod</span></span>      | <span data-ttu-id="9d4e4-128">String</span><span class="sxs-lookup"><span data-stu-id="9d4e4-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="9d4e4-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d4e4-129">JSON representation</span></span>

<span data-ttu-id="9d4e4-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d4e4-130">The following is a JSON representation of the resource.</span></span>

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
