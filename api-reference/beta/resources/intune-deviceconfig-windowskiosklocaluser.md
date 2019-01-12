---
title: windowsKioskLocalUser 资源类型
description: 用于标识网亭配置的本地帐户的类
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2dc1e54f7bc4e9fbbef3113abce90cab00825be8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934630"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="41d9a-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="41d9a-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="41d9a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="41d9a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41d9a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41d9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41d9a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="41d9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41d9a-107">用于标识网亭配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="41d9a-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="41d9a-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="41d9a-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="41d9a-109">属性</span><span class="sxs-lookup"><span data-stu-id="41d9a-109">Properties</span></span>
|<span data-ttu-id="41d9a-110">属性</span><span class="sxs-lookup"><span data-stu-id="41d9a-110">Property</span></span>|<span data-ttu-id="41d9a-111">类型</span><span class="sxs-lookup"><span data-stu-id="41d9a-111">Type</span></span>|<span data-ttu-id="41d9a-112">Description</span><span class="sxs-lookup"><span data-stu-id="41d9a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d9a-113">userName</span><span class="sxs-lookup"><span data-stu-id="41d9a-113">userName</span></span>|<span data-ttu-id="41d9a-114">String</span><span class="sxs-lookup"><span data-stu-id="41d9a-114">String</span></span>|<span data-ttu-id="41d9a-115">将锁定到此网亭配置本地用户</span><span class="sxs-lookup"><span data-stu-id="41d9a-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="41d9a-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="41d9a-116">Relationships</span></span>
<span data-ttu-id="41d9a-117">无</span><span class="sxs-lookup"><span data-stu-id="41d9a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="41d9a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41d9a-118">JSON Representation</span></span>
<span data-ttu-id="41d9a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41d9a-119">Here is a JSON representation of the resource.</span></span>
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





