---
title: windowsKioskWin32App 资源类型
description: KioskModeApp v4 for Win32 应用支持
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7b0dd1a5afb5dcad27bd0b2656f29336be3332d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445946"
---
# <a name="windowskioskwin32app-resource-type"></a><span data-ttu-id="9b516-103">windowsKioskWin32App 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b516-103">windowsKioskWin32App resource type</span></span>

<span data-ttu-id="9b516-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b516-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b516-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b516-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b516-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b516-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b516-107">KioskModeApp v4 for Win32 应用支持</span><span class="sxs-lookup"><span data-stu-id="9b516-107">KioskModeApp v4 for Win32 app support</span></span>


<span data-ttu-id="9b516-108">继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="9b516-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b516-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b516-109">Properties</span></span>
|<span data-ttu-id="9b516-110">属性</span><span class="sxs-lookup"><span data-stu-id="9b516-110">Property</span></span>|<span data-ttu-id="9b516-111">类型</span><span class="sxs-lookup"><span data-stu-id="9b516-111">Type</span></span>|<span data-ttu-id="9b516-112">说明</span><span class="sxs-lookup"><span data-stu-id="9b516-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b516-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="9b516-113">startLayoutTileSize</span></span>|[<span data-ttu-id="9b516-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="9b516-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="9b516-115">开始布局的应用磁贴大小 继承自[windowsKioskAppBase。](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="9b516-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="9b516-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="9b516-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="9b516-117">name</span><span class="sxs-lookup"><span data-stu-id="9b516-117">name</span></span>|<span data-ttu-id="9b516-118">String</span><span class="sxs-lookup"><span data-stu-id="9b516-118">String</span></span>|<span data-ttu-id="9b516-119">表示应用的友好名称 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="9b516-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="9b516-120">appType</span><span class="sxs-lookup"><span data-stu-id="9b516-120">appType</span></span>|[<span data-ttu-id="9b516-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="9b516-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="9b516-122">应用类型 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)。</span><span class="sxs-lookup"><span data-stu-id="9b516-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="9b516-123">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="9b516-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="9b516-124">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="9b516-124">autoLaunch</span></span>|<span data-ttu-id="9b516-125">布尔</span><span class="sxs-lookup"><span data-stu-id="9b516-125">Boolean</span></span>|<span data-ttu-id="9b516-126">允许应用在多应用展台模式下自动启动 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="9b516-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="9b516-127">classicAppPath</span><span class="sxs-lookup"><span data-stu-id="9b516-127">classicAppPath</span></span>|<span data-ttu-id="9b516-128">String</span><span class="sxs-lookup"><span data-stu-id="9b516-128">String</span></span>|<span data-ttu-id="9b516-129">这是在展台模式下由 v4 Win32 应用使用的经典应用路径</span><span class="sxs-lookup"><span data-stu-id="9b516-129">This is the classicapppath to be used by v4 Win32 app while in Kiosk Mode</span></span>|
|<span data-ttu-id="9b516-130">edgeNoFirstRun</span><span class="sxs-lookup"><span data-stu-id="9b516-130">edgeNoFirstRun</span></span>|<span data-ttu-id="9b516-131">布尔</span><span class="sxs-lookup"><span data-stu-id="9b516-131">Boolean</span></span>|<span data-ttu-id="9b516-132">边缘展台模式的边缘首次运行标志</span><span class="sxs-lookup"><span data-stu-id="9b516-132">Edge first run flag for Edge kiosk mode</span></span>|
|<span data-ttu-id="9b516-133">edgeKioskIdleTimeoutMinutes</span><span class="sxs-lookup"><span data-stu-id="9b516-133">edgeKioskIdleTimeoutMinutes</span></span>|<span data-ttu-id="9b516-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9b516-134">Int32</span></span>|<span data-ttu-id="9b516-135">边缘展台模式的边缘展台空闲超时（以分钟表示）。</span><span class="sxs-lookup"><span data-stu-id="9b516-135">Edge kiosk idle timeout in minutes for Edge kiosk mode.</span></span> <span data-ttu-id="9b516-136">有效值为 0 到 1440</span><span class="sxs-lookup"><span data-stu-id="9b516-136">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="9b516-137">edgeKioskType</span><span class="sxs-lookup"><span data-stu-id="9b516-137">edgeKioskType</span></span>|[<span data-ttu-id="9b516-138">windowsEdgeKioskType</span><span class="sxs-lookup"><span data-stu-id="9b516-138">windowsEdgeKioskType</span></span>](../resources/intune-deviceconfig-windowsedgekiosktype.md)|<span data-ttu-id="9b516-139">边缘展台模式的边缘展台类型。</span><span class="sxs-lookup"><span data-stu-id="9b516-139">Edge kiosk type for Edge kiosk mode.</span></span> <span data-ttu-id="9b516-140">可取值为：`publicBrowsing`、`fullScreen`。</span><span class="sxs-lookup"><span data-stu-id="9b516-140">Possible values are: `publicBrowsing`, `fullScreen`.</span></span>|
|<span data-ttu-id="9b516-141">edgeKiosk</span><span class="sxs-lookup"><span data-stu-id="9b516-141">edgeKiosk</span></span>|<span data-ttu-id="9b516-142">String</span><span class="sxs-lookup"><span data-stu-id="9b516-142">String</span></span>|<span data-ttu-id="9b516-143">边缘展 (url) 用于边缘展台模式</span><span class="sxs-lookup"><span data-stu-id="9b516-143">Edge kiosk (url) for Edge kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b516-144">关系</span><span class="sxs-lookup"><span data-stu-id="9b516-144">Relationships</span></span>
<span data-ttu-id="9b516-145">无</span><span class="sxs-lookup"><span data-stu-id="9b516-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b516-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b516-146">JSON Representation</span></span>
<span data-ttu-id="9b516-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b516-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskWin32App",
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
```




