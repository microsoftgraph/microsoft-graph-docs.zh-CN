---
title: macOSLobChildApp 资源类型
description: 包含捆绑包包中的 MacOS LOB 应用程序的属性
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a74d40582806fb4f574cb80beaff2db0abac0caa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798040"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="e5c9b-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5c9b-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="e5c9b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5c9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5c9b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5c9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5c9b-106">包含捆绑包包中的 MacOS LOB 应用程序的属性</span><span class="sxs-lookup"><span data-stu-id="e5c9b-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="e5c9b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5c9b-107">Properties</span></span>
|<span data-ttu-id="e5c9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5c9b-108">Property</span></span>|<span data-ttu-id="e5c9b-109">类型</span><span class="sxs-lookup"><span data-stu-id="e5c9b-109">Type</span></span>|<span data-ttu-id="e5c9b-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5c9b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5c9b-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="e5c9b-111">bundleId</span></span>|<span data-ttu-id="e5c9b-112">String</span><span class="sxs-lookup"><span data-stu-id="e5c9b-112">String</span></span>|<span data-ttu-id="e5c9b-113">标识名称。</span><span class="sxs-lookup"><span data-stu-id="e5c9b-113">The Identity Name.</span></span>|
|<span data-ttu-id="e5c9b-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e5c9b-114">buildNumber</span></span>|<span data-ttu-id="e5c9b-115">String</span><span class="sxs-lookup"><span data-stu-id="e5c9b-115">String</span></span>|<span data-ttu-id="e5c9b-116">MacOS 业务线（LoB）应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="e5c9b-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e5c9b-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e5c9b-117">versionNumber</span></span>|<span data-ttu-id="e5c9b-118">String</span><span class="sxs-lookup"><span data-stu-id="e5c9b-118">String</span></span>|<span data-ttu-id="e5c9b-119">MacOS 业务线（LoB）应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="e5c9b-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5c9b-120">关系</span><span class="sxs-lookup"><span data-stu-id="e5c9b-120">Relationships</span></span>
<span data-ttu-id="e5c9b-121">无</span><span class="sxs-lookup"><span data-stu-id="e5c9b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5c9b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5c9b-122">JSON Representation</span></span>
<span data-ttu-id="e5c9b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5c9b-123">Here is a JSON representation of the resource.</span></span>
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



