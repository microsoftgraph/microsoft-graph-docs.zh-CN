---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581280"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="6ca53-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ca53-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6ca53-104">属性</span><span class="sxs-lookup"><span data-stu-id="6ca53-104">Properties</span></span>

| <span data-ttu-id="6ca53-105">属性</span><span class="sxs-lookup"><span data-stu-id="6ca53-105">Property</span></span>          | <span data-ttu-id="6ca53-106">类型</span><span class="sxs-lookup"><span data-stu-id="6ca53-106">Type</span></span>   | <span data-ttu-id="6ca53-107">说明</span><span class="sxs-lookup"><span data-stu-id="6ca53-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6ca53-108">productType</span><span class="sxs-lookup"><span data-stu-id="6ca53-108">productType</span></span>       | <span data-ttu-id="6ca53-109">String</span><span class="sxs-lookup"><span data-stu-id="6ca53-109">String</span></span> | <span data-ttu-id="6ca53-110">产品类型, 如 "office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="6ca53-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="6ca53-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="6ca53-111">lastActivatedDate</span></span> | <span data-ttu-id="6ca53-112">Date</span><span class="sxs-lookup"><span data-stu-id="6ca53-112">Date</span></span>   | <span data-ttu-id="6ca53-113">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="6ca53-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="6ca53-114">时间</span><span class="sxs-lookup"><span data-stu-id="6ca53-114">windows</span></span>           | <span data-ttu-id="6ca53-115">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca53-115">Int64</span></span>  | <span data-ttu-id="6ca53-116">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="6ca53-116">The activation count on Windows.</span></span> <span data-ttu-id="6ca53-117">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="6ca53-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="6ca53-118">mac</span><span class="sxs-lookup"><span data-stu-id="6ca53-118">mac</span></span>               | <span data-ttu-id="6ca53-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca53-119">Int64</span></span>  | <span data-ttu-id="6ca53-120">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="6ca53-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="6ca53-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="6ca53-121">windows10Mobile</span></span>   | <span data-ttu-id="6ca53-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca53-122">Int64</span></span>  | <span data-ttu-id="6ca53-123">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="6ca53-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="6ca53-124">ios</span><span class="sxs-lookup"><span data-stu-id="6ca53-124">ios</span></span>               | <span data-ttu-id="6ca53-125">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca53-125">Int64</span></span>  | <span data-ttu-id="6ca53-126">iOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="6ca53-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="6ca53-127">android</span><span class="sxs-lookup"><span data-stu-id="6ca53-127">android</span></span>           | <span data-ttu-id="6ca53-128">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca53-128">Int64</span></span>  | <span data-ttu-id="6ca53-129">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="6ca53-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="6ca53-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="6ca53-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="6ca53-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ca53-131">Boolean</span></span> | <span data-ttu-id="6ca53-132">如此如果用户之前在共享计算机上使用过该产品。</span><span class="sxs-lookup"><span data-stu-id="6ca53-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ca53-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ca53-133">JSON representation</span></span>

<span data-ttu-id="6ca53-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ca53-134">The following is a JSON representation of the resource.</span></span>

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
