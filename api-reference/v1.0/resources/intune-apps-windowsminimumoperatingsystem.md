---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: tfitzmac
ms.openlocfilehash: ea1953bd0d58d4e578ffb7171fc157166072189b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314726"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="7e4ab-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e4ab-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="7e4ab-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7e4ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e4ab-105">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="7e4ab-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="7e4ab-106">属性</span><span class="sxs-lookup"><span data-stu-id="7e4ab-106">Properties</span></span>
|<span data-ttu-id="7e4ab-107">属性</span><span class="sxs-lookup"><span data-stu-id="7e4ab-107">Property</span></span>|<span data-ttu-id="7e4ab-108">类型</span><span class="sxs-lookup"><span data-stu-id="7e4ab-108">Type</span></span>|<span data-ttu-id="7e4ab-109">说明</span><span class="sxs-lookup"><span data-stu-id="7e4ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e4ab-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="7e4ab-110">v8_0</span></span>|<span data-ttu-id="7e4ab-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="7e4ab-111">Boolean</span></span>|<span data-ttu-id="7e4ab-112">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="7e4ab-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="7e4ab-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="7e4ab-113">v8_1</span></span>|<span data-ttu-id="7e4ab-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="7e4ab-114">Boolean</span></span>|<span data-ttu-id="7e4ab-115">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="7e4ab-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="7e4ab-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="7e4ab-116">v10_0</span></span>|<span data-ttu-id="7e4ab-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="7e4ab-117">Boolean</span></span>|<span data-ttu-id="7e4ab-118">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="7e4ab-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e4ab-119">关系</span><span class="sxs-lookup"><span data-stu-id="7e4ab-119">Relationships</span></span>
<span data-ttu-id="7e4ab-120">无</span><span class="sxs-lookup"><span data-stu-id="7e4ab-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e4ab-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e4ab-121">JSON Representation</span></span>
<span data-ttu-id="7e4ab-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e4ab-122">Here is a JSON representation of the resource.</span></span>
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



