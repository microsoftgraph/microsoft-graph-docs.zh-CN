---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: dkershaw10
ms.openlocfilehash: 396f6182d000df6d701e8c0cbad3dd02a258c4c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322916"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="ec0c8-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec0c8-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ec0c8-104">属性</span><span class="sxs-lookup"><span data-stu-id="ec0c8-104">Properties</span></span>

| <span data-ttu-id="ec0c8-105">属性</span><span class="sxs-lookup"><span data-stu-id="ec0c8-105">Property</span></span>          | <span data-ttu-id="ec0c8-106">类型</span><span class="sxs-lookup"><span data-stu-id="ec0c8-106">Type</span></span>   | <span data-ttu-id="ec0c8-107">说明</span><span class="sxs-lookup"><span data-stu-id="ec0c8-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="ec0c8-108">productType</span><span class="sxs-lookup"><span data-stu-id="ec0c8-108">productType</span></span>       | <span data-ttu-id="ec0c8-109">字符串</span><span class="sxs-lookup"><span data-stu-id="ec0c8-109">String</span></span> | <span data-ttu-id="ec0c8-110">产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="ec0c8-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="ec0c8-111">lastActivatedDate</span></span> | <span data-ttu-id="ec0c8-112">日期</span><span class="sxs-lookup"><span data-stu-id="ec0c8-112">Date</span></span>   | <span data-ttu-id="ec0c8-113">最新的激活日期。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="ec0c8-114">windows</span><span class="sxs-lookup"><span data-stu-id="ec0c8-114">windows</span></span>           | <span data-ttu-id="ec0c8-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0c8-115">Int64</span></span>  | <span data-ttu-id="ec0c8-116">Windows 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-116">The activation count on Windows.</span></span> <span data-ttu-id="ec0c8-117">此数值包括 Windows 中的任何计算机上的每个激活。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="ec0c8-118">mac</span><span class="sxs-lookup"><span data-stu-id="ec0c8-118">mac</span></span>               | <span data-ttu-id="ec0c8-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0c8-119">Int64</span></span>  | <span data-ttu-id="ec0c8-120">Mac OS 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="ec0c8-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="ec0c8-121">windows10Mobile</span></span>   | <span data-ttu-id="ec0c8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0c8-122">Int64</span></span>  | <span data-ttu-id="ec0c8-123">在激活依靠 Windows 10 移动。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="ec0c8-124">ios</span><span class="sxs-lookup"><span data-stu-id="ec0c8-124">ios</span></span>               | <span data-ttu-id="ec0c8-125">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0c8-125">Int64</span></span>  | <span data-ttu-id="ec0c8-126">在 iOS 激活计数。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="ec0c8-127">android</span><span class="sxs-lookup"><span data-stu-id="ec0c8-127">android</span></span>           | <span data-ttu-id="ec0c8-128">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0c8-128">Int64</span></span>  | <span data-ttu-id="ec0c8-129">在 Android 设备上激活计数。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="ec0c8-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="ec0c8-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="ec0c8-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec0c8-131">Boolean</span></span> | <span data-ttu-id="ec0c8-132">如果用户使用该产品之前的共享计算机上，则为 true。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ec0c8-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec0c8-133">JSON representation</span></span>

<span data-ttu-id="ec0c8-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec0c8-134">The following is a JSON representation of the resource.</span></span>

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
