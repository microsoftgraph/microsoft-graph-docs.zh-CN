---
title: windowsKioskMultipleApps 资源类型
description: 用于标识展台配置的多模式应用配置的类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2d2ff38e3b07920f474d9e3894bbd1f8855e277
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162018"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="c5542-103">windowsKioskMultipleApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5542-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="c5542-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5542-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5542-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5542-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5542-106">用于标识展台配置的多模式应用配置的类</span><span class="sxs-lookup"><span data-stu-id="c5542-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="c5542-107">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5542-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5542-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5542-108">Properties</span></span>
|<span data-ttu-id="c5542-109">属性</span><span class="sxs-lookup"><span data-stu-id="c5542-109">Property</span></span>|<span data-ttu-id="c5542-110">类型</span><span class="sxs-lookup"><span data-stu-id="c5542-110">Type</span></span>|<span data-ttu-id="c5542-111">说明</span><span class="sxs-lookup"><span data-stu-id="c5542-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5542-112">apps</span><span class="sxs-lookup"><span data-stu-id="c5542-112">apps</span></span>|<span data-ttu-id="c5542-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5542-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="c5542-114">这些是仅可从 "开始" 菜单启动的 Windows 应用商店应用程序。</span><span class="sxs-lookup"><span data-stu-id="c5542-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="c5542-115">此集合最多可包含128个元素。</span><span class="sxs-lookup"><span data-stu-id="c5542-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="c5542-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="c5542-116">showTaskBar</span></span>|<span data-ttu-id="c5542-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5542-117">Boolean</span></span>|<span data-ttu-id="c5542-118">通过此设置, 管理员可以指定是否显示任务条形图。</span><span class="sxs-lookup"><span data-stu-id="c5542-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="c5542-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="c5542-119">disallowDesktopApps</span></span>|<span data-ttu-id="c5542-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5542-120">Boolean</span></span>|<span data-ttu-id="c5542-121">此设置指示允许桌面应用。</span><span class="sxs-lookup"><span data-stu-id="c5542-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="c5542-122">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="c5542-122">Default to true.</span></span>|
|<span data-ttu-id="c5542-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="c5542-123">startMenuLayoutXml</span></span>|<span data-ttu-id="c5542-124">Binary</span><span class="sxs-lookup"><span data-stu-id="c5542-124">Binary</span></span>|<span data-ttu-id="c5542-125">允许管理员覆盖默认的 "开始" 布局, 并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="c5542-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="c5542-126">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="c5542-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="c5542-127">XML 必须采用二进制格式。</span><span class="sxs-lookup"><span data-stu-id="c5542-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5542-128">关系</span><span class="sxs-lookup"><span data-stu-id="c5542-128">Relationships</span></span>
<span data-ttu-id="c5542-129">无</span><span class="sxs-lookup"><span data-stu-id="c5542-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5542-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5542-130">JSON Representation</span></span>
<span data-ttu-id="c5542-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5542-131">Here is a JSON representation of the resource.</span></span>
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
      "appType": "String",
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




