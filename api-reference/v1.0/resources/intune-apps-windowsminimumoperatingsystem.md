---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd61874b0b7149c718ba790b2cdee23912a0a832
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439584"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="32cd5-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="32cd5-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="32cd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32cd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32cd5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32cd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32cd5-106">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="32cd5-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="32cd5-107">属性</span><span class="sxs-lookup"><span data-stu-id="32cd5-107">Properties</span></span>
|<span data-ttu-id="32cd5-108">属性</span><span class="sxs-lookup"><span data-stu-id="32cd5-108">Property</span></span>|<span data-ttu-id="32cd5-109">类型</span><span class="sxs-lookup"><span data-stu-id="32cd5-109">Type</span></span>|<span data-ttu-id="32cd5-110">说明</span><span class="sxs-lookup"><span data-stu-id="32cd5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32cd5-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="32cd5-111">v8_0</span></span>|<span data-ttu-id="32cd5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cd5-112">Boolean</span></span>|<span data-ttu-id="32cd5-113">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="32cd5-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="32cd5-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="32cd5-114">v8_1</span></span>|<span data-ttu-id="32cd5-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="32cd5-115">Boolean</span></span>|<span data-ttu-id="32cd5-116">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="32cd5-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="32cd5-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="32cd5-117">v10_0</span></span>|<span data-ttu-id="32cd5-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="32cd5-118">Boolean</span></span>|<span data-ttu-id="32cd5-119">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="32cd5-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32cd5-120">关系</span><span class="sxs-lookup"><span data-stu-id="32cd5-120">Relationships</span></span>
<span data-ttu-id="32cd5-121">无</span><span class="sxs-lookup"><span data-stu-id="32cd5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32cd5-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32cd5-122">JSON Representation</span></span>
<span data-ttu-id="32cd5-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32cd5-123">Here is a JSON representation of the resource.</span></span>
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







