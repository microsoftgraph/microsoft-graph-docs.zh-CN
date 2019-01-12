---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d24e21c9525d49b7af5f8c4efaddd606c20c162b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923031"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="af628-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="af628-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="af628-104">属性</span><span class="sxs-lookup"><span data-stu-id="af628-104">Properties</span></span>

| <span data-ttu-id="af628-105">属性</span><span class="sxs-lookup"><span data-stu-id="af628-105">Property</span></span>          | <span data-ttu-id="af628-106">类型</span><span class="sxs-lookup"><span data-stu-id="af628-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="af628-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="af628-107">reportRefreshDate</span></span> | <span data-ttu-id="af628-108">日期</span><span class="sxs-lookup"><span data-stu-id="af628-108">Date</span></span>              |
| <span data-ttu-id="af628-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af628-109">userPrincipalName</span></span> | <span data-ttu-id="af628-110">字符串</span><span class="sxs-lookup"><span data-stu-id="af628-110">String</span></span>            |
| <span data-ttu-id="af628-111">displayName</span><span class="sxs-lookup"><span data-stu-id="af628-111">displayName</span></span>       | <span data-ttu-id="af628-112">字符串</span><span class="sxs-lookup"><span data-stu-id="af628-112">String</span></span>            |
| <span data-ttu-id="af628-113">userState</span><span class="sxs-lookup"><span data-stu-id="af628-113">userState</span></span>         | <span data-ttu-id="af628-114">字符串</span><span class="sxs-lookup"><span data-stu-id="af628-114">String</span></span>            |
| <span data-ttu-id="af628-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="af628-115">stateChangeDate</span></span>   | <span data-ttu-id="af628-116">日期</span><span class="sxs-lookup"><span data-stu-id="af628-116">Date</span></span>              |
| <span data-ttu-id="af628-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="af628-117">lastActivityDate</span></span>  | <span data-ttu-id="af628-118">日期</span><span class="sxs-lookup"><span data-stu-id="af628-118">Date</span></span>              |
| <span data-ttu-id="af628-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="af628-119">postedCount</span></span>       | <span data-ttu-id="af628-120">Int64</span><span class="sxs-lookup"><span data-stu-id="af628-120">Int64</span></span>             |
| <span data-ttu-id="af628-121">readCount</span><span class="sxs-lookup"><span data-stu-id="af628-121">readCount</span></span>         | <span data-ttu-id="af628-122">Int64</span><span class="sxs-lookup"><span data-stu-id="af628-122">Int64</span></span>             |
| <span data-ttu-id="af628-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="af628-123">likedCount</span></span>        | <span data-ttu-id="af628-124">Int64</span><span class="sxs-lookup"><span data-stu-id="af628-124">Int64</span></span>             |
| <span data-ttu-id="af628-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="af628-125">assignedProducts</span></span>  | <span data-ttu-id="af628-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="af628-126">String collection</span></span> |
| <span data-ttu-id="af628-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="af628-127">reportPeriod</span></span>      | <span data-ttu-id="af628-128">String</span><span class="sxs-lookup"><span data-stu-id="af628-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="af628-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af628-129">JSON representation</span></span>

<span data-ttu-id="af628-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af628-130">The following is a JSON representation of the resource.</span></span>

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
