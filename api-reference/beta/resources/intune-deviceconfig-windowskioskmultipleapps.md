---
title: windowsKioskMultipleApps 资源类型
description: 用于标识展台配置的多模式应用配置的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 766464e258abd3558a5d7e7cd8c5c74cb2b23477
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061943"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="c97ed-103">windowsKioskMultipleApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="c97ed-103">windowsKioskMultipleApps resource type</span></span>

<span data-ttu-id="c97ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c97ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c97ed-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c97ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c97ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c97ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c97ed-107">用于标识展台配置的多模式应用配置的类</span><span class="sxs-lookup"><span data-stu-id="c97ed-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="c97ed-108">继承自 [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c97ed-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c97ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="c97ed-109">Properties</span></span>
|<span data-ttu-id="c97ed-110">属性</span><span class="sxs-lookup"><span data-stu-id="c97ed-110">Property</span></span>|<span data-ttu-id="c97ed-111">类型</span><span class="sxs-lookup"><span data-stu-id="c97ed-111">Type</span></span>|<span data-ttu-id="c97ed-112">说明</span><span class="sxs-lookup"><span data-stu-id="c97ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c97ed-113">apps</span><span class="sxs-lookup"><span data-stu-id="c97ed-113">apps</span></span>|<span data-ttu-id="c97ed-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c97ed-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="c97ed-115">这些是仅可从 "开始" 菜单启动的 Windows 应用商店应用程序。</span><span class="sxs-lookup"><span data-stu-id="c97ed-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="c97ed-116">此集合最多可包含128个元素。</span><span class="sxs-lookup"><span data-stu-id="c97ed-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="c97ed-117">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="c97ed-117">showTaskBar</span></span>|<span data-ttu-id="c97ed-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c97ed-118">Boolean</span></span>|<span data-ttu-id="c97ed-119">通过此设置，管理员可以指定是否显示任务条形图。</span><span class="sxs-lookup"><span data-stu-id="c97ed-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="c97ed-120">allowAccessToDownloadsFolder</span><span class="sxs-lookup"><span data-stu-id="c97ed-120">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="c97ed-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c97ed-121">Boolean</span></span>|<span data-ttu-id="c97ed-122">此设置允许访问文件资源管理器中的下载文件夹。</span><span class="sxs-lookup"><span data-stu-id="c97ed-122">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="c97ed-123">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="c97ed-123">disallowDesktopApps</span></span>|<span data-ttu-id="c97ed-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c97ed-124">Boolean</span></span>|<span data-ttu-id="c97ed-125">此设置指示允许桌面应用。</span><span class="sxs-lookup"><span data-stu-id="c97ed-125">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="c97ed-126">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="c97ed-126">Default to true.</span></span>|
|<span data-ttu-id="c97ed-127">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="c97ed-127">startMenuLayoutXml</span></span>|<span data-ttu-id="c97ed-128">Binary</span><span class="sxs-lookup"><span data-stu-id="c97ed-128">Binary</span></span>|<span data-ttu-id="c97ed-129">允许管理员覆盖默认的 "开始" 布局，并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="c97ed-129">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="c97ed-130">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="c97ed-130"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="c97ed-131">XML 必须采用二进制格式。</span><span class="sxs-lookup"><span data-stu-id="c97ed-131">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c97ed-132">关系</span><span class="sxs-lookup"><span data-stu-id="c97ed-132">Relationships</span></span>
<span data-ttu-id="c97ed-133">无</span><span class="sxs-lookup"><span data-stu-id="c97ed-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c97ed-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c97ed-134">JSON Representation</span></span>
<span data-ttu-id="c97ed-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c97ed-135">Here is a JSON representation of the resource.</span></span>
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






