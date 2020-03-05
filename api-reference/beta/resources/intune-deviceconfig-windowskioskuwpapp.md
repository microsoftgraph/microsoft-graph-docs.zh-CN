---
title: windowsKioskUWPApp 资源类型
description: 一类应用程序的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 840332c2873f1a42adc5a6f1ef501f411842aa32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529020"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="568a1-103">windowsKioskUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="568a1-103">windowsKioskUWPApp resource type</span></span>

<span data-ttu-id="568a1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="568a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="568a1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="568a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="568a1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="568a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="568a1-107">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="568a1-107">The base class for a type of apps</span></span>


<span data-ttu-id="568a1-108">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="568a1-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="568a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="568a1-109">Properties</span></span>
|<span data-ttu-id="568a1-110">属性</span><span class="sxs-lookup"><span data-stu-id="568a1-110">Property</span></span>|<span data-ttu-id="568a1-111">类型</span><span class="sxs-lookup"><span data-stu-id="568a1-111">Type</span></span>|<span data-ttu-id="568a1-112">说明</span><span class="sxs-lookup"><span data-stu-id="568a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="568a1-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="568a1-113">startLayoutTileSize</span></span>|[<span data-ttu-id="568a1-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="568a1-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="568a1-115">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="568a1-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="568a1-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="568a1-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="568a1-117">name</span><span class="sxs-lookup"><span data-stu-id="568a1-117">name</span></span>|<span data-ttu-id="568a1-118">字符串</span><span class="sxs-lookup"><span data-stu-id="568a1-118">String</span></span>|<span data-ttu-id="568a1-119">表示从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="568a1-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="568a1-120">appType</span><span class="sxs-lookup"><span data-stu-id="568a1-120">appType</span></span>|[<span data-ttu-id="568a1-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="568a1-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="568a1-122">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="568a1-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="568a1-123">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="568a1-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="568a1-124">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="568a1-124">autoLaunch</span></span>|<span data-ttu-id="568a1-125">布尔</span><span class="sxs-lookup"><span data-stu-id="568a1-125">Boolean</span></span>|<span data-ttu-id="568a1-126">允许在从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="568a1-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="568a1-127">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="568a1-127">appUserModelId</span></span>|<span data-ttu-id="568a1-128">String</span><span class="sxs-lookup"><span data-stu-id="568a1-128">String</span></span>|<span data-ttu-id="568a1-129">这是在展台模式下可启动使用的唯一应用程序用户模型 ID （AUMID）</span><span class="sxs-lookup"><span data-stu-id="568a1-129">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="568a1-130">appId</span><span class="sxs-lookup"><span data-stu-id="568a1-130">appId</span></span>|<span data-ttu-id="568a1-131">String</span><span class="sxs-lookup"><span data-stu-id="568a1-131">String</span></span>|<span data-ttu-id="568a1-132">这将引用将作为展台配置的目标的 Intune 应用</span><span class="sxs-lookup"><span data-stu-id="568a1-132">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="568a1-133">containedAppId</span><span class="sxs-lookup"><span data-stu-id="568a1-133">containedAppId</span></span>|<span data-ttu-id="568a1-134">String</span><span class="sxs-lookup"><span data-stu-id="568a1-134">String</span></span>|<span data-ttu-id="568a1-135">这将从 Intune 应用程序中引用包含的应用程序</span><span class="sxs-lookup"><span data-stu-id="568a1-135">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="568a1-136">关系</span><span class="sxs-lookup"><span data-stu-id="568a1-136">Relationships</span></span>
<span data-ttu-id="568a1-137">无</span><span class="sxs-lookup"><span data-stu-id="568a1-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="568a1-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="568a1-138">JSON Representation</span></span>
<span data-ttu-id="568a1-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="568a1-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```



