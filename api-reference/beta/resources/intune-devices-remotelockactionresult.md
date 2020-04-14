---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db6ce9d84ad2e280ea562101eab77a83f2f1964f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448111"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="f9492-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9492-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="f9492-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9492-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9492-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9492-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9492-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9492-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9492-107">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="f9492-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="f9492-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f9492-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f9492-109">属性</span><span class="sxs-lookup"><span data-stu-id="f9492-109">Properties</span></span>
|<span data-ttu-id="f9492-110">属性</span><span class="sxs-lookup"><span data-stu-id="f9492-110">Property</span></span>|<span data-ttu-id="f9492-111">类型</span><span class="sxs-lookup"><span data-stu-id="f9492-111">Type</span></span>|<span data-ttu-id="f9492-112">说明</span><span class="sxs-lookup"><span data-stu-id="f9492-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9492-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f9492-113">actionName</span></span>|<span data-ttu-id="f9492-114">String</span><span class="sxs-lookup"><span data-stu-id="f9492-114">String</span></span>|<span data-ttu-id="f9492-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f9492-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f9492-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f9492-116">actionState</span></span>|[<span data-ttu-id="f9492-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f9492-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f9492-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f9492-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f9492-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="f9492-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f9492-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f9492-120">startDateTime</span></span>|<span data-ttu-id="f9492-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9492-121">DateTimeOffset</span></span>|<span data-ttu-id="f9492-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f9492-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f9492-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9492-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f9492-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9492-124">DateTimeOffset</span></span>|<span data-ttu-id="f9492-125">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f9492-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f9492-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="f9492-126">unlockPin</span></span>|<span data-ttu-id="f9492-127">String</span><span class="sxs-lookup"><span data-stu-id="f9492-127">String</span></span>|<span data-ttu-id="f9492-128">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="f9492-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9492-129">关系</span><span class="sxs-lookup"><span data-stu-id="f9492-129">Relationships</span></span>
<span data-ttu-id="f9492-130">无</span><span class="sxs-lookup"><span data-stu-id="f9492-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9492-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9492-131">JSON Representation</span></span>
<span data-ttu-id="f9492-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9492-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



