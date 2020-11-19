---
title: windowsKioskDesktopApp 资源类型
description: 一类应用程序的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5c5f3ab5bc7e87a57c80c74698e4fb8f0656063
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293455"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="f6331-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6331-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="f6331-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6331-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6331-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6331-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6331-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6331-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6331-107">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="f6331-107">The base class for a type of apps</span></span>


<span data-ttu-id="f6331-108">继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="f6331-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6331-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6331-109">Properties</span></span>
|<span data-ttu-id="f6331-110">属性</span><span class="sxs-lookup"><span data-stu-id="f6331-110">Property</span></span>|<span data-ttu-id="f6331-111">类型</span><span class="sxs-lookup"><span data-stu-id="f6331-111">Type</span></span>|<span data-ttu-id="f6331-112">Description</span><span class="sxs-lookup"><span data-stu-id="f6331-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6331-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f6331-113">startLayoutTileSize</span></span>|[<span data-ttu-id="f6331-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f6331-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="f6331-115">从 [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="f6331-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f6331-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="f6331-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="f6331-117">name</span><span class="sxs-lookup"><span data-stu-id="f6331-117">name</span></span>|<span data-ttu-id="f6331-118">字符串</span><span class="sxs-lookup"><span data-stu-id="f6331-118">String</span></span>|<span data-ttu-id="f6331-119">表示从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="f6331-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f6331-120">appType</span><span class="sxs-lookup"><span data-stu-id="f6331-120">appType</span></span>|[<span data-ttu-id="f6331-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="f6331-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="f6331-122">从 [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="f6331-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f6331-123">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="f6331-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="f6331-124">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="f6331-124">autoLaunch</span></span>|<span data-ttu-id="f6331-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6331-125">Boolean</span></span>|<span data-ttu-id="f6331-126">允许在从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="f6331-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f6331-127">路径</span><span class="sxs-lookup"><span data-stu-id="f6331-127">path</span></span>|<span data-ttu-id="f6331-128">String</span><span class="sxs-lookup"><span data-stu-id="f6331-128">String</span></span>|<span data-ttu-id="f6331-129">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="f6331-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="f6331-130">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="f6331-130">desktopApplicationId</span></span>|<span data-ttu-id="f6331-131">字符串</span><span class="sxs-lookup"><span data-stu-id="f6331-131">String</span></span>|<span data-ttu-id="f6331-132">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="f6331-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="f6331-133">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f6331-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="f6331-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f6331-134">String</span></span>|<span data-ttu-id="f6331-135">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f6331-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6331-136">关系</span><span class="sxs-lookup"><span data-stu-id="f6331-136">Relationships</span></span>
<span data-ttu-id="f6331-137">无</span><span class="sxs-lookup"><span data-stu-id="f6331-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6331-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6331-138">JSON Representation</span></span>
<span data-ttu-id="f6331-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6331-139">Here is a JSON representation of the resource.</span></span>
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




