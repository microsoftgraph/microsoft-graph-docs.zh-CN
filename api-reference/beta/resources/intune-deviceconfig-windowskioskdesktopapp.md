---
title: windowsKioskDesktopApp 资源类型
description: 一类应用程序的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7df38deba11cae5199a781a38dda6cd4b5abb698
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529029"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="8a2a7-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a2a7-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="8a2a7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8a2a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a2a7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a2a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a2a7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a2a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a2a7-107">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="8a2a7-107">The base class for a type of apps</span></span>


<span data-ttu-id="8a2a7-108">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8a2a7-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a2a7-109">属性</span><span class="sxs-lookup"><span data-stu-id="8a2a7-109">Properties</span></span>
|<span data-ttu-id="8a2a7-110">属性</span><span class="sxs-lookup"><span data-stu-id="8a2a7-110">Property</span></span>|<span data-ttu-id="8a2a7-111">类型</span><span class="sxs-lookup"><span data-stu-id="8a2a7-111">Type</span></span>|<span data-ttu-id="8a2a7-112">说明</span><span class="sxs-lookup"><span data-stu-id="8a2a7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a2a7-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8a2a7-113">startLayoutTileSize</span></span>|[<span data-ttu-id="8a2a7-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8a2a7-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="8a2a7-115">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="8a2a7-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="8a2a7-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="8a2a7-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="8a2a7-117">name</span><span class="sxs-lookup"><span data-stu-id="8a2a7-117">name</span></span>|<span data-ttu-id="8a2a7-118">String</span><span class="sxs-lookup"><span data-stu-id="8a2a7-118">String</span></span>|<span data-ttu-id="8a2a7-119">表示从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="8a2a7-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="8a2a7-120">appType</span><span class="sxs-lookup"><span data-stu-id="8a2a7-120">appType</span></span>|[<span data-ttu-id="8a2a7-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="8a2a7-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="8a2a7-122">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="8a2a7-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="8a2a7-123">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="8a2a7-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="8a2a7-124">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="8a2a7-124">autoLaunch</span></span>|<span data-ttu-id="8a2a7-125">布尔</span><span class="sxs-lookup"><span data-stu-id="8a2a7-125">Boolean</span></span>|<span data-ttu-id="8a2a7-126">允许在从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="8a2a7-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="8a2a7-127">路径</span><span class="sxs-lookup"><span data-stu-id="8a2a7-127">path</span></span>|<span data-ttu-id="8a2a7-128">String</span><span class="sxs-lookup"><span data-stu-id="8a2a7-128">String</span></span>|<span data-ttu-id="8a2a7-129">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="8a2a7-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="8a2a7-130">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="8a2a7-130">desktopApplicationId</span></span>|<span data-ttu-id="8a2a7-131">String</span><span class="sxs-lookup"><span data-stu-id="8a2a7-131">String</span></span>|<span data-ttu-id="8a2a7-132">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="8a2a7-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="8a2a7-133">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="8a2a7-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="8a2a7-134">String</span><span class="sxs-lookup"><span data-stu-id="8a2a7-134">String</span></span>|<span data-ttu-id="8a2a7-135">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="8a2a7-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a2a7-136">关系</span><span class="sxs-lookup"><span data-stu-id="8a2a7-136">Relationships</span></span>
<span data-ttu-id="8a2a7-137">无</span><span class="sxs-lookup"><span data-stu-id="8a2a7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a2a7-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a2a7-138">JSON Representation</span></span>
<span data-ttu-id="8a2a7-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a2a7-139">Here is a JSON representation of the resource.</span></span>
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



