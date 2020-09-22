---
title: windowsKioskSingleUWPApp 资源类型
description: 用于标识您的展台配置的 UWP 应用信息的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3b6142091183409d0fea45d42a0241e9f41f446b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061887"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="23b64-103">windowsKioskSingleUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="23b64-103">windowsKioskSingleUWPApp resource type</span></span>

<span data-ttu-id="23b64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23b64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23b64-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23b64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23b64-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23b64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23b64-107">用于标识您的展台配置的 UWP 应用信息的类</span><span class="sxs-lookup"><span data-stu-id="23b64-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="23b64-108">继承自 [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b64-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23b64-109">属性</span><span class="sxs-lookup"><span data-stu-id="23b64-109">Properties</span></span>
|<span data-ttu-id="23b64-110">属性</span><span class="sxs-lookup"><span data-stu-id="23b64-110">Property</span></span>|<span data-ttu-id="23b64-111">类型</span><span class="sxs-lookup"><span data-stu-id="23b64-111">Type</span></span>|<span data-ttu-id="23b64-112">说明</span><span class="sxs-lookup"><span data-stu-id="23b64-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23b64-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="23b64-113">uwpApp</span></span>|[<span data-ttu-id="23b64-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="23b64-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="23b64-115">这是在展台模式下可用于启动使用的唯一应用程序用户模型 ID (AUMID) </span><span class="sxs-lookup"><span data-stu-id="23b64-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="23b64-116">关系</span><span class="sxs-lookup"><span data-stu-id="23b64-116">Relationships</span></span>
<span data-ttu-id="23b64-117">无</span><span class="sxs-lookup"><span data-stu-id="23b64-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23b64-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23b64-118">JSON Representation</span></span>
<span data-ttu-id="23b64-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23b64-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```






