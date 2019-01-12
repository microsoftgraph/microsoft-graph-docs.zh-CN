---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 521b82448d58a831f88bdf9d548612aee86bcba6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972948"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="531d7-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="531d7-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="531d7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="531d7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="531d7-105">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="531d7-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="531d7-106">属性</span><span class="sxs-lookup"><span data-stu-id="531d7-106">Properties</span></span>
|<span data-ttu-id="531d7-107">属性</span><span class="sxs-lookup"><span data-stu-id="531d7-107">Property</span></span>|<span data-ttu-id="531d7-108">类型</span><span class="sxs-lookup"><span data-stu-id="531d7-108">Type</span></span>|<span data-ttu-id="531d7-109">说明</span><span class="sxs-lookup"><span data-stu-id="531d7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="531d7-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="531d7-110">v8_0</span></span>|<span data-ttu-id="531d7-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="531d7-111">Boolean</span></span>|<span data-ttu-id="531d7-112">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="531d7-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="531d7-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="531d7-113">v8_1</span></span>|<span data-ttu-id="531d7-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="531d7-114">Boolean</span></span>|<span data-ttu-id="531d7-115">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="531d7-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="531d7-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="531d7-116">v10_0</span></span>|<span data-ttu-id="531d7-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="531d7-117">Boolean</span></span>|<span data-ttu-id="531d7-118">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="531d7-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="531d7-119">关系</span><span class="sxs-lookup"><span data-stu-id="531d7-119">Relationships</span></span>
<span data-ttu-id="531d7-120">无</span><span class="sxs-lookup"><span data-stu-id="531d7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="531d7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="531d7-121">JSON Representation</span></span>
<span data-ttu-id="531d7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="531d7-122">Here is a JSON representation of the resource.</span></span>
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



