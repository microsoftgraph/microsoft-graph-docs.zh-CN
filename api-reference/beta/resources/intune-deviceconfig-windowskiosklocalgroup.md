---
title: windowsKioskLocalGroup 资源类型
description: 用于标识展台配置的本地组的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ab9875759c8610f976e4aaa7cc5fc8733b20ee0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943856"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="34d7b-103">windowsKioskLocalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="34d7b-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="34d7b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34d7b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34d7b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34d7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34d7b-106">用于标识展台配置的本地组的类</span><span class="sxs-lookup"><span data-stu-id="34d7b-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="34d7b-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="34d7b-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34d7b-108">属性</span><span class="sxs-lookup"><span data-stu-id="34d7b-108">Properties</span></span>
|<span data-ttu-id="34d7b-109">属性</span><span class="sxs-lookup"><span data-stu-id="34d7b-109">Property</span></span>|<span data-ttu-id="34d7b-110">类型</span><span class="sxs-lookup"><span data-stu-id="34d7b-110">Type</span></span>|<span data-ttu-id="34d7b-111">说明</span><span class="sxs-lookup"><span data-stu-id="34d7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34d7b-112">名</span><span class="sxs-lookup"><span data-stu-id="34d7b-112">groupName</span></span>|<span data-ttu-id="34d7b-113">String</span><span class="sxs-lookup"><span data-stu-id="34d7b-113">String</span></span>|<span data-ttu-id="34d7b-114">将锁定到此展台配置的本地组的名称</span><span class="sxs-lookup"><span data-stu-id="34d7b-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="34d7b-115">关系</span><span class="sxs-lookup"><span data-stu-id="34d7b-115">Relationships</span></span>
<span data-ttu-id="34d7b-116">无</span><span class="sxs-lookup"><span data-stu-id="34d7b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34d7b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34d7b-117">JSON Representation</span></span>
<span data-ttu-id="34d7b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34d7b-118">Here is a JSON representation of the resource.</span></span>
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




