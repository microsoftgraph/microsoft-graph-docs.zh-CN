---
title: windowsKioskDesktopApp 资源类型
description: 一类应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89f309b53e44b0f2843145dd7c0f4d3ffa6d7f98
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805213"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="d5b85-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5b85-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="d5b85-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5b85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5b85-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5b85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b85-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="d5b85-106">The base class for a type of apps</span></span>


<span data-ttu-id="d5b85-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="d5b85-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5b85-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5b85-108">Properties</span></span>
|<span data-ttu-id="d5b85-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5b85-109">Property</span></span>|<span data-ttu-id="d5b85-110">类型</span><span class="sxs-lookup"><span data-stu-id="d5b85-110">Type</span></span>|<span data-ttu-id="d5b85-111">说明</span><span class="sxs-lookup"><span data-stu-id="d5b85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b85-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="d5b85-112">startLayoutTileSize</span></span>|[<span data-ttu-id="d5b85-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="d5b85-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="d5b85-114">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="d5b85-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="d5b85-115">可取值为：`hidden`、`small`、`medium`、`wide` 或 `large`。</span><span class="sxs-lookup"><span data-stu-id="d5b85-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="d5b85-116">name</span><span class="sxs-lookup"><span data-stu-id="d5b85-116">name</span></span>|<span data-ttu-id="d5b85-117">String</span><span class="sxs-lookup"><span data-stu-id="d5b85-117">String</span></span>|<span data-ttu-id="d5b85-118">表示从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="d5b85-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="d5b85-119">appType</span><span class="sxs-lookup"><span data-stu-id="d5b85-119">appType</span></span>|[<span data-ttu-id="d5b85-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="d5b85-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="d5b85-121">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="d5b85-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="d5b85-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="d5b85-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="d5b85-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="d5b85-123">autoLaunch</span></span>|<span data-ttu-id="d5b85-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="d5b85-124">Boolean</span></span>|<span data-ttu-id="d5b85-125">允许在从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="d5b85-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="d5b85-126">路径</span><span class="sxs-lookup"><span data-stu-id="d5b85-126">path</span></span>|<span data-ttu-id="d5b85-127">String</span><span class="sxs-lookup"><span data-stu-id="d5b85-127">String</span></span>|<span data-ttu-id="d5b85-128">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="d5b85-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="d5b85-129">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="d5b85-129">desktopApplicationId</span></span>|<span data-ttu-id="d5b85-130">String</span><span class="sxs-lookup"><span data-stu-id="d5b85-130">String</span></span>|<span data-ttu-id="d5b85-131">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="d5b85-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="d5b85-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="d5b85-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="d5b85-133">String</span><span class="sxs-lookup"><span data-stu-id="d5b85-133">String</span></span>|<span data-ttu-id="d5b85-134">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="d5b85-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5b85-135">关系</span><span class="sxs-lookup"><span data-stu-id="d5b85-135">Relationships</span></span>
<span data-ttu-id="d5b85-136">无</span><span class="sxs-lookup"><span data-stu-id="d5b85-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5b85-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5b85-137">JSON Representation</span></span>
<span data-ttu-id="d5b85-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5b85-138">Here is a JSON representation of the resource.</span></span>
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





