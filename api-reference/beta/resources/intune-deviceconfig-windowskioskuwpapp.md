---
title: windowsKioskUWPApp 资源类型
description: 一类应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8526eeafbeea990ff2b3f487dd94cfe7b7d302bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573198"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="87c1b-103">windowsKioskUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="87c1b-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="87c1b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87c1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87c1b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87c1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87c1b-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="87c1b-106">The base class for a type of apps</span></span>


<span data-ttu-id="87c1b-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="87c1b-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="87c1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="87c1b-108">Properties</span></span>
|<span data-ttu-id="87c1b-109">属性</span><span class="sxs-lookup"><span data-stu-id="87c1b-109">Property</span></span>|<span data-ttu-id="87c1b-110">类型</span><span class="sxs-lookup"><span data-stu-id="87c1b-110">Type</span></span>|<span data-ttu-id="87c1b-111">说明</span><span class="sxs-lookup"><span data-stu-id="87c1b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87c1b-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="87c1b-112">startLayoutTileSize</span></span>|[<span data-ttu-id="87c1b-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="87c1b-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="87c1b-114">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="87c1b-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="87c1b-115">可取值为：`hidden`、`small`、`medium`、`wide` 或 `large`。</span><span class="sxs-lookup"><span data-stu-id="87c1b-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="87c1b-116">name</span><span class="sxs-lookup"><span data-stu-id="87c1b-116">name</span></span>|<span data-ttu-id="87c1b-117">String</span><span class="sxs-lookup"><span data-stu-id="87c1b-117">String</span></span>|<span data-ttu-id="87c1b-118">表示从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="87c1b-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="87c1b-119">appType</span><span class="sxs-lookup"><span data-stu-id="87c1b-119">appType</span></span>|[<span data-ttu-id="87c1b-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="87c1b-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="87c1b-121">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="87c1b-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="87c1b-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="87c1b-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="87c1b-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="87c1b-123">autoLaunch</span></span>|<span data-ttu-id="87c1b-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="87c1b-124">Boolean</span></span>|<span data-ttu-id="87c1b-125">允许在从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序</span><span class="sxs-lookup"><span data-stu-id="87c1b-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="87c1b-126">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="87c1b-126">appUserModelId</span></span>|<span data-ttu-id="87c1b-127">String</span><span class="sxs-lookup"><span data-stu-id="87c1b-127">String</span></span>|<span data-ttu-id="87c1b-128">这是在展台模式下可启动使用的唯一应用程序用户模型 ID (AUMID)</span><span class="sxs-lookup"><span data-stu-id="87c1b-128">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="87c1b-129">appId</span><span class="sxs-lookup"><span data-stu-id="87c1b-129">appId</span></span>|<span data-ttu-id="87c1b-130">String</span><span class="sxs-lookup"><span data-stu-id="87c1b-130">String</span></span>|<span data-ttu-id="87c1b-131">这将引用将作为展台配置的目标的 Intune 应用</span><span class="sxs-lookup"><span data-stu-id="87c1b-131">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="87c1b-132">containedAppId</span><span class="sxs-lookup"><span data-stu-id="87c1b-132">containedAppId</span></span>|<span data-ttu-id="87c1b-133">String</span><span class="sxs-lookup"><span data-stu-id="87c1b-133">String</span></span>|<span data-ttu-id="87c1b-134">这将从 Intune 应用程序中引用包含的应用程序</span><span class="sxs-lookup"><span data-stu-id="87c1b-134">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="87c1b-135">关系</span><span class="sxs-lookup"><span data-stu-id="87c1b-135">Relationships</span></span>
<span data-ttu-id="87c1b-136">无</span><span class="sxs-lookup"><span data-stu-id="87c1b-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87c1b-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87c1b-137">JSON Representation</span></span>
<span data-ttu-id="87c1b-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87c1b-138">Here is a JSON representation of the resource.</span></span>
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





