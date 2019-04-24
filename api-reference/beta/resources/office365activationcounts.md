---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505464"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="5be5d-103">office365ActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5be5d-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5be5d-104">属性</span><span class="sxs-lookup"><span data-stu-id="5be5d-104">Properties</span></span>

| <span data-ttu-id="5be5d-105">属性</span><span class="sxs-lookup"><span data-stu-id="5be5d-105">Property</span></span>          | <span data-ttu-id="5be5d-106">类型</span><span class="sxs-lookup"><span data-stu-id="5be5d-106">Type</span></span>   | <span data-ttu-id="5be5d-107">说明</span><span class="sxs-lookup"><span data-stu-id="5be5d-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="5be5d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5be5d-108">reportRefreshDate</span></span> | <span data-ttu-id="5be5d-109">Date</span><span class="sxs-lookup"><span data-stu-id="5be5d-109">Date</span></span>   | <span data-ttu-id="5be5d-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="5be5d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="5be5d-111">productType</span><span class="sxs-lookup"><span data-stu-id="5be5d-111">productType</span></span>       | <span data-ttu-id="5be5d-112">字符串</span><span class="sxs-lookup"><span data-stu-id="5be5d-112">String</span></span> | <span data-ttu-id="5be5d-113">产品类型, 如 "office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="5be5d-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="5be5d-114">时间</span><span class="sxs-lookup"><span data-stu-id="5be5d-114">windows</span></span>           | <span data-ttu-id="5be5d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5be5d-115">Int64</span></span>  | <span data-ttu-id="5be5d-116">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="5be5d-116">The activation count on Windows.</span></span> <span data-ttu-id="5be5d-117">此数字包括任何 Windows 计算机上的每次激活。</span><span class="sxs-lookup"><span data-stu-id="5be5d-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="5be5d-118">mac</span><span class="sxs-lookup"><span data-stu-id="5be5d-118">mac</span></span>               | <span data-ttu-id="5be5d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5be5d-119">Int64</span></span>  | <span data-ttu-id="5be5d-120">Mac OS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="5be5d-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="5be5d-121">android</span><span class="sxs-lookup"><span data-stu-id="5be5d-121">android</span></span>           | <span data-ttu-id="5be5d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5be5d-122">Int64</span></span>  | <span data-ttu-id="5be5d-123">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="5be5d-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="5be5d-124">ios</span><span class="sxs-lookup"><span data-stu-id="5be5d-124">ios</span></span>               | <span data-ttu-id="5be5d-125">Int64</span><span class="sxs-lookup"><span data-stu-id="5be5d-125">Int64</span></span>  | <span data-ttu-id="5be5d-126">iOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="5be5d-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="5be5d-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="5be5d-127">windows10Mobile</span></span>   | <span data-ttu-id="5be5d-128">Int64</span><span class="sxs-lookup"><span data-stu-id="5be5d-128">Int64</span></span>  | <span data-ttu-id="5be5d-129">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="5be5d-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5be5d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5be5d-130">JSON representation</span></span>

<span data-ttu-id="5be5d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5be5d-131">The following is a JSON representation of the resource.</span></span>

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
