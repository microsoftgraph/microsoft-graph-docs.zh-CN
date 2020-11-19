---
title: macOSLobChildApp 资源类型
description: 包含捆绑包包中的 MacOS LOB 应用程序的属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b3c115e312333a448318fb718140f5b6e8305494
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281829"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="0e543-103">macOSLobChildApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e543-103">macOSLobChildApp resource type</span></span>

<span data-ttu-id="0e543-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e543-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e543-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e543-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e543-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e543-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e543-107">包含捆绑包包中的 MacOS LOB 应用程序的属性</span><span class="sxs-lookup"><span data-stu-id="0e543-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="0e543-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e543-108">Properties</span></span>
|<span data-ttu-id="0e543-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e543-109">Property</span></span>|<span data-ttu-id="0e543-110">类型</span><span class="sxs-lookup"><span data-stu-id="0e543-110">Type</span></span>|<span data-ttu-id="0e543-111">Description</span><span class="sxs-lookup"><span data-stu-id="0e543-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e543-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="0e543-112">bundleId</span></span>|<span data-ttu-id="0e543-113">String</span><span class="sxs-lookup"><span data-stu-id="0e543-113">String</span></span>|<span data-ttu-id="0e543-114">标识名称。</span><span class="sxs-lookup"><span data-stu-id="0e543-114">The Identity Name.</span></span>|
|<span data-ttu-id="0e543-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="0e543-115">buildNumber</span></span>|<span data-ttu-id="0e543-116">String</span><span class="sxs-lookup"><span data-stu-id="0e543-116">String</span></span>|<span data-ttu-id="0e543-117">MacOS 业务线 (LoB) 应用程序的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="0e543-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0e543-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="0e543-118">versionNumber</span></span>|<span data-ttu-id="0e543-119">String</span><span class="sxs-lookup"><span data-stu-id="0e543-119">String</span></span>|<span data-ttu-id="0e543-120">MacOS 业务线 (LoB) 应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="0e543-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e543-121">关系</span><span class="sxs-lookup"><span data-stu-id="0e543-121">Relationships</span></span>
<span data-ttu-id="0e543-122">无</span><span class="sxs-lookup"><span data-stu-id="0e543-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e543-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e543-123">JSON Representation</span></span>
<span data-ttu-id="0e543-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e543-124">Here is a JSON representation of the resource.</span></span>
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




