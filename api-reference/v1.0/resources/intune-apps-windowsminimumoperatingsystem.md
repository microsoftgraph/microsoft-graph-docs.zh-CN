---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a92d02f6994a7cd18ba44c7da5b43768e87fc61a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032072"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="584fb-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="584fb-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="584fb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="584fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="584fb-105">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="584fb-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="584fb-106">属性</span><span class="sxs-lookup"><span data-stu-id="584fb-106">Properties</span></span>
|<span data-ttu-id="584fb-107">属性</span><span class="sxs-lookup"><span data-stu-id="584fb-107">Property</span></span>|<span data-ttu-id="584fb-108">类型</span><span class="sxs-lookup"><span data-stu-id="584fb-108">Type</span></span>|<span data-ttu-id="584fb-109">说明</span><span class="sxs-lookup"><span data-stu-id="584fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="584fb-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="584fb-110">v8_0</span></span>|<span data-ttu-id="584fb-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="584fb-111">Boolean</span></span>|<span data-ttu-id="584fb-112">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="584fb-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="584fb-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="584fb-113">v8_1</span></span>|<span data-ttu-id="584fb-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="584fb-114">Boolean</span></span>|<span data-ttu-id="584fb-115">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="584fb-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="584fb-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="584fb-116">v10_0</span></span>|<span data-ttu-id="584fb-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="584fb-117">Boolean</span></span>|<span data-ttu-id="584fb-118">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="584fb-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="584fb-119">关系</span><span class="sxs-lookup"><span data-stu-id="584fb-119">Relationships</span></span>
<span data-ttu-id="584fb-120">无</span><span class="sxs-lookup"><span data-stu-id="584fb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="584fb-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="584fb-121">JSON Representation</span></span>
<span data-ttu-id="584fb-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="584fb-122">Here is a JSON representation of the resource.</span></span>
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



