---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6433c1680630b5805cd18a22e550e58a51bcefbc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898301"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="96b1a-103">userActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="96b1a-103">userActivationCounts resource type</span></span>

<span data-ttu-id="96b1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96b1a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="96b1a-105">属性</span><span class="sxs-lookup"><span data-stu-id="96b1a-105">Properties</span></span>

| <span data-ttu-id="96b1a-106">属性</span><span class="sxs-lookup"><span data-stu-id="96b1a-106">Property</span></span>          | <span data-ttu-id="96b1a-107">类型</span><span class="sxs-lookup"><span data-stu-id="96b1a-107">Type</span></span>   | <span data-ttu-id="96b1a-108">说明</span><span class="sxs-lookup"><span data-stu-id="96b1a-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="96b1a-109">productType</span><span class="sxs-lookup"><span data-stu-id="96b1a-109">productType</span></span>       | <span data-ttu-id="96b1a-110">String</span><span class="sxs-lookup"><span data-stu-id="96b1a-110">String</span></span> | <span data-ttu-id="96b1a-111">产品类型，如 "Microsoft 365 专业增强版" 或 "Project Client"。</span><span class="sxs-lookup"><span data-stu-id="96b1a-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="96b1a-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="96b1a-112">lastActivatedDate</span></span> | <span data-ttu-id="96b1a-113">日期</span><span class="sxs-lookup"><span data-stu-id="96b1a-113">Date</span></span>   | <span data-ttu-id="96b1a-114">最新激活的日期。</span><span class="sxs-lookup"><span data-stu-id="96b1a-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="96b1a-115">时间</span><span class="sxs-lookup"><span data-stu-id="96b1a-115">windows</span></span>           | <span data-ttu-id="96b1a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="96b1a-116">Int64</span></span>  | <span data-ttu-id="96b1a-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="96b1a-117">The activation count on Windows.</span></span> <span data-ttu-id="96b1a-118">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="96b1a-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="96b1a-119">mac</span><span class="sxs-lookup"><span data-stu-id="96b1a-119">mac</span></span>               | <span data-ttu-id="96b1a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="96b1a-120">Int64</span></span>  | <span data-ttu-id="96b1a-121">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="96b1a-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="96b1a-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="96b1a-122">windows10Mobile</span></span>   | <span data-ttu-id="96b1a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="96b1a-123">Int64</span></span>  | <span data-ttu-id="96b1a-124">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="96b1a-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="96b1a-125">ios</span><span class="sxs-lookup"><span data-stu-id="96b1a-125">ios</span></span>               | <span data-ttu-id="96b1a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="96b1a-126">Int64</span></span>  | <span data-ttu-id="96b1a-127">IOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="96b1a-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="96b1a-128">android</span><span class="sxs-lookup"><span data-stu-id="96b1a-128">android</span></span>           | <span data-ttu-id="96b1a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="96b1a-129">Int64</span></span>  | <span data-ttu-id="96b1a-130">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="96b1a-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="96b1a-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="96b1a-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="96b1a-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="96b1a-132">Boolean</span></span> | <span data-ttu-id="96b1a-133">如此如果用户之前在共享计算机上使用过该产品。</span><span class="sxs-lookup"><span data-stu-id="96b1a-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96b1a-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96b1a-134">JSON representation</span></span>

<span data-ttu-id="96b1a-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96b1a-135">The following is a JSON representation of the resource.</span></span>

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
