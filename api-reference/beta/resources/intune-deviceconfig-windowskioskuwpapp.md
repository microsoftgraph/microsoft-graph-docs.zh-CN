---
title: windowsKioskUWPApp 资源类型
description: 一类应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dbaf8dfd7f2cd488de37378f934ca3f31daedd6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147325"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="5a045-103">windowsKioskUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a045-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="5a045-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a045-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a045-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a045-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a045-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="5a045-106">The base class for a type of apps</span></span>


<span data-ttu-id="5a045-107">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5a045-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a045-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a045-108">Properties</span></span>
|<span data-ttu-id="5a045-109">属性</span><span class="sxs-lookup"><span data-stu-id="5a045-109">Property</span></span>|<span data-ttu-id="5a045-110">类型</span><span class="sxs-lookup"><span data-stu-id="5a045-110">Type</span></span>|<span data-ttu-id="5a045-111">说明</span><span class="sxs-lookup"><span data-stu-id="5a045-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a045-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="5a045-112">startLayoutTileSize</span></span>|[<span data-ttu-id="5a045-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="5a045-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="5a045-114">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="5a045-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5a045-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="5a045-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="5a045-116">name</span><span class="sxs-lookup"><span data-stu-id="5a045-116">name</span></span>|<span data-ttu-id="5a045-117">字符串</span><span class="sxs-lookup"><span data-stu-id="5a045-117">String</span></span>|<span data-ttu-id="5a045-118">表示从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="5a045-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="5a045-119">appType</span><span class="sxs-lookup"><span data-stu-id="5a045-119">appType</span></span>|[<span data-ttu-id="5a045-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="5a045-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="5a045-121">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="5a045-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5a045-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="5a045-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="5a045-123">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="5a045-123">appUserModelId</span></span>|<span data-ttu-id="5a045-124">字符串</span><span class="sxs-lookup"><span data-stu-id="5a045-124">String</span></span>|<span data-ttu-id="5a045-125">这是在展台模式下可启动使用的唯一应用程序用户模型 ID (AUMID)</span><span class="sxs-lookup"><span data-stu-id="5a045-125">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="5a045-126">appId</span><span class="sxs-lookup"><span data-stu-id="5a045-126">appId</span></span>|<span data-ttu-id="5a045-127">String</span><span class="sxs-lookup"><span data-stu-id="5a045-127">String</span></span>|<span data-ttu-id="5a045-128">这将引用将作为展台配置的目标的 Intune 应用</span><span class="sxs-lookup"><span data-stu-id="5a045-128">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="5a045-129">containedAppId</span><span class="sxs-lookup"><span data-stu-id="5a045-129">containedAppId</span></span>|<span data-ttu-id="5a045-130">字符串</span><span class="sxs-lookup"><span data-stu-id="5a045-130">String</span></span>|<span data-ttu-id="5a045-131">这将从 Intune 应用程序中引用包含的应用程序</span><span class="sxs-lookup"><span data-stu-id="5a045-131">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a045-132">关系</span><span class="sxs-lookup"><span data-stu-id="5a045-132">Relationships</span></span>
<span data-ttu-id="5a045-133">无</span><span class="sxs-lookup"><span data-stu-id="5a045-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a045-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a045-134">JSON Representation</span></span>
<span data-ttu-id="5a045-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a045-135">Here is a JSON representation of the resource.</span></span>
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




