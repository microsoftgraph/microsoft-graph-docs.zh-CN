---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1a45aa058a5186e87d11eed5199b51abf709879b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522489"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="13024-103">office365ActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="13024-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="13024-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="13024-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="13024-105">属性</span><span class="sxs-lookup"><span data-stu-id="13024-105">Properties</span></span>

| <span data-ttu-id="13024-106">属性</span><span class="sxs-lookup"><span data-stu-id="13024-106">Property</span></span>          | <span data-ttu-id="13024-107">类型</span><span class="sxs-lookup"><span data-stu-id="13024-107">Type</span></span>   | <span data-ttu-id="13024-108">说明</span><span class="sxs-lookup"><span data-stu-id="13024-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="13024-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="13024-109">reportRefreshDate</span></span> | <span data-ttu-id="13024-110">日期</span><span class="sxs-lookup"><span data-stu-id="13024-110">Date</span></span>   | <span data-ttu-id="13024-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="13024-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="13024-112">productType</span><span class="sxs-lookup"><span data-stu-id="13024-112">productType</span></span>       | <span data-ttu-id="13024-113">String</span><span class="sxs-lookup"><span data-stu-id="13024-113">String</span></span> | <span data-ttu-id="13024-114">产品类型，如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="13024-114">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="13024-115">时间</span><span class="sxs-lookup"><span data-stu-id="13024-115">windows</span></span>           | <span data-ttu-id="13024-116">Int64</span><span class="sxs-lookup"><span data-stu-id="13024-116">Int64</span></span>  | <span data-ttu-id="13024-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="13024-117">The activation count on Windows.</span></span> <span data-ttu-id="13024-118">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="13024-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="13024-119">mac</span><span class="sxs-lookup"><span data-stu-id="13024-119">mac</span></span>               | <span data-ttu-id="13024-120">Int64</span><span class="sxs-lookup"><span data-stu-id="13024-120">Int64</span></span>  | <span data-ttu-id="13024-121">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="13024-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="13024-122">android</span><span class="sxs-lookup"><span data-stu-id="13024-122">android</span></span>           | <span data-ttu-id="13024-123">Int64</span><span class="sxs-lookup"><span data-stu-id="13024-123">Int64</span></span>  | <span data-ttu-id="13024-124">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="13024-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="13024-125">ios</span><span class="sxs-lookup"><span data-stu-id="13024-125">ios</span></span>               | <span data-ttu-id="13024-126">Int64</span><span class="sxs-lookup"><span data-stu-id="13024-126">Int64</span></span>  | <span data-ttu-id="13024-127">IOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="13024-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="13024-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="13024-128">windows10Mobile</span></span>   | <span data-ttu-id="13024-129">Int64</span><span class="sxs-lookup"><span data-stu-id="13024-129">Int64</span></span>  | <span data-ttu-id="13024-130">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="13024-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13024-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13024-131">JSON representation</span></span>

<span data-ttu-id="13024-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13024-132">The following is a JSON representation of the resource.</span></span>

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
