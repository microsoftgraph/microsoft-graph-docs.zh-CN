---
title: windowsKioskSingleWin32App 资源类型
description: 用于标识展台 win32 配置的单个应用配置的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fefde9fa13849a910c56e4ebaed870ebb9edac62
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446698"
---
# <a name="windowskiosksinglewin32app-resource-type"></a><span data-ttu-id="924fa-103">windowsKioskSingleWin32App 资源类型</span><span class="sxs-lookup"><span data-stu-id="924fa-103">windowsKioskSingleWin32App resource type</span></span>

<span data-ttu-id="924fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="924fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="924fa-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="924fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="924fa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="924fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="924fa-107">用于标识展台 win32 配置的单个应用配置的类</span><span class="sxs-lookup"><span data-stu-id="924fa-107">The class used to identify the single app configuration for the kiosk win32 configuration</span></span>


<span data-ttu-id="924fa-108">继承自 [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="924fa-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="924fa-109">属性</span><span class="sxs-lookup"><span data-stu-id="924fa-109">Properties</span></span>
|<span data-ttu-id="924fa-110">属性</span><span class="sxs-lookup"><span data-stu-id="924fa-110">Property</span></span>|<span data-ttu-id="924fa-111">类型</span><span class="sxs-lookup"><span data-stu-id="924fa-111">Type</span></span>|<span data-ttu-id="924fa-112">说明</span><span class="sxs-lookup"><span data-stu-id="924fa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="924fa-113">win32App</span><span class="sxs-lookup"><span data-stu-id="924fa-113">win32App</span></span>|[<span data-ttu-id="924fa-114">windowsKioskWin32App</span><span class="sxs-lookup"><span data-stu-id="924fa-114">windowsKioskWin32App</span></span>](../resources/intune-deviceconfig-windowskioskwin32app.md)|<span data-ttu-id="924fa-115">这是 win32 应用，可在展台模式下启动使用</span><span class="sxs-lookup"><span data-stu-id="924fa-115">This is the win32 app that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="924fa-116">关系</span><span class="sxs-lookup"><span data-stu-id="924fa-116">Relationships</span></span>
<span data-ttu-id="924fa-117">无</span><span class="sxs-lookup"><span data-stu-id="924fa-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="924fa-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="924fa-118">JSON Representation</span></span>
<span data-ttu-id="924fa-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="924fa-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleWin32App",
  "win32App": {
    "@odata.type": "microsoft.graph.windowsKioskWin32App",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "classicAppPath": "String",
    "edgeNoFirstRun": true,
    "edgeKioskIdleTimeoutMinutes": 1024,
    "edgeKioskType": "String",
    "edgeKiosk": "String"
  }
}
```




