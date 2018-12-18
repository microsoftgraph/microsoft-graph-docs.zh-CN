---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
ms.openlocfilehash: 1947b66a59190945e5a6b823b47ef8df7d02683a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328999"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="84b58-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="84b58-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="84b58-104">属性</span><span class="sxs-lookup"><span data-stu-id="84b58-104">Properties</span></span>

| <span data-ttu-id="84b58-105">属性</span><span class="sxs-lookup"><span data-stu-id="84b58-105">Property</span></span>          | <span data-ttu-id="84b58-106">类型</span><span class="sxs-lookup"><span data-stu-id="84b58-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="84b58-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="84b58-107">reportRefreshDate</span></span> | <span data-ttu-id="84b58-108">日期</span><span class="sxs-lookup"><span data-stu-id="84b58-108">Date</span></span>    |
| <span data-ttu-id="84b58-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84b58-109">userPrincipalName</span></span> | <span data-ttu-id="84b58-110">字符串</span><span class="sxs-lookup"><span data-stu-id="84b58-110">String</span></span>  |
| <span data-ttu-id="84b58-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="84b58-111">lastActivityDate</span></span>  | <span data-ttu-id="84b58-112">日期</span><span class="sxs-lookup"><span data-stu-id="84b58-112">Date</span></span>    |
| <span data-ttu-id="84b58-113">被</span><span class="sxs-lookup"><span data-stu-id="84b58-113">isDeleted</span></span>         | <span data-ttu-id="84b58-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b58-114">Boolean</span></span> |
| <span data-ttu-id="84b58-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="84b58-115">deletedDate</span></span>       | <span data-ttu-id="84b58-116">日期</span><span class="sxs-lookup"><span data-stu-id="84b58-116">Date</span></span>    |
| <span data-ttu-id="84b58-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="84b58-117">usedWeb</span></span>           | <span data-ttu-id="84b58-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b58-118">Boolean</span></span> |
| <span data-ttu-id="84b58-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="84b58-119">usedWindowsPhone</span></span>  | <span data-ttu-id="84b58-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b58-120">Boolean</span></span> |
| <span data-ttu-id="84b58-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="84b58-121">usediOS</span></span>           | <span data-ttu-id="84b58-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b58-122">Boolean</span></span> |
| <span data-ttu-id="84b58-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="84b58-123">usedMac</span></span>           | <span data-ttu-id="84b58-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b58-124">Boolean</span></span> |
| <span data-ttu-id="84b58-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="84b58-125">usedAndroidPhone</span></span>  | <span data-ttu-id="84b58-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b58-126">Boolean</span></span> |
| <span data-ttu-id="84b58-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="84b58-127">usedWindows</span></span>       | <span data-ttu-id="84b58-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b58-128">Boolean</span></span> |
| <span data-ttu-id="84b58-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="84b58-129">reportPeriod</span></span>      | <span data-ttu-id="84b58-130">String</span><span class="sxs-lookup"><span data-stu-id="84b58-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="84b58-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84b58-131">JSON representation</span></span>

<span data-ttu-id="84b58-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84b58-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
