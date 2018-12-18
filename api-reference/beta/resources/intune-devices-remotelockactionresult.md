---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: tfitzmac
ms.openlocfilehash: 9cde6019329be909e688bbc1b7a568aa3a9e7781
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324890"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="dfde3-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfde3-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="dfde3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dfde3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfde3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dfde3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfde3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dfde3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfde3-107">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="dfde3-107">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="dfde3-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dfde3-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dfde3-109">属性</span><span class="sxs-lookup"><span data-stu-id="dfde3-109">Properties</span></span>
|<span data-ttu-id="dfde3-110">属性</span><span class="sxs-lookup"><span data-stu-id="dfde3-110">Property</span></span>|<span data-ttu-id="dfde3-111">类型</span><span class="sxs-lookup"><span data-stu-id="dfde3-111">Type</span></span>|<span data-ttu-id="dfde3-112">说明</span><span class="sxs-lookup"><span data-stu-id="dfde3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfde3-113">actionName</span><span class="sxs-lookup"><span data-stu-id="dfde3-113">actionName</span></span>|<span data-ttu-id="dfde3-114">String</span><span class="sxs-lookup"><span data-stu-id="dfde3-114">String</span></span>|<span data-ttu-id="dfde3-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dfde3-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="dfde3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="dfde3-116">actionState</span></span>|[<span data-ttu-id="dfde3-117">actionState</span><span class="sxs-lookup"><span data-stu-id="dfde3-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="dfde3-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="dfde3-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="dfde3-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="dfde3-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="dfde3-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dfde3-120">startDateTime</span></span>|<span data-ttu-id="dfde3-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfde3-121">DateTimeOffset</span></span>|<span data-ttu-id="dfde3-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dfde3-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="dfde3-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfde3-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="dfde3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfde3-124">DateTimeOffset</span></span>|<span data-ttu-id="dfde3-125">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dfde3-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="dfde3-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="dfde3-126">unlockPin</span></span>|<span data-ttu-id="dfde3-127">String</span><span class="sxs-lookup"><span data-stu-id="dfde3-127">String</span></span>|<span data-ttu-id="dfde3-128">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="dfde3-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfde3-129">关系</span><span class="sxs-lookup"><span data-stu-id="dfde3-129">Relationships</span></span>
<span data-ttu-id="dfde3-130">无</span><span class="sxs-lookup"><span data-stu-id="dfde3-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfde3-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfde3-131">JSON Representation</span></span>
<span data-ttu-id="dfde3-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfde3-132">Here is a JSON representation of the resource.</span></span>
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





