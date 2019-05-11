---
title: windowsKioskProfile 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ac91647d652b6e1124932806fd9ab83414b497a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943996"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="56a9e-103">windowsKioskProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="56a9e-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="56a9e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56a9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56a9e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56a9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56a9e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="56a9e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="56a9e-107">属性</span><span class="sxs-lookup"><span data-stu-id="56a9e-107">Properties</span></span>
|<span data-ttu-id="56a9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="56a9e-108">Property</span></span>|<span data-ttu-id="56a9e-109">类型</span><span class="sxs-lookup"><span data-stu-id="56a9e-109">Type</span></span>|<span data-ttu-id="56a9e-110">说明</span><span class="sxs-lookup"><span data-stu-id="56a9e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a9e-111">profileId</span><span class="sxs-lookup"><span data-stu-id="56a9e-111">profileId</span></span>|<span data-ttu-id="56a9e-112">String</span><span class="sxs-lookup"><span data-stu-id="56a9e-112">String</span></span>|<span data-ttu-id="56a9e-113">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56a9e-113">Key of the entity.</span></span>|
|<span data-ttu-id="56a9e-114">profileName</span><span class="sxs-lookup"><span data-stu-id="56a9e-114">profileName</span></span>|<span data-ttu-id="56a9e-115">String</span><span class="sxs-lookup"><span data-stu-id="56a9e-115">String</span></span>|<span data-ttu-id="56a9e-116">这是一个友好名称, 用于标识一组应用程序、"开始" 菜单上这些应用程序的布局以及为其分配了此展台配置的用户。</span><span class="sxs-lookup"><span data-stu-id="56a9e-116">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="56a9e-117">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="56a9e-117">appConfiguration</span></span>|[<span data-ttu-id="56a9e-118">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="56a9e-118">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="56a9e-119">将用于此展台配置的应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="56a9e-119">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="56a9e-120">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="56a9e-120">userAccountsConfiguration</span></span>|<span data-ttu-id="56a9e-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="56a9e-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="56a9e-122">将锁定到此展台配置的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="56a9e-122">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="56a9e-123">此集合最多可包含100个元素。</span><span class="sxs-lookup"><span data-stu-id="56a9e-123">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56a9e-124">关系</span><span class="sxs-lookup"><span data-stu-id="56a9e-124">Relationships</span></span>
<span data-ttu-id="56a9e-125">无</span><span class="sxs-lookup"><span data-stu-id="56a9e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56a9e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56a9e-126">JSON Representation</span></span>
<span data-ttu-id="56a9e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56a9e-127">Here is a JSON representation of the resource.</span></span>
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




