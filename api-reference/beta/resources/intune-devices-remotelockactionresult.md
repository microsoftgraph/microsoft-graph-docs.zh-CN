---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e57949e689f3d8e26c5217acec1a36662145b1a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416466"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="f98a9-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="f98a9-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="f98a9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f98a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f98a9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f98a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f98a9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f98a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f98a9-107">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="f98a9-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="f98a9-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f98a9-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f98a9-109">属性</span><span class="sxs-lookup"><span data-stu-id="f98a9-109">Properties</span></span>
|<span data-ttu-id="f98a9-110">属性</span><span class="sxs-lookup"><span data-stu-id="f98a9-110">Property</span></span>|<span data-ttu-id="f98a9-111">类型</span><span class="sxs-lookup"><span data-stu-id="f98a9-111">Type</span></span>|<span data-ttu-id="f98a9-112">说明</span><span class="sxs-lookup"><span data-stu-id="f98a9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f98a9-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f98a9-113">actionName</span></span>|<span data-ttu-id="f98a9-114">String</span><span class="sxs-lookup"><span data-stu-id="f98a9-114">String</span></span>|<span data-ttu-id="f98a9-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f98a9-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f98a9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f98a9-116">actionState</span></span>|[<span data-ttu-id="f98a9-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f98a9-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f98a9-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f98a9-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f98a9-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="f98a9-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f98a9-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f98a9-120">startDateTime</span></span>|<span data-ttu-id="f98a9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f98a9-121">DateTimeOffset</span></span>|<span data-ttu-id="f98a9-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f98a9-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f98a9-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f98a9-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f98a9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f98a9-124">DateTimeOffset</span></span>|<span data-ttu-id="f98a9-125">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f98a9-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f98a9-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="f98a9-126">unlockPin</span></span>|<span data-ttu-id="f98a9-127">String</span><span class="sxs-lookup"><span data-stu-id="f98a9-127">String</span></span>|<span data-ttu-id="f98a9-128">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="f98a9-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="f98a9-129">关系</span><span class="sxs-lookup"><span data-stu-id="f98a9-129">Relationships</span></span>
<span data-ttu-id="f98a9-130">无</span><span class="sxs-lookup"><span data-stu-id="f98a9-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f98a9-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f98a9-131">JSON Representation</span></span>
<span data-ttu-id="f98a9-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f98a9-132">Here is a JSON representation of the resource.</span></span>
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




