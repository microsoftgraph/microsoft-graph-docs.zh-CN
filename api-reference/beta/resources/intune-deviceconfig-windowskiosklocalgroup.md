---
title: windowsKioskLocalGroup 资源类型
description: 用于标识展台配置的本地组的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd26b8e7d7649d832e844ee9c6a0a68e7ed9cd5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039760"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="42d38-103">windowsKioskLocalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="42d38-103">windowsKioskLocalGroup resource type</span></span>

<span data-ttu-id="42d38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42d38-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42d38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42d38-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42d38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d38-107">用于标识展台配置的本地组的类</span><span class="sxs-lookup"><span data-stu-id="42d38-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="42d38-108">继承自 [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="42d38-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42d38-109">属性</span><span class="sxs-lookup"><span data-stu-id="42d38-109">Properties</span></span>
|<span data-ttu-id="42d38-110">属性</span><span class="sxs-lookup"><span data-stu-id="42d38-110">Property</span></span>|<span data-ttu-id="42d38-111">类型</span><span class="sxs-lookup"><span data-stu-id="42d38-111">Type</span></span>|<span data-ttu-id="42d38-112">说明</span><span class="sxs-lookup"><span data-stu-id="42d38-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d38-113">名</span><span class="sxs-lookup"><span data-stu-id="42d38-113">groupName</span></span>|<span data-ttu-id="42d38-114">String</span><span class="sxs-lookup"><span data-stu-id="42d38-114">String</span></span>|<span data-ttu-id="42d38-115">将锁定到此展台配置的本地组的名称</span><span class="sxs-lookup"><span data-stu-id="42d38-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d38-116">关系</span><span class="sxs-lookup"><span data-stu-id="42d38-116">Relationships</span></span>
<span data-ttu-id="42d38-117">无</span><span class="sxs-lookup"><span data-stu-id="42d38-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42d38-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42d38-118">JSON Representation</span></span>
<span data-ttu-id="42d38-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42d38-119">Here is a JSON representation of the resource.</span></span>
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






