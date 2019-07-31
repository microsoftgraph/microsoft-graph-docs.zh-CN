---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9c1dbbaa6a429a90a54f8af5f3b380ff58c86dab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007492"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="edd63-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="edd63-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="edd63-104">属性</span><span class="sxs-lookup"><span data-stu-id="edd63-104">Properties</span></span>

| <span data-ttu-id="edd63-105">属性</span><span class="sxs-lookup"><span data-stu-id="edd63-105">Property</span></span>          | <span data-ttu-id="edd63-106">类型</span><span class="sxs-lookup"><span data-stu-id="edd63-106">Type</span></span>   | <span data-ttu-id="edd63-107">说明</span><span class="sxs-lookup"><span data-stu-id="edd63-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="edd63-108">productType</span><span class="sxs-lookup"><span data-stu-id="edd63-108">productType</span></span>       | <span data-ttu-id="edd63-109">String</span><span class="sxs-lookup"><span data-stu-id="edd63-109">String</span></span> | <span data-ttu-id="edd63-110">产品类型, 如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="edd63-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="edd63-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="edd63-111">lastActivatedDate</span></span> | <span data-ttu-id="edd63-112">日期</span><span class="sxs-lookup"><span data-stu-id="edd63-112">Date</span></span>   | <span data-ttu-id="edd63-113">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="edd63-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="edd63-114">时间</span><span class="sxs-lookup"><span data-stu-id="edd63-114">windows</span></span>           | <span data-ttu-id="edd63-115">Int64</span><span class="sxs-lookup"><span data-stu-id="edd63-115">Int64</span></span>  | <span data-ttu-id="edd63-116">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="edd63-116">The activation count on Windows.</span></span> <span data-ttu-id="edd63-117">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="edd63-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="edd63-118">mac</span><span class="sxs-lookup"><span data-stu-id="edd63-118">mac</span></span>               | <span data-ttu-id="edd63-119">Int64</span><span class="sxs-lookup"><span data-stu-id="edd63-119">Int64</span></span>  | <span data-ttu-id="edd63-120">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="edd63-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="edd63-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="edd63-121">windows10Mobile</span></span>   | <span data-ttu-id="edd63-122">Int64</span><span class="sxs-lookup"><span data-stu-id="edd63-122">Int64</span></span>  | <span data-ttu-id="edd63-123">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="edd63-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="edd63-124">ios</span><span class="sxs-lookup"><span data-stu-id="edd63-124">ios</span></span>               | <span data-ttu-id="edd63-125">Int64</span><span class="sxs-lookup"><span data-stu-id="edd63-125">Int64</span></span>  | <span data-ttu-id="edd63-126">IOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="edd63-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="edd63-127">android</span><span class="sxs-lookup"><span data-stu-id="edd63-127">android</span></span>           | <span data-ttu-id="edd63-128">Int64</span><span class="sxs-lookup"><span data-stu-id="edd63-128">Int64</span></span>  | <span data-ttu-id="edd63-129">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="edd63-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="edd63-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="edd63-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="edd63-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="edd63-131">Boolean</span></span> | <span data-ttu-id="edd63-132">如此如果用户之前在共享计算机上使用过该产品。</span><span class="sxs-lookup"><span data-stu-id="edd63-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="edd63-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edd63-133">JSON representation</span></span>

<span data-ttu-id="edd63-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edd63-134">The following is a JSON representation of the resource.</span></span>

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
