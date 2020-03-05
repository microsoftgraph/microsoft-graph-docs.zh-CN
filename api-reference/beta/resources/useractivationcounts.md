---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65554254260d640638e7cbbbb2d0a0076e209f22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519545"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="56e76-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="56e76-103">userActivationCounts resource type</span></span>

<span data-ttu-id="56e76-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="56e76-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="56e76-105">属性</span><span class="sxs-lookup"><span data-stu-id="56e76-105">Properties</span></span>

| <span data-ttu-id="56e76-106">属性</span><span class="sxs-lookup"><span data-stu-id="56e76-106">Property</span></span>          | <span data-ttu-id="56e76-107">类型</span><span class="sxs-lookup"><span data-stu-id="56e76-107">Type</span></span>   | <span data-ttu-id="56e76-108">说明</span><span class="sxs-lookup"><span data-stu-id="56e76-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="56e76-109">productType</span><span class="sxs-lookup"><span data-stu-id="56e76-109">productType</span></span>       | <span data-ttu-id="56e76-110">String</span><span class="sxs-lookup"><span data-stu-id="56e76-110">String</span></span> | <span data-ttu-id="56e76-111">产品类型，如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="56e76-111">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="56e76-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="56e76-112">lastActivatedDate</span></span> | <span data-ttu-id="56e76-113">日期</span><span class="sxs-lookup"><span data-stu-id="56e76-113">Date</span></span>   | <span data-ttu-id="56e76-114">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="56e76-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="56e76-115">时间</span><span class="sxs-lookup"><span data-stu-id="56e76-115">windows</span></span>           | <span data-ttu-id="56e76-116">Int64</span><span class="sxs-lookup"><span data-stu-id="56e76-116">Int64</span></span>  | <span data-ttu-id="56e76-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="56e76-117">The activation count on Windows.</span></span> <span data-ttu-id="56e76-118">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="56e76-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="56e76-119">mac</span><span class="sxs-lookup"><span data-stu-id="56e76-119">mac</span></span>               | <span data-ttu-id="56e76-120">Int64</span><span class="sxs-lookup"><span data-stu-id="56e76-120">Int64</span></span>  | <span data-ttu-id="56e76-121">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="56e76-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="56e76-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="56e76-122">windows10Mobile</span></span>   | <span data-ttu-id="56e76-123">Int64</span><span class="sxs-lookup"><span data-stu-id="56e76-123">Int64</span></span>  | <span data-ttu-id="56e76-124">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="56e76-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="56e76-125">ios</span><span class="sxs-lookup"><span data-stu-id="56e76-125">ios</span></span>               | <span data-ttu-id="56e76-126">Int64</span><span class="sxs-lookup"><span data-stu-id="56e76-126">Int64</span></span>  | <span data-ttu-id="56e76-127">IOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="56e76-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="56e76-128">android</span><span class="sxs-lookup"><span data-stu-id="56e76-128">android</span></span>           | <span data-ttu-id="56e76-129">Int64</span><span class="sxs-lookup"><span data-stu-id="56e76-129">Int64</span></span>  | <span data-ttu-id="56e76-130">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="56e76-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="56e76-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="56e76-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="56e76-132">布尔</span><span class="sxs-lookup"><span data-stu-id="56e76-132">Boolean</span></span> | <span data-ttu-id="56e76-133">如此如果用户之前在共享计算机上使用过该产品。</span><span class="sxs-lookup"><span data-stu-id="56e76-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56e76-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56e76-134">JSON representation</span></span>

<span data-ttu-id="56e76-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56e76-135">The following is a JSON representation of the resource.</span></span>

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
