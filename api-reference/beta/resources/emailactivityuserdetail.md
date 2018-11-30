---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 4f74b4af41c44e41b07bae1a8421011bc5188efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041469"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="98708-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="98708-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="98708-104">属性</span><span class="sxs-lookup"><span data-stu-id="98708-104">Properties</span></span>

| <span data-ttu-id="98708-105">属性</span><span class="sxs-lookup"><span data-stu-id="98708-105">Property</span></span>          | <span data-ttu-id="98708-106">类型</span><span class="sxs-lookup"><span data-stu-id="98708-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="98708-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="98708-107">reportRefreshDate</span></span> | <span data-ttu-id="98708-108">日期</span><span class="sxs-lookup"><span data-stu-id="98708-108">Date</span></span>              |
| <span data-ttu-id="98708-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="98708-109">userPrincipalName</span></span> | <span data-ttu-id="98708-110">字符串</span><span class="sxs-lookup"><span data-stu-id="98708-110">String</span></span>            |
| <span data-ttu-id="98708-111">displayName</span><span class="sxs-lookup"><span data-stu-id="98708-111">displayName</span></span>       | <span data-ttu-id="98708-112">字符串</span><span class="sxs-lookup"><span data-stu-id="98708-112">String</span></span>            |
| <span data-ttu-id="98708-113">被</span><span class="sxs-lookup"><span data-stu-id="98708-113">isDeleted</span></span>         | <span data-ttu-id="98708-114">布尔</span><span class="sxs-lookup"><span data-stu-id="98708-114">Boolean</span></span>           |
| <span data-ttu-id="98708-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="98708-115">deletedDate</span></span>       | <span data-ttu-id="98708-116">日期</span><span class="sxs-lookup"><span data-stu-id="98708-116">Date</span></span>              |
| <span data-ttu-id="98708-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="98708-117">lastActivityDate</span></span>  | <span data-ttu-id="98708-118">日期</span><span class="sxs-lookup"><span data-stu-id="98708-118">Date</span></span>              |
| <span data-ttu-id="98708-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="98708-119">sendCount</span></span>         | <span data-ttu-id="98708-120">Int64</span><span class="sxs-lookup"><span data-stu-id="98708-120">Int64</span></span>             |
| <span data-ttu-id="98708-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="98708-121">receiveCount</span></span>      | <span data-ttu-id="98708-122">Int64</span><span class="sxs-lookup"><span data-stu-id="98708-122">Int64</span></span>             |
| <span data-ttu-id="98708-123">readCount</span><span class="sxs-lookup"><span data-stu-id="98708-123">readCount</span></span>         | <span data-ttu-id="98708-124">Int64</span><span class="sxs-lookup"><span data-stu-id="98708-124">Int64</span></span>             |
| <span data-ttu-id="98708-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="98708-125">assignedProducts</span></span>  | <span data-ttu-id="98708-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="98708-126">String collection</span></span> |
| <span data-ttu-id="98708-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="98708-127">reportPeriod</span></span>      | <span data-ttu-id="98708-128">String</span><span class="sxs-lookup"><span data-stu-id="98708-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="98708-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98708-129">JSON representation</span></span>

<span data-ttu-id="98708-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98708-130">The following is a JSON representation of the resource.</span></span>

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
