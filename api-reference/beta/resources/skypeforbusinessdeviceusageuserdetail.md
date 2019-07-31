---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b84cf9c7654354446fb7c6a5005befe3d17a0fa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964912"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="d5882-103">skypeForBusinessDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5882-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d5882-104">属性</span><span class="sxs-lookup"><span data-stu-id="d5882-104">Properties</span></span>

| <span data-ttu-id="d5882-105">属性</span><span class="sxs-lookup"><span data-stu-id="d5882-105">Property</span></span>          | <span data-ttu-id="d5882-106">类型</span><span class="sxs-lookup"><span data-stu-id="d5882-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="d5882-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d5882-107">reportRefreshDate</span></span> | <span data-ttu-id="d5882-108">日期</span><span class="sxs-lookup"><span data-stu-id="d5882-108">Date</span></span>    |
| <span data-ttu-id="d5882-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d5882-109">userPrincipalName</span></span> | <span data-ttu-id="d5882-110">String</span><span class="sxs-lookup"><span data-stu-id="d5882-110">String</span></span>  |
| <span data-ttu-id="d5882-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d5882-111">lastActivityDate</span></span>  | <span data-ttu-id="d5882-112">日期</span><span class="sxs-lookup"><span data-stu-id="d5882-112">Date</span></span>    |
| <span data-ttu-id="d5882-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="d5882-113">usedWindows</span></span>       | <span data-ttu-id="d5882-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5882-114">Boolean</span></span> |
| <span data-ttu-id="d5882-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="d5882-115">usedWindowsPhone</span></span>  | <span data-ttu-id="d5882-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5882-116">Boolean</span></span> |
| <span data-ttu-id="d5882-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="d5882-117">usedAndroidPhone</span></span>  | <span data-ttu-id="d5882-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5882-118">Boolean</span></span> |
| <span data-ttu-id="d5882-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="d5882-119">usediPhone</span></span>        | <span data-ttu-id="d5882-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5882-120">Boolean</span></span> |
| <span data-ttu-id="d5882-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="d5882-121">usediPad</span></span>          | <span data-ttu-id="d5882-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5882-122">Boolean</span></span> |
| <span data-ttu-id="d5882-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d5882-123">reportPeriod</span></span>      | <span data-ttu-id="d5882-124">String</span><span class="sxs-lookup"><span data-stu-id="d5882-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d5882-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5882-125">JSON representation</span></span>

<span data-ttu-id="d5882-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5882-126">The following is a JSON representation of the resource.</span></span>

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
