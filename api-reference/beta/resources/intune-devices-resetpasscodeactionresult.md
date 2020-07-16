---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35ffae18d564ccda9d54599833195ea845d654f4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788057"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="9b288-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b288-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="9b288-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b288-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b288-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b288-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b288-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b288-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b288-107">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="9b288-107">Reset passcode action result</span></span>


<span data-ttu-id="9b288-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b288-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b288-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b288-109">Properties</span></span>
|<span data-ttu-id="9b288-110">属性</span><span class="sxs-lookup"><span data-stu-id="9b288-110">Property</span></span>|<span data-ttu-id="9b288-111">类型</span><span class="sxs-lookup"><span data-stu-id="9b288-111">Type</span></span>|<span data-ttu-id="9b288-112">说明</span><span class="sxs-lookup"><span data-stu-id="9b288-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b288-113">actionName</span><span class="sxs-lookup"><span data-stu-id="9b288-113">actionName</span></span>|<span data-ttu-id="9b288-114">String</span><span class="sxs-lookup"><span data-stu-id="9b288-114">String</span></span>|<span data-ttu-id="9b288-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b288-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b288-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9b288-116">actionState</span></span>|[<span data-ttu-id="9b288-117">actionState</span><span class="sxs-lookup"><span data-stu-id="9b288-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9b288-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9b288-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9b288-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="9b288-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9b288-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b288-120">startDateTime</span></span>|<span data-ttu-id="9b288-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b288-121">DateTimeOffset</span></span>|<span data-ttu-id="9b288-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b288-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b288-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b288-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="9b288-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b288-124">DateTimeOffset</span></span>|<span data-ttu-id="9b288-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b288-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b288-126">密码</span><span class="sxs-lookup"><span data-stu-id="9b288-126">passcode</span></span>|<span data-ttu-id="9b288-127">String</span><span class="sxs-lookup"><span data-stu-id="9b288-127">String</span></span>|<span data-ttu-id="9b288-128">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="9b288-128">Newly generated passcode for the device</span></span> |
|<span data-ttu-id="9b288-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="9b288-129">errorCode</span></span>|<span data-ttu-id="9b288-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9b288-130">Int32</span></span>|<span data-ttu-id="9b288-131">RotateBitLockerKeys 操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="9b288-131">RotateBitLockerKeys action error code.</span></span> <span data-ttu-id="9b288-132">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="9b288-132">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b288-133">关系</span><span class="sxs-lookup"><span data-stu-id="9b288-133">Relationships</span></span>
<span data-ttu-id="9b288-134">无</span><span class="sxs-lookup"><span data-stu-id="9b288-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b288-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b288-135">JSON Representation</span></span>
<span data-ttu-id="9b288-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b288-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String",
  "errorCode": 1024
}
```



