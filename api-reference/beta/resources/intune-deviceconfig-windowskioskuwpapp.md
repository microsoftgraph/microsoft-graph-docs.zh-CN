---
title: windowsKioskUWPApp 资源类型
description: 一类应用程序的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 324d4806abbbbdbd409b920c1e4fad7ebf8dbe4b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370793"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="6b972-103">windowsKioskUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b972-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="6b972-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b972-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b972-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="6b972-106">The base class for a type of apps</span></span>


<span data-ttu-id="6b972-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="6b972-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b972-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b972-108">Properties</span></span>
|<span data-ttu-id="6b972-109">属性</span><span class="sxs-lookup"><span data-stu-id="6b972-109">Property</span></span>|<span data-ttu-id="6b972-110">类型</span><span class="sxs-lookup"><span data-stu-id="6b972-110">Type</span></span>|<span data-ttu-id="6b972-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b972-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b972-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6b972-112">startLayoutTileSize</span></span>|[<span data-ttu-id="6b972-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6b972-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="6b972-114">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="6b972-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6b972-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="6b972-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="6b972-116">name</span><span class="sxs-lookup"><span data-stu-id="6b972-116">name</span></span>|<span data-ttu-id="6b972-117">字符串</span><span class="sxs-lookup"><span data-stu-id="6b972-117">String</span></span>|<span data-ttu-id="6b972-118">表示从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="6b972-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="6b972-119">appType</span><span class="sxs-lookup"><span data-stu-id="6b972-119">appType</span></span>|[<span data-ttu-id="6b972-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="6b972-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="6b972-121">从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="6b972-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6b972-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="6b972-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="6b972-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="6b972-123">autoLaunch</span></span>|<span data-ttu-id="6b972-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b972-124">Boolean</span></span>|<span data-ttu-id="6b972-125">允许在从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="6b972-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="6b972-126">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="6b972-126">appUserModelId</span></span>|<span data-ttu-id="6b972-127">String</span><span class="sxs-lookup"><span data-stu-id="6b972-127">String</span></span>|<span data-ttu-id="6b972-128">这是在展台模式下可启动使用的唯一应用程序用户模型 ID (AUMID)</span><span class="sxs-lookup"><span data-stu-id="6b972-128">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="6b972-129">appId</span><span class="sxs-lookup"><span data-stu-id="6b972-129">appId</span></span>|<span data-ttu-id="6b972-130">String</span><span class="sxs-lookup"><span data-stu-id="6b972-130">String</span></span>|<span data-ttu-id="6b972-131">这将引用将作为展台配置的目标的 Intune 应用</span><span class="sxs-lookup"><span data-stu-id="6b972-131">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="6b972-132">containedAppId</span><span class="sxs-lookup"><span data-stu-id="6b972-132">containedAppId</span></span>|<span data-ttu-id="6b972-133">String</span><span class="sxs-lookup"><span data-stu-id="6b972-133">String</span></span>|<span data-ttu-id="6b972-134">这将从 Intune 应用程序中引用包含的应用程序</span><span class="sxs-lookup"><span data-stu-id="6b972-134">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b972-135">关系</span><span class="sxs-lookup"><span data-stu-id="6b972-135">Relationships</span></span>
<span data-ttu-id="6b972-136">无</span><span class="sxs-lookup"><span data-stu-id="6b972-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b972-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b972-137">JSON Representation</span></span>
<span data-ttu-id="6b972-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b972-138">Here is a JSON representation of the resource.</span></span>
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



