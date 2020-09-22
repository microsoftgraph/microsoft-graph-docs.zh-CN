---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9f9dc76e287e6533b2b33606825a19da67d8675
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032486"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="c5336-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5336-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="c5336-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5336-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5336-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5336-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5336-106">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="c5336-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="c5336-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5336-107">Properties</span></span>
|<span data-ttu-id="c5336-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5336-108">Property</span></span>|<span data-ttu-id="c5336-109">类型</span><span class="sxs-lookup"><span data-stu-id="c5336-109">Type</span></span>|<span data-ttu-id="c5336-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5336-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5336-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="c5336-111">v8_0</span></span>|<span data-ttu-id="c5336-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="c5336-112">Boolean</span></span>|<span data-ttu-id="c5336-113">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="c5336-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="c5336-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="c5336-114">v8_1</span></span>|<span data-ttu-id="c5336-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="c5336-115">Boolean</span></span>|<span data-ttu-id="c5336-116">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="c5336-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="c5336-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="c5336-117">v10_0</span></span>|<span data-ttu-id="c5336-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="c5336-118">Boolean</span></span>|<span data-ttu-id="c5336-119">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="c5336-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5336-120">关系</span><span class="sxs-lookup"><span data-stu-id="c5336-120">Relationships</span></span>
<span data-ttu-id="c5336-121">无</span><span class="sxs-lookup"><span data-stu-id="c5336-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5336-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5336-122">JSON Representation</span></span>
<span data-ttu-id="c5336-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5336-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```









