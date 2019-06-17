---
title: macOSLobChildApp 资源类型
description: 包含捆绑包包中的 MacOS LOB 应用程序的属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46e84e629f7664f8a5ab33eaa9db6bbc95fd80bc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34957757"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="e6dcb-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6dcb-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="e6dcb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6dcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6dcb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6dcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6dcb-106">包含捆绑包包中的 MacOS LOB 应用程序的属性</span><span class="sxs-lookup"><span data-stu-id="e6dcb-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="e6dcb-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6dcb-107">Properties</span></span>
|<span data-ttu-id="e6dcb-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6dcb-108">Property</span></span>|<span data-ttu-id="e6dcb-109">类型</span><span class="sxs-lookup"><span data-stu-id="e6dcb-109">Type</span></span>|<span data-ttu-id="e6dcb-110">说明</span><span class="sxs-lookup"><span data-stu-id="e6dcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6dcb-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="e6dcb-111">bundleId</span></span>|<span data-ttu-id="e6dcb-112">String</span><span class="sxs-lookup"><span data-stu-id="e6dcb-112">String</span></span>|<span data-ttu-id="e6dcb-113">标识名称。</span><span class="sxs-lookup"><span data-stu-id="e6dcb-113">The Identity Name.</span></span>|
|<span data-ttu-id="e6dcb-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e6dcb-114">buildNumber</span></span>|<span data-ttu-id="e6dcb-115">String</span><span class="sxs-lookup"><span data-stu-id="e6dcb-115">String</span></span>|<span data-ttu-id="e6dcb-116">MacOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="e6dcb-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e6dcb-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e6dcb-117">versionNumber</span></span>|<span data-ttu-id="e6dcb-118">String</span><span class="sxs-lookup"><span data-stu-id="e6dcb-118">String</span></span>|<span data-ttu-id="e6dcb-119">MacOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="e6dcb-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6dcb-120">关系</span><span class="sxs-lookup"><span data-stu-id="e6dcb-120">Relationships</span></span>
<span data-ttu-id="e6dcb-121">无</span><span class="sxs-lookup"><span data-stu-id="e6dcb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6dcb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6dcb-122">JSON Representation</span></span>
<span data-ttu-id="e6dcb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6dcb-123">Here is a JSON representation of the resource.</span></span>
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





