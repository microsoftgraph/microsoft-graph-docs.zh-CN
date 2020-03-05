---
title: windowsKioskLocalGroup 资源类型
description: 用于标识展台配置的本地组的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52a7295a6a0c0d157ac8200c8de367cf67103bb6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525486"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="c9a47-103">windowsKioskLocalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9a47-103">windowsKioskLocalGroup resource type</span></span>

<span data-ttu-id="c9a47-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c9a47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9a47-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9a47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9a47-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9a47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9a47-107">用于标识展台配置的本地组的类</span><span class="sxs-lookup"><span data-stu-id="c9a47-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="c9a47-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c9a47-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9a47-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9a47-109">Properties</span></span>
|<span data-ttu-id="c9a47-110">属性</span><span class="sxs-lookup"><span data-stu-id="c9a47-110">Property</span></span>|<span data-ttu-id="c9a47-111">类型</span><span class="sxs-lookup"><span data-stu-id="c9a47-111">Type</span></span>|<span data-ttu-id="c9a47-112">说明</span><span class="sxs-lookup"><span data-stu-id="c9a47-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9a47-113">名</span><span class="sxs-lookup"><span data-stu-id="c9a47-113">groupName</span></span>|<span data-ttu-id="c9a47-114">String</span><span class="sxs-lookup"><span data-stu-id="c9a47-114">String</span></span>|<span data-ttu-id="c9a47-115">将锁定到此展台配置的本地组的名称</span><span class="sxs-lookup"><span data-stu-id="c9a47-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9a47-116">关系</span><span class="sxs-lookup"><span data-stu-id="c9a47-116">Relationships</span></span>
<span data-ttu-id="c9a47-117">无</span><span class="sxs-lookup"><span data-stu-id="c9a47-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9a47-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9a47-118">JSON Representation</span></span>
<span data-ttu-id="c9a47-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9a47-119">Here is a JSON representation of the resource.</span></span>
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



