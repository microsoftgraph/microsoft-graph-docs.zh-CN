---
title: windowsKioskDesktopApp 资源类型
description: 一类应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cccd1b5e7ec7ca16aeb76b87fc31d90e92e7dcd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572080"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="69782-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="69782-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="69782-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69782-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69782-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69782-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69782-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="69782-106">The base class for a type of apps</span></span>


<span data-ttu-id="69782-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="69782-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69782-108">属性</span><span class="sxs-lookup"><span data-stu-id="69782-108">Properties</span></span>
|<span data-ttu-id="69782-109">属性</span><span class="sxs-lookup"><span data-stu-id="69782-109">Property</span></span>|<span data-ttu-id="69782-110">类型</span><span class="sxs-lookup"><span data-stu-id="69782-110">Type</span></span>|<span data-ttu-id="69782-111">说明</span><span class="sxs-lookup"><span data-stu-id="69782-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69782-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="69782-112">startLayoutTileSize</span></span>|[<span data-ttu-id="69782-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="69782-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="69782-114">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="69782-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="69782-115">可取值为：`hidden`、`small`、`medium`、`wide` 或 `large`。</span><span class="sxs-lookup"><span data-stu-id="69782-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="69782-116">name</span><span class="sxs-lookup"><span data-stu-id="69782-116">name</span></span>|<span data-ttu-id="69782-117">String</span><span class="sxs-lookup"><span data-stu-id="69782-117">String</span></span>|<span data-ttu-id="69782-118">表示从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="69782-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="69782-119">appType</span><span class="sxs-lookup"><span data-stu-id="69782-119">appType</span></span>|[<span data-ttu-id="69782-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="69782-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="69782-121">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="69782-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="69782-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="69782-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="69782-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="69782-123">autoLaunch</span></span>|<span data-ttu-id="69782-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="69782-124">Boolean</span></span>|<span data-ttu-id="69782-125">允许在从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="69782-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="69782-126">路径</span><span class="sxs-lookup"><span data-stu-id="69782-126">path</span></span>|<span data-ttu-id="69782-127">String</span><span class="sxs-lookup"><span data-stu-id="69782-127">String</span></span>|<span data-ttu-id="69782-128">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="69782-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="69782-129">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="69782-129">desktopApplicationId</span></span>|<span data-ttu-id="69782-130">String</span><span class="sxs-lookup"><span data-stu-id="69782-130">String</span></span>|<span data-ttu-id="69782-131">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="69782-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="69782-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="69782-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="69782-133">String</span><span class="sxs-lookup"><span data-stu-id="69782-133">String</span></span>|<span data-ttu-id="69782-134">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="69782-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="69782-135">关系</span><span class="sxs-lookup"><span data-stu-id="69782-135">Relationships</span></span>
<span data-ttu-id="69782-136">无</span><span class="sxs-lookup"><span data-stu-id="69782-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69782-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69782-137">JSON Representation</span></span>
<span data-ttu-id="69782-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69782-138">Here is a JSON representation of the resource.</span></span>
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




