---
title: windowsKioskDesktopApp 资源类型
description: 一类应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89f309b53e44b0f2843145dd7c0f4d3ffa6d7f98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453962"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="f1cdd-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1cdd-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="f1cdd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1cdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1cdd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1cdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1cdd-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="f1cdd-106">The base class for a type of apps</span></span>


<span data-ttu-id="f1cdd-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="f1cdd-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1cdd-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1cdd-108">Properties</span></span>
|<span data-ttu-id="f1cdd-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1cdd-109">Property</span></span>|<span data-ttu-id="f1cdd-110">类型</span><span class="sxs-lookup"><span data-stu-id="f1cdd-110">Type</span></span>|<span data-ttu-id="f1cdd-111">描述</span><span class="sxs-lookup"><span data-stu-id="f1cdd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1cdd-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f1cdd-112">startLayoutTileSize</span></span>|[<span data-ttu-id="f1cdd-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f1cdd-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="f1cdd-114">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="f1cdd-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f1cdd-115">可取值为：`hidden`、`small`、`medium`、`wide` 或 `large`。</span><span class="sxs-lookup"><span data-stu-id="f1cdd-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="f1cdd-116">name</span><span class="sxs-lookup"><span data-stu-id="f1cdd-116">name</span></span>|<span data-ttu-id="f1cdd-117">String</span><span class="sxs-lookup"><span data-stu-id="f1cdd-117">String</span></span>|<span data-ttu-id="f1cdd-118">表示从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="f1cdd-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f1cdd-119">appType</span><span class="sxs-lookup"><span data-stu-id="f1cdd-119">appType</span></span>|[<span data-ttu-id="f1cdd-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="f1cdd-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="f1cdd-121">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="f1cdd-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f1cdd-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="f1cdd-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="f1cdd-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="f1cdd-123">autoLaunch</span></span>|<span data-ttu-id="f1cdd-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1cdd-124">Boolean</span></span>|<span data-ttu-id="f1cdd-125">允许在从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="f1cdd-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f1cdd-126">路径</span><span class="sxs-lookup"><span data-stu-id="f1cdd-126">path</span></span>|<span data-ttu-id="f1cdd-127">String</span><span class="sxs-lookup"><span data-stu-id="f1cdd-127">String</span></span>|<span data-ttu-id="f1cdd-128">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="f1cdd-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="f1cdd-129">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="f1cdd-129">desktopApplicationId</span></span>|<span data-ttu-id="f1cdd-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f1cdd-130">String</span></span>|<span data-ttu-id="f1cdd-131">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="f1cdd-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="f1cdd-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f1cdd-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="f1cdd-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f1cdd-133">String</span></span>|<span data-ttu-id="f1cdd-134">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f1cdd-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1cdd-135">关系</span><span class="sxs-lookup"><span data-stu-id="f1cdd-135">Relationships</span></span>
<span data-ttu-id="f1cdd-136">无</span><span class="sxs-lookup"><span data-stu-id="f1cdd-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1cdd-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1cdd-137">JSON Representation</span></span>
<span data-ttu-id="f1cdd-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1cdd-138">Here is a JSON representation of the resource.</span></span>
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





