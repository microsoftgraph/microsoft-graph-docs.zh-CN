---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 16512c3a8a4dab62d4a71406d6c33d52a5a9bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817997"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="3818c-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="3818c-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3818c-104">属性</span><span class="sxs-lookup"><span data-stu-id="3818c-104">Properties</span></span>

| <span data-ttu-id="3818c-105">属性</span><span class="sxs-lookup"><span data-stu-id="3818c-105">Property</span></span>          | <span data-ttu-id="3818c-106">类型</span><span class="sxs-lookup"><span data-stu-id="3818c-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="3818c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3818c-107">reportRefreshDate</span></span> | <span data-ttu-id="3818c-108">日期</span><span class="sxs-lookup"><span data-stu-id="3818c-108">Date</span></span>              |
| <span data-ttu-id="3818c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3818c-109">userPrincipalName</span></span> | <span data-ttu-id="3818c-110">字符串</span><span class="sxs-lookup"><span data-stu-id="3818c-110">String</span></span>            |
| <span data-ttu-id="3818c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3818c-111">displayName</span></span>       | <span data-ttu-id="3818c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="3818c-112">String</span></span>            |
| <span data-ttu-id="3818c-113">被</span><span class="sxs-lookup"><span data-stu-id="3818c-113">isDeleted</span></span>         | <span data-ttu-id="3818c-114">布尔</span><span class="sxs-lookup"><span data-stu-id="3818c-114">Boolean</span></span>           |
| <span data-ttu-id="3818c-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="3818c-115">deletedDate</span></span>       | <span data-ttu-id="3818c-116">日期</span><span class="sxs-lookup"><span data-stu-id="3818c-116">Date</span></span>              |
| <span data-ttu-id="3818c-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3818c-117">lastActivityDate</span></span>  | <span data-ttu-id="3818c-118">日期</span><span class="sxs-lookup"><span data-stu-id="3818c-118">Date</span></span>              |
| <span data-ttu-id="3818c-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="3818c-119">sendCount</span></span>         | <span data-ttu-id="3818c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3818c-120">Int64</span></span>             |
| <span data-ttu-id="3818c-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="3818c-121">receiveCount</span></span>      | <span data-ttu-id="3818c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3818c-122">Int64</span></span>             |
| <span data-ttu-id="3818c-123">readCount</span><span class="sxs-lookup"><span data-stu-id="3818c-123">readCount</span></span>         | <span data-ttu-id="3818c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3818c-124">Int64</span></span>             |
| <span data-ttu-id="3818c-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="3818c-125">assignedProducts</span></span>  | <span data-ttu-id="3818c-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="3818c-126">String collection</span></span> |
| <span data-ttu-id="3818c-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3818c-127">reportPeriod</span></span>      | <span data-ttu-id="3818c-128">String</span><span class="sxs-lookup"><span data-stu-id="3818c-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="3818c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3818c-129">JSON representation</span></span>

<span data-ttu-id="3818c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3818c-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
