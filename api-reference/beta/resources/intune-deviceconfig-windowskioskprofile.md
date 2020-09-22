---
title: windowsKioskProfile 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1fe6caea9eafc0c31f4befb6297fdc9ad5ffa3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061915"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="43055-103">windowsKioskProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="43055-103">windowsKioskProfile resource type</span></span>

<span data-ttu-id="43055-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43055-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43055-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43055-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43055-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43055-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43055-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="43055-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="43055-108">属性</span><span class="sxs-lookup"><span data-stu-id="43055-108">Properties</span></span>
|<span data-ttu-id="43055-109">属性</span><span class="sxs-lookup"><span data-stu-id="43055-109">Property</span></span>|<span data-ttu-id="43055-110">类型</span><span class="sxs-lookup"><span data-stu-id="43055-110">Type</span></span>|<span data-ttu-id="43055-111">说明</span><span class="sxs-lookup"><span data-stu-id="43055-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43055-112">profileId</span><span class="sxs-lookup"><span data-stu-id="43055-112">profileId</span></span>|<span data-ttu-id="43055-113">String</span><span class="sxs-lookup"><span data-stu-id="43055-113">String</span></span>|<span data-ttu-id="43055-114">实体的键。</span><span class="sxs-lookup"><span data-stu-id="43055-114">Key of the entity.</span></span>|
|<span data-ttu-id="43055-115">profileName</span><span class="sxs-lookup"><span data-stu-id="43055-115">profileName</span></span>|<span data-ttu-id="43055-116">String</span><span class="sxs-lookup"><span data-stu-id="43055-116">String</span></span>|<span data-ttu-id="43055-117">这是一个友好名称，用于标识一组应用程序、"开始" 菜单上这些应用程序的布局以及为其分配了此展台配置的用户。</span><span class="sxs-lookup"><span data-stu-id="43055-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="43055-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="43055-118">appConfiguration</span></span>|[<span data-ttu-id="43055-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="43055-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="43055-120">将用于此展台配置的应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="43055-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="43055-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="43055-121">userAccountsConfiguration</span></span>|<span data-ttu-id="43055-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43055-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="43055-123">将锁定到此展台配置的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="43055-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="43055-124">此集合最多可包含100个元素。</span><span class="sxs-lookup"><span data-stu-id="43055-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43055-125">关系</span><span class="sxs-lookup"><span data-stu-id="43055-125">Relationships</span></span>
<span data-ttu-id="43055-126">无</span><span class="sxs-lookup"><span data-stu-id="43055-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43055-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43055-127">JSON Representation</span></span>
<span data-ttu-id="43055-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43055-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
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
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```






