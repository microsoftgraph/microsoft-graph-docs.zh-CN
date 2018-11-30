---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: b62920d124fd52e0f653c128eeb0956cdfe0c680
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043046"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="adfe9-103">skypeForBusinessDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="adfe9-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="adfe9-104">属性</span><span class="sxs-lookup"><span data-stu-id="adfe9-104">Properties</span></span>

| <span data-ttu-id="adfe9-105">属性</span><span class="sxs-lookup"><span data-stu-id="adfe9-105">Property</span></span>          | <span data-ttu-id="adfe9-106">类型</span><span class="sxs-lookup"><span data-stu-id="adfe9-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="adfe9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="adfe9-107">reportRefreshDate</span></span> | <span data-ttu-id="adfe9-108">日期</span><span class="sxs-lookup"><span data-stu-id="adfe9-108">Date</span></span>    |
| <span data-ttu-id="adfe9-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="adfe9-109">userPrincipalName</span></span> | <span data-ttu-id="adfe9-110">字符串</span><span class="sxs-lookup"><span data-stu-id="adfe9-110">String</span></span>  |
| <span data-ttu-id="adfe9-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="adfe9-111">lastActivityDate</span></span>  | <span data-ttu-id="adfe9-112">日期</span><span class="sxs-lookup"><span data-stu-id="adfe9-112">Date</span></span>    |
| <span data-ttu-id="adfe9-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="adfe9-113">usedWindows</span></span>       | <span data-ttu-id="adfe9-114">布尔</span><span class="sxs-lookup"><span data-stu-id="adfe9-114">Boolean</span></span> |
| <span data-ttu-id="adfe9-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="adfe9-115">usedWindowsPhone</span></span>  | <span data-ttu-id="adfe9-116">布尔</span><span class="sxs-lookup"><span data-stu-id="adfe9-116">Boolean</span></span> |
| <span data-ttu-id="adfe9-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="adfe9-117">usedAndroidPhone</span></span>  | <span data-ttu-id="adfe9-118">布尔</span><span class="sxs-lookup"><span data-stu-id="adfe9-118">Boolean</span></span> |
| <span data-ttu-id="adfe9-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="adfe9-119">usediPhone</span></span>        | <span data-ttu-id="adfe9-120">布尔</span><span class="sxs-lookup"><span data-stu-id="adfe9-120">Boolean</span></span> |
| <span data-ttu-id="adfe9-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="adfe9-121">usediPad</span></span>          | <span data-ttu-id="adfe9-122">布尔</span><span class="sxs-lookup"><span data-stu-id="adfe9-122">Boolean</span></span> |
| <span data-ttu-id="adfe9-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="adfe9-123">reportPeriod</span></span>      | <span data-ttu-id="adfe9-124">String</span><span class="sxs-lookup"><span data-stu-id="adfe9-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="adfe9-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adfe9-125">JSON representation</span></span>

<span data-ttu-id="adfe9-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adfe9-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
