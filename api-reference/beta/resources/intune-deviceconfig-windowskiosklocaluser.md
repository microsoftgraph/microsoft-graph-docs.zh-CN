---
title: windowsKioskLocalUser 资源类型
description: 用于标识展台配置的本地帐户的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22db475ecb8cda48d4d73cba8ecb2145ae24a03a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061936"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="e5e35-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5e35-103">windowsKioskLocalUser resource type</span></span>

<span data-ttu-id="e5e35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5e35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5e35-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5e35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5e35-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5e35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5e35-107">用于标识展台配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="e5e35-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="e5e35-108">继承自 [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5e35-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5e35-109">属性</span><span class="sxs-lookup"><span data-stu-id="e5e35-109">Properties</span></span>
|<span data-ttu-id="e5e35-110">属性</span><span class="sxs-lookup"><span data-stu-id="e5e35-110">Property</span></span>|<span data-ttu-id="e5e35-111">类型</span><span class="sxs-lookup"><span data-stu-id="e5e35-111">Type</span></span>|<span data-ttu-id="e5e35-112">说明</span><span class="sxs-lookup"><span data-stu-id="e5e35-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5e35-113">userName</span><span class="sxs-lookup"><span data-stu-id="e5e35-113">userName</span></span>|<span data-ttu-id="e5e35-114">String</span><span class="sxs-lookup"><span data-stu-id="e5e35-114">String</span></span>|<span data-ttu-id="e5e35-115">将锁定到此展台配置的本地用户</span><span class="sxs-lookup"><span data-stu-id="e5e35-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5e35-116">关系</span><span class="sxs-lookup"><span data-stu-id="e5e35-116">Relationships</span></span>
<span data-ttu-id="e5e35-117">无</span><span class="sxs-lookup"><span data-stu-id="e5e35-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5e35-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5e35-118">JSON Representation</span></span>
<span data-ttu-id="e5e35-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5e35-119">Here is a JSON representation of the resource.</span></span>
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






