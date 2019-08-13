---
title: macOSLobChildApp 资源类型
description: 包含捆绑包包中的 MacOS LOB 应用程序的属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b665391a4e7832feea72302db9ffb49c98f69964
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365914"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="dc0b3-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc0b3-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="dc0b3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc0b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc0b3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc0b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc0b3-106">包含捆绑包包中的 MacOS LOB 应用程序的属性</span><span class="sxs-lookup"><span data-stu-id="dc0b3-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="dc0b3-107">属性</span><span class="sxs-lookup"><span data-stu-id="dc0b3-107">Properties</span></span>
|<span data-ttu-id="dc0b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc0b3-108">Property</span></span>|<span data-ttu-id="dc0b3-109">类型</span><span class="sxs-lookup"><span data-stu-id="dc0b3-109">Type</span></span>|<span data-ttu-id="dc0b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc0b3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc0b3-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="dc0b3-111">bundleId</span></span>|<span data-ttu-id="dc0b3-112">String</span><span class="sxs-lookup"><span data-stu-id="dc0b3-112">String</span></span>|<span data-ttu-id="dc0b3-113">标识名称。</span><span class="sxs-lookup"><span data-stu-id="dc0b3-113">The Identity Name.</span></span>|
|<span data-ttu-id="dc0b3-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="dc0b3-114">buildNumber</span></span>|<span data-ttu-id="dc0b3-115">String</span><span class="sxs-lookup"><span data-stu-id="dc0b3-115">String</span></span>|<span data-ttu-id="dc0b3-116">MacOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="dc0b3-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dc0b3-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="dc0b3-117">versionNumber</span></span>|<span data-ttu-id="dc0b3-118">String</span><span class="sxs-lookup"><span data-stu-id="dc0b3-118">String</span></span>|<span data-ttu-id="dc0b3-119">MacOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="dc0b3-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc0b3-120">关系</span><span class="sxs-lookup"><span data-stu-id="dc0b3-120">Relationships</span></span>
<span data-ttu-id="dc0b3-121">无</span><span class="sxs-lookup"><span data-stu-id="dc0b3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc0b3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc0b3-122">JSON Representation</span></span>
<span data-ttu-id="dc0b3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc0b3-123">Here is a JSON representation of the resource.</span></span>
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



