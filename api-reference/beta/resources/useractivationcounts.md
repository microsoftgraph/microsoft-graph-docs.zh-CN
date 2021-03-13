---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 48adb73bac65ddced88aea3edb18deae7653f5b3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761791"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="bb150-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb150-103">userActivationCounts resource type</span></span>

<span data-ttu-id="bb150-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb150-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="bb150-105">属性</span><span class="sxs-lookup"><span data-stu-id="bb150-105">Properties</span></span>

| <span data-ttu-id="bb150-106">属性</span><span class="sxs-lookup"><span data-stu-id="bb150-106">Property</span></span>          | <span data-ttu-id="bb150-107">类型</span><span class="sxs-lookup"><span data-stu-id="bb150-107">Type</span></span>   | <span data-ttu-id="bb150-108">说明</span><span class="sxs-lookup"><span data-stu-id="bb150-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="bb150-109">productType</span><span class="sxs-lookup"><span data-stu-id="bb150-109">productType</span></span>       | <span data-ttu-id="bb150-110">String</span><span class="sxs-lookup"><span data-stu-id="bb150-110">String</span></span> | <span data-ttu-id="bb150-111">产品类型，例如"Microsoft 365 专业增强版"或"Project 客户端"。</span><span class="sxs-lookup"><span data-stu-id="bb150-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="bb150-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="bb150-112">lastActivatedDate</span></span> | <span data-ttu-id="bb150-113">日期</span><span class="sxs-lookup"><span data-stu-id="bb150-113">Date</span></span>   | <span data-ttu-id="bb150-114">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="bb150-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="bb150-115">windows</span><span class="sxs-lookup"><span data-stu-id="bb150-115">windows</span></span>           | <span data-ttu-id="bb150-116">Int64</span><span class="sxs-lookup"><span data-stu-id="bb150-116">Int64</span></span>  | <span data-ttu-id="bb150-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="bb150-117">The activation count on Windows.</span></span> <span data-ttu-id="bb150-118">此数字包括任何 Windows 计算机上每次激活。</span><span class="sxs-lookup"><span data-stu-id="bb150-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="bb150-119">mac</span><span class="sxs-lookup"><span data-stu-id="bb150-119">mac</span></span>               | <span data-ttu-id="bb150-120">Int64</span><span class="sxs-lookup"><span data-stu-id="bb150-120">Int64</span></span>  | <span data-ttu-id="bb150-121">Mac 操作系统上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="bb150-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="bb150-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="bb150-122">windows10Mobile</span></span>   | <span data-ttu-id="bb150-123">Int64</span><span class="sxs-lookup"><span data-stu-id="bb150-123">Int64</span></span>  | <span data-ttu-id="bb150-124">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="bb150-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="bb150-125">ios</span><span class="sxs-lookup"><span data-stu-id="bb150-125">ios</span></span>               | <span data-ttu-id="bb150-126">Int64</span><span class="sxs-lookup"><span data-stu-id="bb150-126">Int64</span></span>  | <span data-ttu-id="bb150-127">iOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="bb150-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="bb150-128">android</span><span class="sxs-lookup"><span data-stu-id="bb150-128">android</span></span>           | <span data-ttu-id="bb150-129">Int64</span><span class="sxs-lookup"><span data-stu-id="bb150-129">Int64</span></span>  | <span data-ttu-id="bb150-130">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="bb150-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="bb150-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="bb150-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="bb150-132">布尔</span><span class="sxs-lookup"><span data-stu-id="bb150-132">Boolean</span></span> | <span data-ttu-id="bb150-133">如果用户之前在共享计算机上使用过该产品，则其为 True。</span><span class="sxs-lookup"><span data-stu-id="bb150-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bb150-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb150-134">JSON representation</span></span>

<span data-ttu-id="bb150-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb150-135">The following is a JSON representation of the resource.</span></span>

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


