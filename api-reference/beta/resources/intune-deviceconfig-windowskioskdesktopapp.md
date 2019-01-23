---
title: windowsKioskDesktopApp 资源类型
description: 一种类型的应用程序的基类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 831ed86da24791cde549687ecaff42cabc29a99e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415304"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="f3647-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3647-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="f3647-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f3647-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3647-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f3647-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3647-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3647-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3647-107">一种类型的应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="f3647-107">The base class for a type of apps</span></span>


<span data-ttu-id="f3647-108">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="f3647-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3647-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3647-109">Properties</span></span>
|<span data-ttu-id="f3647-110">属性</span><span class="sxs-lookup"><span data-stu-id="f3647-110">Property</span></span>|<span data-ttu-id="f3647-111">类型</span><span class="sxs-lookup"><span data-stu-id="f3647-111">Type</span></span>|<span data-ttu-id="f3647-112">说明</span><span class="sxs-lookup"><span data-stu-id="f3647-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3647-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f3647-113">startLayoutTileSize</span></span>|[<span data-ttu-id="f3647-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f3647-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="f3647-115">开始布局继承[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)从应用程序图块大小。</span><span class="sxs-lookup"><span data-stu-id="f3647-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f3647-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="f3647-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="f3647-117">name</span><span class="sxs-lookup"><span data-stu-id="f3647-117">name</span></span>|<span data-ttu-id="f3647-118">String</span><span class="sxs-lookup"><span data-stu-id="f3647-118">String</span></span>|<span data-ttu-id="f3647-119">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)代表应用程序继承的友好名称</span><span class="sxs-lookup"><span data-stu-id="f3647-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f3647-120">appType</span><span class="sxs-lookup"><span data-stu-id="f3647-120">appType</span></span>|[<span data-ttu-id="f3647-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="f3647-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="f3647-122">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)该应用程序类型继承。</span><span class="sxs-lookup"><span data-stu-id="f3647-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f3647-123">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="f3647-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="f3647-124">路径</span><span class="sxs-lookup"><span data-stu-id="f3647-124">path</span></span>|<span data-ttu-id="f3647-125">String</span><span class="sxs-lookup"><span data-stu-id="f3647-125">String</span></span>|<span data-ttu-id="f3647-126">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="f3647-126">Define the path of a desktop app</span></span>|
|<span data-ttu-id="f3647-127">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="f3647-127">desktopApplicationId</span></span>|<span data-ttu-id="f3647-128">String</span><span class="sxs-lookup"><span data-stu-id="f3647-128">String</span></span>|<span data-ttu-id="f3647-129">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="f3647-129">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="f3647-130">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f3647-130">desktopApplicationLinkPath</span></span>|<span data-ttu-id="f3647-131">String</span><span class="sxs-lookup"><span data-stu-id="f3647-131">String</span></span>|<span data-ttu-id="f3647-132">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f3647-132">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3647-133">关系</span><span class="sxs-lookup"><span data-stu-id="f3647-133">Relationships</span></span>
<span data-ttu-id="f3647-134">无</span><span class="sxs-lookup"><span data-stu-id="f3647-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3647-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3647-135">JSON Representation</span></span>
<span data-ttu-id="f3647-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3647-136">Here is a JSON representation of the resource.</span></span>
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




