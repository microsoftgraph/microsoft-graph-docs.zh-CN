---
title: windowsKioskProfile 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55d8c23d3bfae2baf9d632c33390b8aafb5e7ef8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420246"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="7081d-103">windowsKioskProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="7081d-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="7081d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7081d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7081d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7081d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7081d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7081d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7081d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7081d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7081d-108">属性</span><span class="sxs-lookup"><span data-stu-id="7081d-108">Properties</span></span>
|<span data-ttu-id="7081d-109">属性</span><span class="sxs-lookup"><span data-stu-id="7081d-109">Property</span></span>|<span data-ttu-id="7081d-110">类型</span><span class="sxs-lookup"><span data-stu-id="7081d-110">Type</span></span>|<span data-ttu-id="7081d-111">说明</span><span class="sxs-lookup"><span data-stu-id="7081d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7081d-112">档案 Id</span><span class="sxs-lookup"><span data-stu-id="7081d-112">profileId</span></span>|<span data-ttu-id="7081d-113">String</span><span class="sxs-lookup"><span data-stu-id="7081d-113">String</span></span>|<span data-ttu-id="7081d-114">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7081d-114">Key of the entity.</span></span>|
|<span data-ttu-id="7081d-115">profileName</span><span class="sxs-lookup"><span data-stu-id="7081d-115">profileName</span></span>|<span data-ttu-id="7081d-116">String</span><span class="sxs-lookup"><span data-stu-id="7081d-116">String</span></span>|<span data-ttu-id="7081d-117">这是用于标识一组应用程序，在开始菜单和用户为其分配此网亭配置这些应用程序的布局的友好名称。</span><span class="sxs-lookup"><span data-stu-id="7081d-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="7081d-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="7081d-118">appConfiguration</span></span>|[<span data-ttu-id="7081d-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7081d-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="7081d-120">将用于此网亭配置应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="7081d-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="7081d-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="7081d-121">userAccountsConfiguration</span></span>|<span data-ttu-id="7081d-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="7081d-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="7081d-123">将锁定到此网亭配置用户帐户。</span><span class="sxs-lookup"><span data-stu-id="7081d-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="7081d-124">此集合可以包含 100 个元素的最大值。</span><span class="sxs-lookup"><span data-stu-id="7081d-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7081d-125">关系</span><span class="sxs-lookup"><span data-stu-id="7081d-125">Relationships</span></span>
<span data-ttu-id="7081d-126">无</span><span class="sxs-lookup"><span data-stu-id="7081d-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7081d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7081d-127">JSON Representation</span></span>
<span data-ttu-id="7081d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7081d-128">Here is a JSON representation of the resource.</span></span>
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
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
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




