---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858378"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="38438-103">skypeForBusinessDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="38438-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="38438-104">属性</span><span class="sxs-lookup"><span data-stu-id="38438-104">Properties</span></span>

| <span data-ttu-id="38438-105">属性</span><span class="sxs-lookup"><span data-stu-id="38438-105">Property</span></span>          | <span data-ttu-id="38438-106">类型</span><span class="sxs-lookup"><span data-stu-id="38438-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="38438-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="38438-107">reportRefreshDate</span></span> | <span data-ttu-id="38438-108">日期</span><span class="sxs-lookup"><span data-stu-id="38438-108">Date</span></span>    |
| <span data-ttu-id="38438-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38438-109">userPrincipalName</span></span> | <span data-ttu-id="38438-110">字符串</span><span class="sxs-lookup"><span data-stu-id="38438-110">String</span></span>  |
| <span data-ttu-id="38438-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="38438-111">lastActivityDate</span></span>  | <span data-ttu-id="38438-112">日期</span><span class="sxs-lookup"><span data-stu-id="38438-112">Date</span></span>    |
| <span data-ttu-id="38438-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="38438-113">usedWindows</span></span>       | <span data-ttu-id="38438-114">布尔</span><span class="sxs-lookup"><span data-stu-id="38438-114">Boolean</span></span> |
| <span data-ttu-id="38438-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="38438-115">usedWindowsPhone</span></span>  | <span data-ttu-id="38438-116">布尔</span><span class="sxs-lookup"><span data-stu-id="38438-116">Boolean</span></span> |
| <span data-ttu-id="38438-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="38438-117">usedAndroidPhone</span></span>  | <span data-ttu-id="38438-118">布尔</span><span class="sxs-lookup"><span data-stu-id="38438-118">Boolean</span></span> |
| <span data-ttu-id="38438-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="38438-119">usediPhone</span></span>        | <span data-ttu-id="38438-120">布尔</span><span class="sxs-lookup"><span data-stu-id="38438-120">Boolean</span></span> |
| <span data-ttu-id="38438-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="38438-121">usediPad</span></span>          | <span data-ttu-id="38438-122">布尔</span><span class="sxs-lookup"><span data-stu-id="38438-122">Boolean</span></span> |
| <span data-ttu-id="38438-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="38438-123">reportPeriod</span></span>      | <span data-ttu-id="38438-124">String</span><span class="sxs-lookup"><span data-stu-id="38438-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="38438-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38438-125">JSON representation</span></span>

<span data-ttu-id="38438-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38438-126">The following is a JSON representation of the resource.</span></span>

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
