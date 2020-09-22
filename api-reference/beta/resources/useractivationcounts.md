---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d81e8078d785761c09aa1070120924b2318415a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057883"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="d636b-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d636b-103">userActivationCounts resource type</span></span>

<span data-ttu-id="d636b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d636b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d636b-105">属性</span><span class="sxs-lookup"><span data-stu-id="d636b-105">Properties</span></span>

| <span data-ttu-id="d636b-106">属性</span><span class="sxs-lookup"><span data-stu-id="d636b-106">Property</span></span>          | <span data-ttu-id="d636b-107">类型</span><span class="sxs-lookup"><span data-stu-id="d636b-107">Type</span></span>   | <span data-ttu-id="d636b-108">说明</span><span class="sxs-lookup"><span data-stu-id="d636b-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d636b-109">productType</span><span class="sxs-lookup"><span data-stu-id="d636b-109">productType</span></span>       | <span data-ttu-id="d636b-110">String</span><span class="sxs-lookup"><span data-stu-id="d636b-110">String</span></span> | <span data-ttu-id="d636b-111">产品类型，如 "Microsoft 365 专业增强版" 或 "Project Client"。</span><span class="sxs-lookup"><span data-stu-id="d636b-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="d636b-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="d636b-112">lastActivatedDate</span></span> | <span data-ttu-id="d636b-113">日期</span><span class="sxs-lookup"><span data-stu-id="d636b-113">Date</span></span>   | <span data-ttu-id="d636b-114">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="d636b-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="d636b-115">时间</span><span class="sxs-lookup"><span data-stu-id="d636b-115">windows</span></span>           | <span data-ttu-id="d636b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d636b-116">Int64</span></span>  | <span data-ttu-id="d636b-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="d636b-117">The activation count on Windows.</span></span> <span data-ttu-id="d636b-118">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="d636b-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="d636b-119">mac</span><span class="sxs-lookup"><span data-stu-id="d636b-119">mac</span></span>               | <span data-ttu-id="d636b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="d636b-120">Int64</span></span>  | <span data-ttu-id="d636b-121">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="d636b-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="d636b-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="d636b-122">windows10Mobile</span></span>   | <span data-ttu-id="d636b-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d636b-123">Int64</span></span>  | <span data-ttu-id="d636b-124">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="d636b-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="d636b-125">ios</span><span class="sxs-lookup"><span data-stu-id="d636b-125">ios</span></span>               | <span data-ttu-id="d636b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d636b-126">Int64</span></span>  | <span data-ttu-id="d636b-127">IOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="d636b-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="d636b-128">android</span><span class="sxs-lookup"><span data-stu-id="d636b-128">android</span></span>           | <span data-ttu-id="d636b-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d636b-129">Int64</span></span>  | <span data-ttu-id="d636b-130">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="d636b-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="d636b-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="d636b-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="d636b-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="d636b-132">Boolean</span></span> | <span data-ttu-id="d636b-133">如此如果用户之前在共享计算机上使用过该产品。</span><span class="sxs-lookup"><span data-stu-id="d636b-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d636b-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d636b-134">JSON representation</span></span>

<span data-ttu-id="d636b-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d636b-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```


