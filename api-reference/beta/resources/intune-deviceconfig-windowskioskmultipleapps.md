---
title: windowsKioskMultipleApps 资源类型
description: 用于标识网亭配置的多模式的应用程序配置的类
ms.openlocfilehash: 2b52cbe343c4a8d81391ad448e8f10f64fef295e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044114"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="76d82-103">windowsKioskMultipleApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="76d82-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="76d82-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="76d82-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76d82-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76d82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76d82-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="76d82-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76d82-107">用于标识网亭配置的多模式的应用程序配置的类</span><span class="sxs-lookup"><span data-stu-id="76d82-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="76d82-108">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76d82-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76d82-109">属性</span><span class="sxs-lookup"><span data-stu-id="76d82-109">Properties</span></span>
|<span data-ttu-id="76d82-110">属性</span><span class="sxs-lookup"><span data-stu-id="76d82-110">Property</span></span>|<span data-ttu-id="76d82-111">类型</span><span class="sxs-lookup"><span data-stu-id="76d82-111">Type</span></span>|<span data-ttu-id="76d82-112">说明</span><span class="sxs-lookup"><span data-stu-id="76d82-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76d82-113">apps</span><span class="sxs-lookup"><span data-stu-id="76d82-113">apps</span></span>|<span data-ttu-id="76d82-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)集合</span><span class="sxs-lookup"><span data-stu-id="76d82-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="76d82-115">这些是唯一的 Windows 应用商店应用程序将可以从开始菜单启动。</span><span class="sxs-lookup"><span data-stu-id="76d82-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="76d82-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="76d82-116">showTaskBar</span></span>|<span data-ttu-id="76d82-117">布尔</span><span class="sxs-lookup"><span data-stu-id="76d82-117">Boolean</span></span>|<span data-ttu-id="76d82-118">此设置，管理员可以指定任务条形图或不所示。</span><span class="sxs-lookup"><span data-stu-id="76d82-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="76d82-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="76d82-119">disallowDesktopApps</span></span>|<span data-ttu-id="76d82-120">布尔</span><span class="sxs-lookup"><span data-stu-id="76d82-120">Boolean</span></span>|<span data-ttu-id="76d82-121">此设置表示允许桌面应用程序。</span><span class="sxs-lookup"><span data-stu-id="76d82-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="76d82-122">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="76d82-122">Default to true.</span></span>|
|<span data-ttu-id="76d82-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="76d82-123">startMenuLayoutXml</span></span>|<span data-ttu-id="76d82-124">Binary</span><span class="sxs-lookup"><span data-stu-id="76d82-124">Binary</span></span>|<span data-ttu-id="76d82-125">允许管理员可以重写默认开始布局，并禁止用户更改它。</span><span class="sxs-lookup"><span data-stu-id="76d82-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="76d82-126">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="76d82-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="76d82-127">XML 需要以二进制格式。</span><span class="sxs-lookup"><span data-stu-id="76d82-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76d82-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="76d82-128">Relationships</span></span>
<span data-ttu-id="76d82-129">无</span><span class="sxs-lookup"><span data-stu-id="76d82-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="76d82-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76d82-130">JSON Representation</span></span>
<span data-ttu-id="76d82-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76d82-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





