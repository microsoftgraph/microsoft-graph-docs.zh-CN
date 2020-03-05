---
title: windowsKioskLocalUser 资源类型
description: 用于标识展台配置的本地帐户的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e25c887c34008e0ffa001cfe713340ad9443f4dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525479"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="f657d-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f657d-103">windowsKioskLocalUser resource type</span></span>

<span data-ttu-id="f657d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f657d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f657d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f657d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f657d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f657d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f657d-107">用于标识展台配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="f657d-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="f657d-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="f657d-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f657d-109">属性</span><span class="sxs-lookup"><span data-stu-id="f657d-109">Properties</span></span>
|<span data-ttu-id="f657d-110">属性</span><span class="sxs-lookup"><span data-stu-id="f657d-110">Property</span></span>|<span data-ttu-id="f657d-111">类型</span><span class="sxs-lookup"><span data-stu-id="f657d-111">Type</span></span>|<span data-ttu-id="f657d-112">说明</span><span class="sxs-lookup"><span data-stu-id="f657d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f657d-113">userName</span><span class="sxs-lookup"><span data-stu-id="f657d-113">userName</span></span>|<span data-ttu-id="f657d-114">String</span><span class="sxs-lookup"><span data-stu-id="f657d-114">String</span></span>|<span data-ttu-id="f657d-115">将锁定到此展台配置的本地用户</span><span class="sxs-lookup"><span data-stu-id="f657d-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="f657d-116">关系</span><span class="sxs-lookup"><span data-stu-id="f657d-116">Relationships</span></span>
<span data-ttu-id="f657d-117">无</span><span class="sxs-lookup"><span data-stu-id="f657d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f657d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f657d-118">JSON Representation</span></span>
<span data-ttu-id="f657d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f657d-119">Here is a JSON representation of the resource.</span></span>
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



