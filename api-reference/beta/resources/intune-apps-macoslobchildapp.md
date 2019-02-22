---
title: macOSLobChildApp 资源类型
description: 包含捆绑包包中的 MacOS LOB 应用程序的属性
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4bf8a8715bb681d1737a2fb1b39e5bac61fb9d7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146996"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="e18a1-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e18a1-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="e18a1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e18a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e18a1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e18a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e18a1-106">包含捆绑包包中的 MacOS LOB 应用程序的属性</span><span class="sxs-lookup"><span data-stu-id="e18a1-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="e18a1-107">属性</span><span class="sxs-lookup"><span data-stu-id="e18a1-107">Properties</span></span>
|<span data-ttu-id="e18a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="e18a1-108">Property</span></span>|<span data-ttu-id="e18a1-109">类型</span><span class="sxs-lookup"><span data-stu-id="e18a1-109">Type</span></span>|<span data-ttu-id="e18a1-110">说明</span><span class="sxs-lookup"><span data-stu-id="e18a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e18a1-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="e18a1-111">bundleId</span></span>|<span data-ttu-id="e18a1-112">String</span><span class="sxs-lookup"><span data-stu-id="e18a1-112">String</span></span>|<span data-ttu-id="e18a1-113">标识名称。</span><span class="sxs-lookup"><span data-stu-id="e18a1-113">The Identity Name.</span></span>|
|<span data-ttu-id="e18a1-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e18a1-114">buildNumber</span></span>|<span data-ttu-id="e18a1-115">String</span><span class="sxs-lookup"><span data-stu-id="e18a1-115">String</span></span>|<span data-ttu-id="e18a1-116">MacOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="e18a1-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e18a1-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e18a1-117">versionNumber</span></span>|<span data-ttu-id="e18a1-118">String</span><span class="sxs-lookup"><span data-stu-id="e18a1-118">String</span></span>|<span data-ttu-id="e18a1-119">MacOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="e18a1-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e18a1-120">关系</span><span class="sxs-lookup"><span data-stu-id="e18a1-120">Relationships</span></span>
<span data-ttu-id="e18a1-121">无</span><span class="sxs-lookup"><span data-stu-id="e18a1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e18a1-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e18a1-122">JSON Representation</span></span>
<span data-ttu-id="e18a1-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e18a1-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




