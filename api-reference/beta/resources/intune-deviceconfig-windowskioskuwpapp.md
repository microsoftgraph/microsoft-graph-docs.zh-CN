---
title: windowsKioskUWPApp 资源类型
description: 一种类型的应用程序的基类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ba5367721890f02af3b348ad469b15024de4800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392680"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="6be90-103">windowsKioskUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="6be90-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="6be90-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6be90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6be90-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6be90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6be90-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6be90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be90-107">一种类型的应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="6be90-107">The base class for a type of apps</span></span>


<span data-ttu-id="6be90-108">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="6be90-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6be90-109">属性</span><span class="sxs-lookup"><span data-stu-id="6be90-109">Properties</span></span>
|<span data-ttu-id="6be90-110">属性</span><span class="sxs-lookup"><span data-stu-id="6be90-110">Property</span></span>|<span data-ttu-id="6be90-111">类型</span><span class="sxs-lookup"><span data-stu-id="6be90-111">Type</span></span>|<span data-ttu-id="6be90-112">说明</span><span class="sxs-lookup"><span data-stu-id="6be90-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be90-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6be90-113">startLayoutTileSize</span></span>|[<span data-ttu-id="6be90-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6be90-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="6be90-115">开始布局继承[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)从应用程序图块大小。</span><span class="sxs-lookup"><span data-stu-id="6be90-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6be90-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="6be90-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="6be90-117">name</span><span class="sxs-lookup"><span data-stu-id="6be90-117">name</span></span>|<span data-ttu-id="6be90-118">String</span><span class="sxs-lookup"><span data-stu-id="6be90-118">String</span></span>|<span data-ttu-id="6be90-119">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)代表应用程序继承的友好名称</span><span class="sxs-lookup"><span data-stu-id="6be90-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="6be90-120">appType</span><span class="sxs-lookup"><span data-stu-id="6be90-120">appType</span></span>|[<span data-ttu-id="6be90-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="6be90-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="6be90-122">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)该应用程序类型继承。</span><span class="sxs-lookup"><span data-stu-id="6be90-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6be90-123">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="6be90-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="6be90-124">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="6be90-124">appUserModelId</span></span>|<span data-ttu-id="6be90-125">String</span><span class="sxs-lookup"><span data-stu-id="6be90-125">String</span></span>|<span data-ttu-id="6be90-126">这是仅应用程序用户模型 ID (AUMID) 将可用于启动在展台模式中使用</span><span class="sxs-lookup"><span data-stu-id="6be90-126">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="6be90-127">appId</span><span class="sxs-lookup"><span data-stu-id="6be90-127">appId</span></span>|<span data-ttu-id="6be90-128">String</span><span class="sxs-lookup"><span data-stu-id="6be90-128">String</span></span>|<span data-ttu-id="6be90-129">此引用 Intune 应用程序将作为网亭配置的同一个分配到的目标</span><span class="sxs-lookup"><span data-stu-id="6be90-129">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="6be90-130">containedAppId</span><span class="sxs-lookup"><span data-stu-id="6be90-130">containedAppId</span></span>|<span data-ttu-id="6be90-131">String</span><span class="sxs-lookup"><span data-stu-id="6be90-131">String</span></span>|<span data-ttu-id="6be90-132">此引用包含应用程序中 Intune 应用程序</span><span class="sxs-lookup"><span data-stu-id="6be90-132">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="6be90-133">关系</span><span class="sxs-lookup"><span data-stu-id="6be90-133">Relationships</span></span>
<span data-ttu-id="6be90-134">无</span><span class="sxs-lookup"><span data-stu-id="6be90-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6be90-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6be90-135">JSON Representation</span></span>
<span data-ttu-id="6be90-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6be90-136">Here is a JSON representation of the resource.</span></span>
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




