---
title: windowsKioskMultipleApps 资源类型
description: 用于标识展台配置的多模式应用配置的类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c657300cf3ca00482b85b7983f28b4df3135c97d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570841"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="96a17-103">windowsKioskMultipleApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="96a17-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="96a17-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96a17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96a17-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96a17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96a17-106">用于标识展台配置的多模式应用配置的类</span><span class="sxs-lookup"><span data-stu-id="96a17-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="96a17-107">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96a17-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96a17-108">属性</span><span class="sxs-lookup"><span data-stu-id="96a17-108">Properties</span></span>
|<span data-ttu-id="96a17-109">属性</span><span class="sxs-lookup"><span data-stu-id="96a17-109">Property</span></span>|<span data-ttu-id="96a17-110">类型</span><span class="sxs-lookup"><span data-stu-id="96a17-110">Type</span></span>|<span data-ttu-id="96a17-111">说明</span><span class="sxs-lookup"><span data-stu-id="96a17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a17-112">apps</span><span class="sxs-lookup"><span data-stu-id="96a17-112">apps</span></span>|<span data-ttu-id="96a17-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)集合</span><span class="sxs-lookup"><span data-stu-id="96a17-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="96a17-114">这些是仅可从 "开始" 菜单启动的 Windows 应用商店应用程序。</span><span class="sxs-lookup"><span data-stu-id="96a17-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="96a17-115">此集合最多可包含128个元素。</span><span class="sxs-lookup"><span data-stu-id="96a17-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="96a17-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="96a17-116">showTaskBar</span></span>|<span data-ttu-id="96a17-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a17-117">Boolean</span></span>|<span data-ttu-id="96a17-118">通过此设置, 管理员可以指定是否显示任务条形图。</span><span class="sxs-lookup"><span data-stu-id="96a17-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="96a17-119">allowAccessToDownloadsFolder</span><span class="sxs-lookup"><span data-stu-id="96a17-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="96a17-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a17-120">Boolean</span></span>|<span data-ttu-id="96a17-121">此设置允许访问文件资源管理器中的下载文件夹。</span><span class="sxs-lookup"><span data-stu-id="96a17-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="96a17-122">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="96a17-122">disallowDesktopApps</span></span>|<span data-ttu-id="96a17-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a17-123">Boolean</span></span>|<span data-ttu-id="96a17-124">此设置指示允许桌面应用。</span><span class="sxs-lookup"><span data-stu-id="96a17-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="96a17-125">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="96a17-125">Default to true.</span></span>|
|<span data-ttu-id="96a17-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="96a17-126">startMenuLayoutXml</span></span>|<span data-ttu-id="96a17-127">Binary</span><span class="sxs-lookup"><span data-stu-id="96a17-127">Binary</span></span>|<span data-ttu-id="96a17-128">允许管理员覆盖默认的 "开始" 布局, 并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="96a17-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="96a17-129">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="96a17-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="96a17-130">XML 必须采用二进制格式。</span><span class="sxs-lookup"><span data-stu-id="96a17-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96a17-131">关系</span><span class="sxs-lookup"><span data-stu-id="96a17-131">Relationships</span></span>
<span data-ttu-id="96a17-132">无</span><span class="sxs-lookup"><span data-stu-id="96a17-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96a17-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96a17-133">JSON Representation</span></span>
<span data-ttu-id="96a17-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96a17-134">Here is a JSON representation of the resource.</span></span>
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
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```




