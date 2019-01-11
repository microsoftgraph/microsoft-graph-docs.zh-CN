---
title: windowsKioskLocalGroup 资源类型
description: 用于标识为网亭配置本地组的类
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dcc4f6ae47abf07ae259562b2aee72d187abd476
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807712"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="46b34-103">windowsKioskLocalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="46b34-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="46b34-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="46b34-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46b34-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="46b34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46b34-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="46b34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46b34-107">用于标识为网亭配置本地组的类</span><span class="sxs-lookup"><span data-stu-id="46b34-107">The class used to identify a local group for the kiosk configuration</span></span>

<span data-ttu-id="46b34-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="46b34-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46b34-109">属性</span><span class="sxs-lookup"><span data-stu-id="46b34-109">Properties</span></span>
|<span data-ttu-id="46b34-110">属性</span><span class="sxs-lookup"><span data-stu-id="46b34-110">Property</span></span>|<span data-ttu-id="46b34-111">类型</span><span class="sxs-lookup"><span data-stu-id="46b34-111">Type</span></span>|<span data-ttu-id="46b34-112">Description</span><span class="sxs-lookup"><span data-stu-id="46b34-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46b34-113">groupName</span><span class="sxs-lookup"><span data-stu-id="46b34-113">groupName</span></span>|<span data-ttu-id="46b34-114">字符串</span><span class="sxs-lookup"><span data-stu-id="46b34-114">String</span></span>|<span data-ttu-id="46b34-115">将锁定到此网亭配置本地组的名称</span><span class="sxs-lookup"><span data-stu-id="46b34-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="46b34-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="46b34-116">Relationships</span></span>
<span data-ttu-id="46b34-117">无</span><span class="sxs-lookup"><span data-stu-id="46b34-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46b34-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46b34-118">JSON Representation</span></span>
<span data-ttu-id="46b34-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46b34-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```





