---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980347"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="052f4-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="052f4-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="052f4-104">属性</span><span class="sxs-lookup"><span data-stu-id="052f4-104">Properties</span></span>

| <span data-ttu-id="052f4-105">属性</span><span class="sxs-lookup"><span data-stu-id="052f4-105">Property</span></span>          | <span data-ttu-id="052f4-106">类型</span><span class="sxs-lookup"><span data-stu-id="052f4-106">Type</span></span>   | <span data-ttu-id="052f4-107">Description</span><span class="sxs-lookup"><span data-stu-id="052f4-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="052f4-108">productType</span><span class="sxs-lookup"><span data-stu-id="052f4-108">productType</span></span>       | <span data-ttu-id="052f4-109">字符串</span><span class="sxs-lookup"><span data-stu-id="052f4-109">String</span></span> | <span data-ttu-id="052f4-110">产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="052f4-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="052f4-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="052f4-111">lastActivatedDate</span></span> | <span data-ttu-id="052f4-112">日期</span><span class="sxs-lookup"><span data-stu-id="052f4-112">Date</span></span>   | <span data-ttu-id="052f4-113">最新的激活日期。</span><span class="sxs-lookup"><span data-stu-id="052f4-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="052f4-114">windows</span><span class="sxs-lookup"><span data-stu-id="052f4-114">windows</span></span>           | <span data-ttu-id="052f4-115">Int64</span><span class="sxs-lookup"><span data-stu-id="052f4-115">Int64</span></span>  | <span data-ttu-id="052f4-116">Windows 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="052f4-116">The activation count on Windows.</span></span> <span data-ttu-id="052f4-117">此数值包括 Windows 中的任何计算机上的每个激活。</span><span class="sxs-lookup"><span data-stu-id="052f4-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="052f4-118">mac</span><span class="sxs-lookup"><span data-stu-id="052f4-118">mac</span></span>               | <span data-ttu-id="052f4-119">Int64</span><span class="sxs-lookup"><span data-stu-id="052f4-119">Int64</span></span>  | <span data-ttu-id="052f4-120">Mac OS 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="052f4-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="052f4-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="052f4-121">windows10Mobile</span></span>   | <span data-ttu-id="052f4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="052f4-122">Int64</span></span>  | <span data-ttu-id="052f4-123">在激活依靠 Windows 10 移动。</span><span class="sxs-lookup"><span data-stu-id="052f4-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="052f4-124">ios</span><span class="sxs-lookup"><span data-stu-id="052f4-124">ios</span></span>               | <span data-ttu-id="052f4-125">Int64</span><span class="sxs-lookup"><span data-stu-id="052f4-125">Int64</span></span>  | <span data-ttu-id="052f4-126">在 iOS 激活计数。</span><span class="sxs-lookup"><span data-stu-id="052f4-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="052f4-127">android</span><span class="sxs-lookup"><span data-stu-id="052f4-127">android</span></span>           | <span data-ttu-id="052f4-128">Int64</span><span class="sxs-lookup"><span data-stu-id="052f4-128">Int64</span></span>  | <span data-ttu-id="052f4-129">在 Android 设备上激活计数。</span><span class="sxs-lookup"><span data-stu-id="052f4-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="052f4-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="052f4-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="052f4-131">布尔</span><span class="sxs-lookup"><span data-stu-id="052f4-131">Boolean</span></span> | <span data-ttu-id="052f4-132">如果用户使用该产品之前的共享计算机上，则为 true。</span><span class="sxs-lookup"><span data-stu-id="052f4-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="052f4-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="052f4-133">JSON representation</span></span>

<span data-ttu-id="052f4-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="052f4-134">The following is a JSON representation of the resource.</span></span>

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
