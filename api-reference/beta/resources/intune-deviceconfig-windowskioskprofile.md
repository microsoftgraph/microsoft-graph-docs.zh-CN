---
title: windowsKioskProfile 资源类型
description: 尚未记录
ms.openlocfilehash: 074c6caa9b632016f092f67192064ae18e9dcce3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043264"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="7ec64-103">windowsKioskProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ec64-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="7ec64-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ec64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ec64-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ec64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ec64-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ec64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ec64-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7ec64-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7ec64-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ec64-108">Properties</span></span>
|<span data-ttu-id="7ec64-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ec64-109">Property</span></span>|<span data-ttu-id="7ec64-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ec64-110">Type</span></span>|<span data-ttu-id="7ec64-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ec64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ec64-112">档案 Id</span><span class="sxs-lookup"><span data-stu-id="7ec64-112">profileId</span></span>|<span data-ttu-id="7ec64-113">String</span><span class="sxs-lookup"><span data-stu-id="7ec64-113">String</span></span>|<span data-ttu-id="7ec64-114">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ec64-114">Key of the entity.</span></span>|
|<span data-ttu-id="7ec64-115">profileName</span><span class="sxs-lookup"><span data-stu-id="7ec64-115">profileName</span></span>|<span data-ttu-id="7ec64-116">字符串</span><span class="sxs-lookup"><span data-stu-id="7ec64-116">String</span></span>|<span data-ttu-id="7ec64-117">这是用于标识一组应用程序，在开始菜单和用户为其分配此网亭配置这些应用程序的布局的友好名称。</span><span class="sxs-lookup"><span data-stu-id="7ec64-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="7ec64-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ec64-118">appConfiguration</span></span>|[<span data-ttu-id="7ec64-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ec64-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="7ec64-120">将用于此网亭配置应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="7ec64-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="7ec64-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ec64-121">userAccountsConfiguration</span></span>|<span data-ttu-id="7ec64-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ec64-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="7ec64-123">将锁定到此网亭配置用户帐户。</span><span class="sxs-lookup"><span data-stu-id="7ec64-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="7ec64-124">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7ec64-124">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ec64-125">关系</span><span class="sxs-lookup"><span data-stu-id="7ec64-125">Relationships</span></span>
<span data-ttu-id="7ec64-126">无</span><span class="sxs-lookup"><span data-stu-id="7ec64-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ec64-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ec64-127">JSON Representation</span></span>
<span data-ttu-id="7ec64-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ec64-128">Here is a JSON representation of the resource.</span></span>
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





