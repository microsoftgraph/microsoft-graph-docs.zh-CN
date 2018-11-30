---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: e53a979ac627735ef63a24e1823d83f4c9fe9f7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048092"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="7f202-103">office365ActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f202-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7f202-104">属性</span><span class="sxs-lookup"><span data-stu-id="7f202-104">Properties</span></span>

| <span data-ttu-id="7f202-105">属性</span><span class="sxs-lookup"><span data-stu-id="7f202-105">Property</span></span>          | <span data-ttu-id="7f202-106">类型</span><span class="sxs-lookup"><span data-stu-id="7f202-106">Type</span></span>   | <span data-ttu-id="7f202-107">说明</span><span class="sxs-lookup"><span data-stu-id="7f202-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="7f202-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7f202-108">reportRefreshDate</span></span> | <span data-ttu-id="7f202-109">日期</span><span class="sxs-lookup"><span data-stu-id="7f202-109">Date</span></span>   | <span data-ttu-id="7f202-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="7f202-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="7f202-111">productType</span><span class="sxs-lookup"><span data-stu-id="7f202-111">productType</span></span>       | <span data-ttu-id="7f202-112">字符串</span><span class="sxs-lookup"><span data-stu-id="7f202-112">String</span></span> | <span data-ttu-id="7f202-113">产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="7f202-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="7f202-114">windows</span><span class="sxs-lookup"><span data-stu-id="7f202-114">windows</span></span>           | <span data-ttu-id="7f202-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7f202-115">Int64</span></span>  | <span data-ttu-id="7f202-116">Windows 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="7f202-116">The activation count on Windows.</span></span> <span data-ttu-id="7f202-117">此数值包括 Windows 中的任何计算机上的每个激活。</span><span class="sxs-lookup"><span data-stu-id="7f202-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="7f202-118">mac</span><span class="sxs-lookup"><span data-stu-id="7f202-118">mac</span></span>               | <span data-ttu-id="7f202-119">Int64</span><span class="sxs-lookup"><span data-stu-id="7f202-119">Int64</span></span>  | <span data-ttu-id="7f202-120">Mac OS 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="7f202-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="7f202-121">android</span><span class="sxs-lookup"><span data-stu-id="7f202-121">android</span></span>           | <span data-ttu-id="7f202-122">Int64</span><span class="sxs-lookup"><span data-stu-id="7f202-122">Int64</span></span>  | <span data-ttu-id="7f202-123">在 Android 设备上激活计数。</span><span class="sxs-lookup"><span data-stu-id="7f202-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="7f202-124">ios</span><span class="sxs-lookup"><span data-stu-id="7f202-124">ios</span></span>               | <span data-ttu-id="7f202-125">Int64</span><span class="sxs-lookup"><span data-stu-id="7f202-125">Int64</span></span>  | <span data-ttu-id="7f202-126">在 iOS 激活计数。</span><span class="sxs-lookup"><span data-stu-id="7f202-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="7f202-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="7f202-127">windows10Mobile</span></span>   | <span data-ttu-id="7f202-128">Int64</span><span class="sxs-lookup"><span data-stu-id="7f202-128">Int64</span></span>  | <span data-ttu-id="7f202-129">在激活依靠 Windows 10 移动。</span><span class="sxs-lookup"><span data-stu-id="7f202-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7f202-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f202-130">JSON representation</span></span>

<span data-ttu-id="7f202-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f202-131">The following is a JSON representation of the resource.</span></span>

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
