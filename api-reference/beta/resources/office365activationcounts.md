---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac3b6bb14b347f4ab273bbf65ce767f1ae6e1a2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983201"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="4f876-103">office365ActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f876-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="4f876-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f876-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="4f876-105">属性</span><span class="sxs-lookup"><span data-stu-id="4f876-105">Properties</span></span>

| <span data-ttu-id="4f876-106">属性</span><span class="sxs-lookup"><span data-stu-id="4f876-106">Property</span></span>          | <span data-ttu-id="4f876-107">类型</span><span class="sxs-lookup"><span data-stu-id="4f876-107">Type</span></span>   | <span data-ttu-id="4f876-108">说明</span><span class="sxs-lookup"><span data-stu-id="4f876-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="4f876-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4f876-109">reportRefreshDate</span></span> | <span data-ttu-id="4f876-110">日期</span><span class="sxs-lookup"><span data-stu-id="4f876-110">Date</span></span>   | <span data-ttu-id="4f876-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="4f876-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="4f876-112">productType</span><span class="sxs-lookup"><span data-stu-id="4f876-112">productType</span></span>       | <span data-ttu-id="4f876-113">String</span><span class="sxs-lookup"><span data-stu-id="4f876-113">String</span></span> | <span data-ttu-id="4f876-114">产品类型，例如"Microsoft 365 ProPlus"或"Project Client"。</span><span class="sxs-lookup"><span data-stu-id="4f876-114">The product type, such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="4f876-115">windows</span><span class="sxs-lookup"><span data-stu-id="4f876-115">windows</span></span>           | <span data-ttu-id="4f876-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4f876-116">Int64</span></span>  | <span data-ttu-id="4f876-117">Windows 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f876-117">The activation count on Windows.</span></span> <span data-ttu-id="4f876-118">此数字包括任何 Windows 计算机上每次激活。</span><span class="sxs-lookup"><span data-stu-id="4f876-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="4f876-119">mac</span><span class="sxs-lookup"><span data-stu-id="4f876-119">mac</span></span>               | <span data-ttu-id="4f876-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4f876-120">Int64</span></span>  | <span data-ttu-id="4f876-121">Mac 操作系统上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f876-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="4f876-122">android</span><span class="sxs-lookup"><span data-stu-id="4f876-122">android</span></span>           | <span data-ttu-id="4f876-123">Int64</span><span class="sxs-lookup"><span data-stu-id="4f876-123">Int64</span></span>  | <span data-ttu-id="4f876-124">Android 设备上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f876-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="4f876-125">ios</span><span class="sxs-lookup"><span data-stu-id="4f876-125">ios</span></span>               | <span data-ttu-id="4f876-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4f876-126">Int64</span></span>  | <span data-ttu-id="4f876-127">iOS 上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f876-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="4f876-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="4f876-128">windows10Mobile</span></span>   | <span data-ttu-id="4f876-129">Int64</span><span class="sxs-lookup"><span data-stu-id="4f876-129">Int64</span></span>  | <span data-ttu-id="4f876-130">Windows 10 移动版上的激活计数。</span><span class="sxs-lookup"><span data-stu-id="4f876-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f876-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f876-131">JSON representation</span></span>

<span data-ttu-id="4f876-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f876-132">The following is a JSON representation of the resource.</span></span>

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


