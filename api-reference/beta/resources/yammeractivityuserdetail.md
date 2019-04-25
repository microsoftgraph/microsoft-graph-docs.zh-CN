---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541183"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="5cd21-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cd21-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5cd21-104">属性</span><span class="sxs-lookup"><span data-stu-id="5cd21-104">Properties</span></span>

| <span data-ttu-id="5cd21-105">属性</span><span class="sxs-lookup"><span data-stu-id="5cd21-105">Property</span></span>          | <span data-ttu-id="5cd21-106">类型</span><span class="sxs-lookup"><span data-stu-id="5cd21-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="5cd21-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5cd21-107">reportRefreshDate</span></span> | <span data-ttu-id="5cd21-108">Date</span><span class="sxs-lookup"><span data-stu-id="5cd21-108">Date</span></span>              |
| <span data-ttu-id="5cd21-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5cd21-109">userPrincipalName</span></span> | <span data-ttu-id="5cd21-110">String</span><span class="sxs-lookup"><span data-stu-id="5cd21-110">String</span></span>            |
| <span data-ttu-id="5cd21-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5cd21-111">displayName</span></span>       | <span data-ttu-id="5cd21-112">String</span><span class="sxs-lookup"><span data-stu-id="5cd21-112">String</span></span>            |
| <span data-ttu-id="5cd21-113">userState</span><span class="sxs-lookup"><span data-stu-id="5cd21-113">userState</span></span>         | <span data-ttu-id="5cd21-114">String</span><span class="sxs-lookup"><span data-stu-id="5cd21-114">String</span></span>            |
| <span data-ttu-id="5cd21-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="5cd21-115">stateChangeDate</span></span>   | <span data-ttu-id="5cd21-116">Date</span><span class="sxs-lookup"><span data-stu-id="5cd21-116">Date</span></span>              |
| <span data-ttu-id="5cd21-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="5cd21-117">lastActivityDate</span></span>  | <span data-ttu-id="5cd21-118">Date</span><span class="sxs-lookup"><span data-stu-id="5cd21-118">Date</span></span>              |
| <span data-ttu-id="5cd21-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="5cd21-119">postedCount</span></span>       | <span data-ttu-id="5cd21-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5cd21-120">Int64</span></span>             |
| <span data-ttu-id="5cd21-121">readCount</span><span class="sxs-lookup"><span data-stu-id="5cd21-121">readCount</span></span>         | <span data-ttu-id="5cd21-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5cd21-122">Int64</span></span>             |
| <span data-ttu-id="5cd21-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="5cd21-123">likedCount</span></span>        | <span data-ttu-id="5cd21-124">Int64</span><span class="sxs-lookup"><span data-stu-id="5cd21-124">Int64</span></span>             |
| <span data-ttu-id="5cd21-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="5cd21-125">assignedProducts</span></span>  | <span data-ttu-id="5cd21-126">String collection</span><span class="sxs-lookup"><span data-stu-id="5cd21-126">String collection</span></span> |
| <span data-ttu-id="5cd21-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5cd21-127">reportPeriod</span></span>      | <span data-ttu-id="5cd21-128">String</span><span class="sxs-lookup"><span data-stu-id="5cd21-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="5cd21-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cd21-129">JSON representation</span></span>

<span data-ttu-id="5cd21-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cd21-130">The following is a JSON representation of the resource.</span></span>

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
