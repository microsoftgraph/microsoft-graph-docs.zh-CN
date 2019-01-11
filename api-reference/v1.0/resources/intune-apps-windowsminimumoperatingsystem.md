---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d80a7c957b4a03132b349ebd609e21481322021a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863789"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="5c763-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c763-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="5c763-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c763-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c763-105">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="5c763-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="5c763-106">属性</span><span class="sxs-lookup"><span data-stu-id="5c763-106">Properties</span></span>
|<span data-ttu-id="5c763-107">属性</span><span class="sxs-lookup"><span data-stu-id="5c763-107">Property</span></span>|<span data-ttu-id="5c763-108">类型</span><span class="sxs-lookup"><span data-stu-id="5c763-108">Type</span></span>|<span data-ttu-id="5c763-109">说明</span><span class="sxs-lookup"><span data-stu-id="5c763-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c763-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="5c763-110">v8_0</span></span>|<span data-ttu-id="5c763-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c763-111">Boolean</span></span>|<span data-ttu-id="5c763-112">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="5c763-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="5c763-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="5c763-113">v8_1</span></span>|<span data-ttu-id="5c763-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c763-114">Boolean</span></span>|<span data-ttu-id="5c763-115">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="5c763-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="5c763-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="5c763-116">v10_0</span></span>|<span data-ttu-id="5c763-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="5c763-117">Boolean</span></span>|<span data-ttu-id="5c763-118">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="5c763-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c763-119">关系</span><span class="sxs-lookup"><span data-stu-id="5c763-119">Relationships</span></span>
<span data-ttu-id="5c763-120">无</span><span class="sxs-lookup"><span data-stu-id="5c763-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c763-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c763-121">JSON Representation</span></span>
<span data-ttu-id="5c763-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c763-122">Here is a JSON representation of the resource.</span></span>
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



