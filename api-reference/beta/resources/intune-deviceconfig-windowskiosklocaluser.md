---
title: windowsKioskLocalUser 资源类型
description: 用于标识网亭配置的本地帐户的类
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7ab6a9dc0e3ea63ed5d9f60bb48b005aa98acab1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844553"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="f4f3b-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4f3b-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="f4f3b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f4f3b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4f3b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f4f3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4f3b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f4f3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4f3b-107">用于标识网亭配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="f4f3b-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="f4f3b-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="f4f3b-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4f3b-109">属性</span><span class="sxs-lookup"><span data-stu-id="f4f3b-109">Properties</span></span>
|<span data-ttu-id="f4f3b-110">属性</span><span class="sxs-lookup"><span data-stu-id="f4f3b-110">Property</span></span>|<span data-ttu-id="f4f3b-111">类型</span><span class="sxs-lookup"><span data-stu-id="f4f3b-111">Type</span></span>|<span data-ttu-id="f4f3b-112">Description</span><span class="sxs-lookup"><span data-stu-id="f4f3b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f3b-113">userName</span><span class="sxs-lookup"><span data-stu-id="f4f3b-113">userName</span></span>|<span data-ttu-id="f4f3b-114">String</span><span class="sxs-lookup"><span data-stu-id="f4f3b-114">String</span></span>|<span data-ttu-id="f4f3b-115">将锁定到此网亭配置本地用户</span><span class="sxs-lookup"><span data-stu-id="f4f3b-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4f3b-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="f4f3b-116">Relationships</span></span>
<span data-ttu-id="f4f3b-117">无</span><span class="sxs-lookup"><span data-stu-id="f4f3b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f4f3b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4f3b-118">JSON Representation</span></span>
<span data-ttu-id="f4f3b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4f3b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





