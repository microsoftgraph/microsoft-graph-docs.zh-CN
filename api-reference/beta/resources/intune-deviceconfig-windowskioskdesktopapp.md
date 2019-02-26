---
title: windowsKioskDesktopApp 资源类型
description: 一类应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0487fa24ecd2d27817349b68063cf606a2401944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170474"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="78e2e-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="78e2e-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="78e2e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78e2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e2e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78e2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e2e-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="78e2e-106">The base class for a type of apps</span></span>


<span data-ttu-id="78e2e-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="78e2e-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78e2e-108">属性</span><span class="sxs-lookup"><span data-stu-id="78e2e-108">Properties</span></span>
|<span data-ttu-id="78e2e-109">属性</span><span class="sxs-lookup"><span data-stu-id="78e2e-109">Property</span></span>|<span data-ttu-id="78e2e-110">类型</span><span class="sxs-lookup"><span data-stu-id="78e2e-110">Type</span></span>|<span data-ttu-id="78e2e-111">说明</span><span class="sxs-lookup"><span data-stu-id="78e2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e2e-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="78e2e-112">startLayoutTileSize</span></span>|[<span data-ttu-id="78e2e-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="78e2e-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="78e2e-114">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="78e2e-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="78e2e-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="78e2e-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="78e2e-116">name</span><span class="sxs-lookup"><span data-stu-id="78e2e-116">name</span></span>|<span data-ttu-id="78e2e-117">字符串</span><span class="sxs-lookup"><span data-stu-id="78e2e-117">String</span></span>|<span data-ttu-id="78e2e-118">表示从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="78e2e-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="78e2e-119">appType</span><span class="sxs-lookup"><span data-stu-id="78e2e-119">appType</span></span>|[<span data-ttu-id="78e2e-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="78e2e-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="78e2e-121">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="78e2e-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="78e2e-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="78e2e-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="78e2e-123">路径</span><span class="sxs-lookup"><span data-stu-id="78e2e-123">path</span></span>|<span data-ttu-id="78e2e-124">String</span><span class="sxs-lookup"><span data-stu-id="78e2e-124">String</span></span>|<span data-ttu-id="78e2e-125">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="78e2e-125">Define the path of a desktop app</span></span>|
|<span data-ttu-id="78e2e-126">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="78e2e-126">desktopApplicationId</span></span>|<span data-ttu-id="78e2e-127">String</span><span class="sxs-lookup"><span data-stu-id="78e2e-127">String</span></span>|<span data-ttu-id="78e2e-128">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="78e2e-128">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="78e2e-129">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="78e2e-129">desktopApplicationLinkPath</span></span>|<span data-ttu-id="78e2e-130">String</span><span class="sxs-lookup"><span data-stu-id="78e2e-130">String</span></span>|<span data-ttu-id="78e2e-131">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="78e2e-131">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="78e2e-132">关系</span><span class="sxs-lookup"><span data-stu-id="78e2e-132">Relationships</span></span>
<span data-ttu-id="78e2e-133">无</span><span class="sxs-lookup"><span data-stu-id="78e2e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78e2e-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78e2e-134">JSON Representation</span></span>
<span data-ttu-id="78e2e-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78e2e-135">Here is a JSON representation of the resource.</span></span>
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




