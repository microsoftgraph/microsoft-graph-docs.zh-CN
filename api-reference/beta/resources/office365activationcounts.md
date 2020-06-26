---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1e514eb538b1edc4d9681b9937fe8cfeecc40b23
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896887"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="7a7d8-103">office365ActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a7d8-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="7a7d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a7d8-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7a7d8-105">属性</span><span class="sxs-lookup"><span data-stu-id="7a7d8-105">Properties</span></span>

| <span data-ttu-id="7a7d8-106">属性</span><span class="sxs-lookup"><span data-stu-id="7a7d8-106">Property</span></span>          | <span data-ttu-id="7a7d8-107">类型</span><span class="sxs-lookup"><span data-stu-id="7a7d8-107">Type</span></span>   | <span data-ttu-id="7a7d8-108">说明</span><span class="sxs-lookup"><span data-stu-id="7a7d8-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="7a7d8-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7a7d8-109">reportRefreshDate</span></span> | <span data-ttu-id="7a7d8-110">日期</span><span class="sxs-lookup"><span data-stu-id="7a7d8-110">Date</span></span>   | <span data-ttu-id="7a7d8-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="7a7d8-112">productType</span><span class="sxs-lookup"><span data-stu-id="7a7d8-112">productType</span></span>       | <span data-ttu-id="7a7d8-113">String</span><span class="sxs-lookup"><span data-stu-id="7a7d8-113">String</span></span> | <span data-ttu-id="7a7d8-114">产品类型，如 "Microsoft 365 专业增强版" 或 "Project Client"。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-114">The product type, such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="7a7d8-115">时间</span><span class="sxs-lookup"><span data-stu-id="7a7d8-115">windows</span></span>           | <span data-ttu-id="7a7d8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7a7d8-116">Int64</span></span>  | <span data-ttu-id="7a7d8-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-117">The activation count on Windows.</span></span> <span data-ttu-id="7a7d8-118">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="7a7d8-119">mac</span><span class="sxs-lookup"><span data-stu-id="7a7d8-119">mac</span></span>               | <span data-ttu-id="7a7d8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="7a7d8-120">Int64</span></span>  | <span data-ttu-id="7a7d8-121">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="7a7d8-122">android</span><span class="sxs-lookup"><span data-stu-id="7a7d8-122">android</span></span>           | <span data-ttu-id="7a7d8-123">Int64</span><span class="sxs-lookup"><span data-stu-id="7a7d8-123">Int64</span></span>  | <span data-ttu-id="7a7d8-124">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="7a7d8-125">ios</span><span class="sxs-lookup"><span data-stu-id="7a7d8-125">ios</span></span>               | <span data-ttu-id="7a7d8-126">Int64</span><span class="sxs-lookup"><span data-stu-id="7a7d8-126">Int64</span></span>  | <span data-ttu-id="7a7d8-127">IOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="7a7d8-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="7a7d8-128">windows10Mobile</span></span>   | <span data-ttu-id="7a7d8-129">Int64</span><span class="sxs-lookup"><span data-stu-id="7a7d8-129">Int64</span></span>  | <span data-ttu-id="7a7d8-130">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a7d8-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a7d8-131">JSON representation</span></span>

<span data-ttu-id="7a7d8-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a7d8-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
