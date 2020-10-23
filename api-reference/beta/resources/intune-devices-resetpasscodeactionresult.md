---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a8d38fc68a9ce02645892810bc4029ea126198d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691328"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="c33dc-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="c33dc-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="c33dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c33dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c33dc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c33dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c33dc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c33dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c33dc-107">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="c33dc-107">Reset passcode action result</span></span>


<span data-ttu-id="c33dc-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c33dc-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c33dc-109">属性</span><span class="sxs-lookup"><span data-stu-id="c33dc-109">Properties</span></span>
|<span data-ttu-id="c33dc-110">属性</span><span class="sxs-lookup"><span data-stu-id="c33dc-110">Property</span></span>|<span data-ttu-id="c33dc-111">类型</span><span class="sxs-lookup"><span data-stu-id="c33dc-111">Type</span></span>|<span data-ttu-id="c33dc-112">说明</span><span class="sxs-lookup"><span data-stu-id="c33dc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c33dc-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c33dc-113">actionName</span></span>|<span data-ttu-id="c33dc-114">String</span><span class="sxs-lookup"><span data-stu-id="c33dc-114">String</span></span>|<span data-ttu-id="c33dc-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c33dc-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c33dc-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c33dc-116">actionState</span></span>|[<span data-ttu-id="c33dc-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c33dc-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c33dc-118">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="c33dc-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c33dc-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="c33dc-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c33dc-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c33dc-120">startDateTime</span></span>|<span data-ttu-id="c33dc-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c33dc-121">DateTimeOffset</span></span>|<span data-ttu-id="c33dc-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c33dc-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c33dc-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c33dc-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c33dc-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c33dc-124">DateTimeOffset</span></span>|<span data-ttu-id="c33dc-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c33dc-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c33dc-126">密码</span><span class="sxs-lookup"><span data-stu-id="c33dc-126">passcode</span></span>|<span data-ttu-id="c33dc-127">String</span><span class="sxs-lookup"><span data-stu-id="c33dc-127">String</span></span>|<span data-ttu-id="c33dc-128">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="c33dc-128">Newly generated passcode for the device</span></span> |
|<span data-ttu-id="c33dc-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="c33dc-129">errorCode</span></span>|<span data-ttu-id="c33dc-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c33dc-130">Int32</span></span>|<span data-ttu-id="c33dc-131">RotateBitLockerKeys 操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="c33dc-131">RotateBitLockerKeys action error code.</span></span> <span data-ttu-id="c33dc-132">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="c33dc-132">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="c33dc-133">关系</span><span class="sxs-lookup"><span data-stu-id="c33dc-133">Relationships</span></span>
<span data-ttu-id="c33dc-134">无</span><span class="sxs-lookup"><span data-stu-id="c33dc-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c33dc-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c33dc-135">JSON Representation</span></span>
<span data-ttu-id="c33dc-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c33dc-136">Here is a JSON representation of the resource.</span></span>
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





