---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: jpettere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719a73739a64dca2bd7a052cc9cdd51007173eff
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719897"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="a9c30-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9c30-103">userActivationCounts resource type</span></span>

<span data-ttu-id="a9c30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9c30-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a9c30-105">属性</span><span class="sxs-lookup"><span data-stu-id="a9c30-105">Properties</span></span>

| <span data-ttu-id="a9c30-106">属性</span><span class="sxs-lookup"><span data-stu-id="a9c30-106">Property</span></span>          | <span data-ttu-id="a9c30-107">类型</span><span class="sxs-lookup"><span data-stu-id="a9c30-107">Type</span></span>   | <span data-ttu-id="a9c30-108">说明</span><span class="sxs-lookup"><span data-stu-id="a9c30-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a9c30-109">productType</span><span class="sxs-lookup"><span data-stu-id="a9c30-109">productType</span></span>       | <span data-ttu-id="a9c30-110">String</span><span class="sxs-lookup"><span data-stu-id="a9c30-110">String</span></span> | <span data-ttu-id="a9c30-111">产品类型，例如"Microsoft 365 ProPlus"或"Project Client"。</span><span class="sxs-lookup"><span data-stu-id="a9c30-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="a9c30-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="a9c30-112">lastActivatedDate</span></span> | <span data-ttu-id="a9c30-113">日期</span><span class="sxs-lookup"><span data-stu-id="a9c30-113">Date</span></span>   | <span data-ttu-id="a9c30-114">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="a9c30-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="a9c30-115">windows</span><span class="sxs-lookup"><span data-stu-id="a9c30-115">windows</span></span>           | <span data-ttu-id="a9c30-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a9c30-116">Int64</span></span>  | <span data-ttu-id="a9c30-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="a9c30-117">The activation count on Windows.</span></span> <span data-ttu-id="a9c30-118">此数字包括任何 Windows 计算机上每次激活。</span><span class="sxs-lookup"><span data-stu-id="a9c30-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="a9c30-119">mac</span><span class="sxs-lookup"><span data-stu-id="a9c30-119">mac</span></span>               | <span data-ttu-id="a9c30-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a9c30-120">Int64</span></span>  | <span data-ttu-id="a9c30-121">Mac 操作系统上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="a9c30-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="a9c30-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="a9c30-122">windows10Mobile</span></span>   | <span data-ttu-id="a9c30-123">Int64</span><span class="sxs-lookup"><span data-stu-id="a9c30-123">Int64</span></span>  | <span data-ttu-id="a9c30-124">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="a9c30-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="a9c30-125">ios</span><span class="sxs-lookup"><span data-stu-id="a9c30-125">ios</span></span>               | <span data-ttu-id="a9c30-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a9c30-126">Int64</span></span>  | <span data-ttu-id="a9c30-127">iOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="a9c30-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="a9c30-128">android</span><span class="sxs-lookup"><span data-stu-id="a9c30-128">android</span></span>           | <span data-ttu-id="a9c30-129">Int64</span><span class="sxs-lookup"><span data-stu-id="a9c30-129">Int64</span></span>  | <span data-ttu-id="a9c30-130">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="a9c30-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="a9c30-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="a9c30-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="a9c30-132">布尔</span><span class="sxs-lookup"><span data-stu-id="a9c30-132">Boolean</span></span> | <span data-ttu-id="a9c30-133">如果用户之前在共享计算机上使用过该产品，则其为 True。</span><span class="sxs-lookup"><span data-stu-id="a9c30-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9c30-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9c30-134">JSON representation</span></span>

<span data-ttu-id="a9c30-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9c30-135">The following is a JSON representation of the resource.</span></span>

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


