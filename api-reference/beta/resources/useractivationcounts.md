---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91366f9d2b2308c997c111123d856581db7c00c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384952"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="4f912-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f912-103">userActivationCounts resource type</span></span>

<span data-ttu-id="4f912-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f912-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="4f912-105">属性</span><span class="sxs-lookup"><span data-stu-id="4f912-105">Properties</span></span>

| <span data-ttu-id="4f912-106">属性</span><span class="sxs-lookup"><span data-stu-id="4f912-106">Property</span></span>          | <span data-ttu-id="4f912-107">类型</span><span class="sxs-lookup"><span data-stu-id="4f912-107">Type</span></span>   | <span data-ttu-id="4f912-108">说明</span><span class="sxs-lookup"><span data-stu-id="4f912-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="4f912-109">productType</span><span class="sxs-lookup"><span data-stu-id="4f912-109">productType</span></span>       | <span data-ttu-id="4f912-110">字符串</span><span class="sxs-lookup"><span data-stu-id="4f912-110">String</span></span> | <span data-ttu-id="4f912-111">产品类型，如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="4f912-111">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="4f912-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="4f912-112">lastActivatedDate</span></span> | <span data-ttu-id="4f912-113">日期</span><span class="sxs-lookup"><span data-stu-id="4f912-113">Date</span></span>   | <span data-ttu-id="4f912-114">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="4f912-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="4f912-115">时间</span><span class="sxs-lookup"><span data-stu-id="4f912-115">windows</span></span>           | <span data-ttu-id="4f912-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4f912-116">Int64</span></span>  | <span data-ttu-id="4f912-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f912-117">The activation count on Windows.</span></span> <span data-ttu-id="4f912-118">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="4f912-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="4f912-119">mac</span><span class="sxs-lookup"><span data-stu-id="4f912-119">mac</span></span>               | <span data-ttu-id="4f912-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4f912-120">Int64</span></span>  | <span data-ttu-id="4f912-121">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f912-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="4f912-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="4f912-122">windows10Mobile</span></span>   | <span data-ttu-id="4f912-123">Int64</span><span class="sxs-lookup"><span data-stu-id="4f912-123">Int64</span></span>  | <span data-ttu-id="4f912-124">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f912-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="4f912-125">ios</span><span class="sxs-lookup"><span data-stu-id="4f912-125">ios</span></span>               | <span data-ttu-id="4f912-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4f912-126">Int64</span></span>  | <span data-ttu-id="4f912-127">IOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f912-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="4f912-128">android</span><span class="sxs-lookup"><span data-stu-id="4f912-128">android</span></span>           | <span data-ttu-id="4f912-129">Int64</span><span class="sxs-lookup"><span data-stu-id="4f912-129">Int64</span></span>  | <span data-ttu-id="4f912-130">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f912-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="4f912-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="4f912-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="4f912-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f912-132">Boolean</span></span> | <span data-ttu-id="4f912-133">如此如果用户之前在共享计算机上使用过该产品。</span><span class="sxs-lookup"><span data-stu-id="4f912-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f912-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f912-134">JSON representation</span></span>

<span data-ttu-id="4f912-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f912-135">The following is a JSON representation of the resource.</span></span>

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
