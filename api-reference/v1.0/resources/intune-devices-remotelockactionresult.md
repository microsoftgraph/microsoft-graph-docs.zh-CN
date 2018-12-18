---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: tfitzmac
ms.openlocfilehash: 44d56b2ee20629d1cefbf965c72e5f6cc17fb0a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353688"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="8c8da-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c8da-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="8c8da-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c8da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c8da-105">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="8c8da-105">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="8c8da-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c8da-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c8da-107">属性</span><span class="sxs-lookup"><span data-stu-id="8c8da-107">Properties</span></span>
|<span data-ttu-id="8c8da-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c8da-108">Property</span></span>|<span data-ttu-id="8c8da-109">类型</span><span class="sxs-lookup"><span data-stu-id="8c8da-109">Type</span></span>|<span data-ttu-id="8c8da-110">说明</span><span class="sxs-lookup"><span data-stu-id="8c8da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c8da-111">actionName</span><span class="sxs-lookup"><span data-stu-id="8c8da-111">actionName</span></span>|<span data-ttu-id="8c8da-112">String</span><span class="sxs-lookup"><span data-stu-id="8c8da-112">String</span></span>|<span data-ttu-id="8c8da-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c8da-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8c8da-114">actionState</span><span class="sxs-lookup"><span data-stu-id="8c8da-114">actionState</span></span>|[<span data-ttu-id="8c8da-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8c8da-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="8c8da-116">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8c8da-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8c8da-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="8c8da-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8c8da-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8c8da-118">startDateTime</span></span>|<span data-ttu-id="8c8da-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c8da-119">DateTimeOffset</span></span>|<span data-ttu-id="8c8da-120">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c8da-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8c8da-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c8da-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="8c8da-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c8da-122">DateTimeOffset</span></span>|<span data-ttu-id="8c8da-123">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c8da-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8c8da-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="8c8da-124">unlockPin</span></span>|<span data-ttu-id="8c8da-125">String</span><span class="sxs-lookup"><span data-stu-id="8c8da-125">String</span></span>|<span data-ttu-id="8c8da-126">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="8c8da-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c8da-127">关系</span><span class="sxs-lookup"><span data-stu-id="8c8da-127">Relationships</span></span>
<span data-ttu-id="8c8da-128">无</span><span class="sxs-lookup"><span data-stu-id="8c8da-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c8da-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c8da-129">JSON Representation</span></span>
<span data-ttu-id="8c8da-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c8da-130">Here is a JSON representation of the resource.</span></span>
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



