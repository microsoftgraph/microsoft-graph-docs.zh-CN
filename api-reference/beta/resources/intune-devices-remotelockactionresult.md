---
title: remoteLockActionResult 资源类型
description: 锁定操作结果，包含用于解锁的 PIN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1c4e19212e5f4e54abf90cd22942160d0f1ce24
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611872"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="54d91-103">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="54d91-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="54d91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54d91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54d91-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54d91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54d91-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54d91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54d91-107">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="54d91-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="54d91-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54d91-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54d91-109">属性</span><span class="sxs-lookup"><span data-stu-id="54d91-109">Properties</span></span>
|<span data-ttu-id="54d91-110">属性</span><span class="sxs-lookup"><span data-stu-id="54d91-110">Property</span></span>|<span data-ttu-id="54d91-111">类型</span><span class="sxs-lookup"><span data-stu-id="54d91-111">Type</span></span>|<span data-ttu-id="54d91-112">Description</span><span class="sxs-lookup"><span data-stu-id="54d91-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54d91-113">actionName</span><span class="sxs-lookup"><span data-stu-id="54d91-113">actionName</span></span>|<span data-ttu-id="54d91-114">String</span><span class="sxs-lookup"><span data-stu-id="54d91-114">String</span></span>|<span data-ttu-id="54d91-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54d91-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="54d91-116">actionState</span><span class="sxs-lookup"><span data-stu-id="54d91-116">actionState</span></span>|[<span data-ttu-id="54d91-117">actionState</span><span class="sxs-lookup"><span data-stu-id="54d91-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="54d91-118">操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。</span><span class="sxs-lookup"><span data-stu-id="54d91-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="54d91-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="54d91-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="54d91-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="54d91-120">startDateTime</span></span>|<span data-ttu-id="54d91-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54d91-121">DateTimeOffset</span></span>|<span data-ttu-id="54d91-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54d91-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="54d91-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="54d91-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="54d91-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54d91-124">DateTimeOffset</span></span>|<span data-ttu-id="54d91-125">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54d91-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="54d91-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="54d91-126">unlockPin</span></span>|<span data-ttu-id="54d91-127">String</span><span class="sxs-lookup"><span data-stu-id="54d91-127">String</span></span>|<span data-ttu-id="54d91-128">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="54d91-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="54d91-129">关系</span><span class="sxs-lookup"><span data-stu-id="54d91-129">Relationships</span></span>
<span data-ttu-id="54d91-130">无</span><span class="sxs-lookup"><span data-stu-id="54d91-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54d91-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54d91-131">JSON Representation</span></span>
<span data-ttu-id="54d91-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54d91-132">Here is a JSON representation of the resource.</span></span>
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




