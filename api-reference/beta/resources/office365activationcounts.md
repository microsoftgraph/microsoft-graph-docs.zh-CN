---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4787672df6462e8d1f343e4dace43ede7c79ff37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991179"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="2fa94-103">office365ActivationCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fa94-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2fa94-104">属性</span><span class="sxs-lookup"><span data-stu-id="2fa94-104">Properties</span></span>

| <span data-ttu-id="2fa94-105">属性</span><span class="sxs-lookup"><span data-stu-id="2fa94-105">Property</span></span>          | <span data-ttu-id="2fa94-106">类型</span><span class="sxs-lookup"><span data-stu-id="2fa94-106">Type</span></span>   | <span data-ttu-id="2fa94-107">说明</span><span class="sxs-lookup"><span data-stu-id="2fa94-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2fa94-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2fa94-108">reportRefreshDate</span></span> | <span data-ttu-id="2fa94-109">日期</span><span class="sxs-lookup"><span data-stu-id="2fa94-109">Date</span></span>   | <span data-ttu-id="2fa94-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="2fa94-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2fa94-111">productType</span><span class="sxs-lookup"><span data-stu-id="2fa94-111">productType</span></span>       | <span data-ttu-id="2fa94-112">字符串</span><span class="sxs-lookup"><span data-stu-id="2fa94-112">String</span></span> | <span data-ttu-id="2fa94-113">产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="2fa94-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="2fa94-114">windows</span><span class="sxs-lookup"><span data-stu-id="2fa94-114">windows</span></span>           | <span data-ttu-id="2fa94-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2fa94-115">Int64</span></span>  | <span data-ttu-id="2fa94-116">Windows 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="2fa94-116">The activation count on Windows.</span></span> <span data-ttu-id="2fa94-117">此数值包括 Windows 中的任何计算机上的每个激活。</span><span class="sxs-lookup"><span data-stu-id="2fa94-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="2fa94-118">mac</span><span class="sxs-lookup"><span data-stu-id="2fa94-118">mac</span></span>               | <span data-ttu-id="2fa94-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2fa94-119">Int64</span></span>  | <span data-ttu-id="2fa94-120">Mac OS 上激活计数。</span><span class="sxs-lookup"><span data-stu-id="2fa94-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="2fa94-121">android</span><span class="sxs-lookup"><span data-stu-id="2fa94-121">android</span></span>           | <span data-ttu-id="2fa94-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2fa94-122">Int64</span></span>  | <span data-ttu-id="2fa94-123">在 Android 设备上激活计数。</span><span class="sxs-lookup"><span data-stu-id="2fa94-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="2fa94-124">ios</span><span class="sxs-lookup"><span data-stu-id="2fa94-124">ios</span></span>               | <span data-ttu-id="2fa94-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2fa94-125">Int64</span></span>  | <span data-ttu-id="2fa94-126">在 iOS 激活计数。</span><span class="sxs-lookup"><span data-stu-id="2fa94-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="2fa94-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="2fa94-127">windows10Mobile</span></span>   | <span data-ttu-id="2fa94-128">Int64</span><span class="sxs-lookup"><span data-stu-id="2fa94-128">Int64</span></span>  | <span data-ttu-id="2fa94-129">在激活依靠 Windows 10 移动。</span><span class="sxs-lookup"><span data-stu-id="2fa94-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2fa94-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fa94-130">JSON representation</span></span>

<span data-ttu-id="2fa94-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fa94-131">The following is a JSON representation of the resource.</span></span>

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
