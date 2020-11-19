---
title: windowsKioskProfile 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c69c8d32be23dccc935d1de74b0a450850091722
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268214"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="12216-103">windowsKioskProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="12216-103">windowsKioskProfile resource type</span></span>

<span data-ttu-id="12216-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12216-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12216-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12216-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12216-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12216-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12216-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12216-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="12216-108">属性</span><span class="sxs-lookup"><span data-stu-id="12216-108">Properties</span></span>
|<span data-ttu-id="12216-109">属性</span><span class="sxs-lookup"><span data-stu-id="12216-109">Property</span></span>|<span data-ttu-id="12216-110">类型</span><span class="sxs-lookup"><span data-stu-id="12216-110">Type</span></span>|<span data-ttu-id="12216-111">说明</span><span class="sxs-lookup"><span data-stu-id="12216-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12216-112">profileId</span><span class="sxs-lookup"><span data-stu-id="12216-112">profileId</span></span>|<span data-ttu-id="12216-113">String</span><span class="sxs-lookup"><span data-stu-id="12216-113">String</span></span>|<span data-ttu-id="12216-114">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12216-114">Key of the entity.</span></span>|
|<span data-ttu-id="12216-115">profileName</span><span class="sxs-lookup"><span data-stu-id="12216-115">profileName</span></span>|<span data-ttu-id="12216-116">字符串</span><span class="sxs-lookup"><span data-stu-id="12216-116">String</span></span>|<span data-ttu-id="12216-117">这是一个友好名称，用于标识一组应用程序、"开始" 菜单上这些应用程序的布局以及为其分配了此展台配置的用户。</span><span class="sxs-lookup"><span data-stu-id="12216-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="12216-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="12216-118">appConfiguration</span></span>|[<span data-ttu-id="12216-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12216-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="12216-120">将用于此展台配置的应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="12216-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="12216-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="12216-121">userAccountsConfiguration</span></span>|<span data-ttu-id="12216-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12216-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="12216-123">将锁定到此展台配置的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="12216-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="12216-124">此集合最多可包含100个元素。</span><span class="sxs-lookup"><span data-stu-id="12216-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12216-125">关系</span><span class="sxs-lookup"><span data-stu-id="12216-125">Relationships</span></span>
<span data-ttu-id="12216-126">无</span><span class="sxs-lookup"><span data-stu-id="12216-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12216-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12216-127">JSON Representation</span></span>
<span data-ttu-id="12216-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12216-128">Here is a JSON representation of the resource.</span></span>
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




