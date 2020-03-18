---
title: windowsKioskDesktopApp 资源类型
description: 一类应用程序的基类
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f940a656395a58df4487648a2090455b97d1647b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786389"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="f8389-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8389-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="f8389-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8389-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8389-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8389-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8389-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="f8389-106">The base class for a type of apps</span></span>


<span data-ttu-id="f8389-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="f8389-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8389-108">属性</span><span class="sxs-lookup"><span data-stu-id="f8389-108">Properties</span></span>
|<span data-ttu-id="f8389-109">属性</span><span class="sxs-lookup"><span data-stu-id="f8389-109">Property</span></span>|<span data-ttu-id="f8389-110">类型</span><span class="sxs-lookup"><span data-stu-id="f8389-110">Type</span></span>|<span data-ttu-id="f8389-111">说明</span><span class="sxs-lookup"><span data-stu-id="f8389-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8389-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f8389-112">startLayoutTileSize</span></span>|[<span data-ttu-id="f8389-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f8389-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="f8389-114">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="f8389-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f8389-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="f8389-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="f8389-116">name</span><span class="sxs-lookup"><span data-stu-id="f8389-116">name</span></span>|<span data-ttu-id="f8389-117">String</span><span class="sxs-lookup"><span data-stu-id="f8389-117">String</span></span>|<span data-ttu-id="f8389-118">表示从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="f8389-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f8389-119">appType</span><span class="sxs-lookup"><span data-stu-id="f8389-119">appType</span></span>|[<span data-ttu-id="f8389-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="f8389-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="f8389-121">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="f8389-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f8389-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="f8389-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="f8389-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="f8389-123">autoLaunch</span></span>|<span data-ttu-id="f8389-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="f8389-124">Boolean</span></span>|<span data-ttu-id="f8389-125">允许在从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="f8389-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f8389-126">路径</span><span class="sxs-lookup"><span data-stu-id="f8389-126">path</span></span>|<span data-ttu-id="f8389-127">String</span><span class="sxs-lookup"><span data-stu-id="f8389-127">String</span></span>|<span data-ttu-id="f8389-128">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="f8389-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="f8389-129">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="f8389-129">desktopApplicationId</span></span>|<span data-ttu-id="f8389-130">String</span><span class="sxs-lookup"><span data-stu-id="f8389-130">String</span></span>|<span data-ttu-id="f8389-131">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="f8389-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="f8389-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f8389-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="f8389-133">String</span><span class="sxs-lookup"><span data-stu-id="f8389-133">String</span></span>|<span data-ttu-id="f8389-134">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f8389-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8389-135">关系</span><span class="sxs-lookup"><span data-stu-id="f8389-135">Relationships</span></span>
<span data-ttu-id="f8389-136">无</span><span class="sxs-lookup"><span data-stu-id="f8389-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8389-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8389-137">JSON Representation</span></span>
<span data-ttu-id="f8389-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8389-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```



