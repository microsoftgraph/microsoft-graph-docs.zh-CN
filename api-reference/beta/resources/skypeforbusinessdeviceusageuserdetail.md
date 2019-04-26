---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555932"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="1467b-103">skypeForBusinessDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="1467b-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1467b-104">属性</span><span class="sxs-lookup"><span data-stu-id="1467b-104">Properties</span></span>

| <span data-ttu-id="1467b-105">属性</span><span class="sxs-lookup"><span data-stu-id="1467b-105">Property</span></span>          | <span data-ttu-id="1467b-106">类型</span><span class="sxs-lookup"><span data-stu-id="1467b-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="1467b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1467b-107">reportRefreshDate</span></span> | <span data-ttu-id="1467b-108">Date</span><span class="sxs-lookup"><span data-stu-id="1467b-108">Date</span></span>    |
| <span data-ttu-id="1467b-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1467b-109">userPrincipalName</span></span> | <span data-ttu-id="1467b-110">String</span><span class="sxs-lookup"><span data-stu-id="1467b-110">String</span></span>  |
| <span data-ttu-id="1467b-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1467b-111">lastActivityDate</span></span>  | <span data-ttu-id="1467b-112">Date</span><span class="sxs-lookup"><span data-stu-id="1467b-112">Date</span></span>    |
| <span data-ttu-id="1467b-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="1467b-113">usedWindows</span></span>       | <span data-ttu-id="1467b-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="1467b-114">Boolean</span></span> |
| <span data-ttu-id="1467b-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="1467b-115">usedWindowsPhone</span></span>  | <span data-ttu-id="1467b-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="1467b-116">Boolean</span></span> |
| <span data-ttu-id="1467b-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="1467b-117">usedAndroidPhone</span></span>  | <span data-ttu-id="1467b-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="1467b-118">Boolean</span></span> |
| <span data-ttu-id="1467b-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="1467b-119">usediPhone</span></span>        | <span data-ttu-id="1467b-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="1467b-120">Boolean</span></span> |
| <span data-ttu-id="1467b-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="1467b-121">usediPad</span></span>          | <span data-ttu-id="1467b-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="1467b-122">Boolean</span></span> |
| <span data-ttu-id="1467b-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1467b-123">reportPeriod</span></span>      | <span data-ttu-id="1467b-124">String</span><span class="sxs-lookup"><span data-stu-id="1467b-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1467b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1467b-125">JSON representation</span></span>

<span data-ttu-id="1467b-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1467b-126">The following is a JSON representation of the resource.</span></span>

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
