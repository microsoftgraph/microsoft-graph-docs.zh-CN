---
title: windowsKioskLocalGroup 资源类型
description: 用于标识展台配置的本地组的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 661b1a4a6dd06fe44754232f967ebf8ec9c1ab55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969000"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="2c4bf-103">windowsKioskLocalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c4bf-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="2c4bf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c4bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c4bf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c4bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c4bf-106">用于标识展台配置的本地组的类</span><span class="sxs-lookup"><span data-stu-id="2c4bf-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="2c4bf-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="2c4bf-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c4bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c4bf-108">Properties</span></span>
|<span data-ttu-id="2c4bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="2c4bf-109">Property</span></span>|<span data-ttu-id="2c4bf-110">类型</span><span class="sxs-lookup"><span data-stu-id="2c4bf-110">Type</span></span>|<span data-ttu-id="2c4bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="2c4bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c4bf-112">名</span><span class="sxs-lookup"><span data-stu-id="2c4bf-112">groupName</span></span>|<span data-ttu-id="2c4bf-113">String</span><span class="sxs-lookup"><span data-stu-id="2c4bf-113">String</span></span>|<span data-ttu-id="2c4bf-114">将锁定到此展台配置的本地组的名称</span><span class="sxs-lookup"><span data-stu-id="2c4bf-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c4bf-115">关系</span><span class="sxs-lookup"><span data-stu-id="2c4bf-115">Relationships</span></span>
<span data-ttu-id="2c4bf-116">无</span><span class="sxs-lookup"><span data-stu-id="2c4bf-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c4bf-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c4bf-117">JSON Representation</span></span>
<span data-ttu-id="2c4bf-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c4bf-118">Here is a JSON representation of the resource.</span></span>
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





