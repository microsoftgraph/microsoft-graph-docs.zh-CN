---
title: rotateBitLockerKeysDeviceActionResult 资源类型
description: RotateBitLockerKeys 设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 527e90eab465045c5987830c08a6124ccacf16bf
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612040"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="f69be-103">rotateBitLockerKeysDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="f69be-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="f69be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f69be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f69be-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f69be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f69be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f69be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f69be-107">RotateBitLockerKeys 设备操作结果</span><span class="sxs-lookup"><span data-stu-id="f69be-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="f69be-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f69be-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f69be-109">属性</span><span class="sxs-lookup"><span data-stu-id="f69be-109">Properties</span></span>
|<span data-ttu-id="f69be-110">属性</span><span class="sxs-lookup"><span data-stu-id="f69be-110">Property</span></span>|<span data-ttu-id="f69be-111">类型</span><span class="sxs-lookup"><span data-stu-id="f69be-111">Type</span></span>|<span data-ttu-id="f69be-112">Description</span><span class="sxs-lookup"><span data-stu-id="f69be-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f69be-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f69be-113">actionName</span></span>|<span data-ttu-id="f69be-114">String</span><span class="sxs-lookup"><span data-stu-id="f69be-114">String</span></span>|<span data-ttu-id="f69be-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f69be-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f69be-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f69be-116">actionState</span></span>|[<span data-ttu-id="f69be-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f69be-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="f69be-118">操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。</span><span class="sxs-lookup"><span data-stu-id="f69be-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f69be-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="f69be-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f69be-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f69be-120">startDateTime</span></span>|<span data-ttu-id="f69be-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f69be-121">DateTimeOffset</span></span>|<span data-ttu-id="f69be-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f69be-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f69be-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f69be-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f69be-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f69be-124">DateTimeOffset</span></span>|<span data-ttu-id="f69be-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f69be-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f69be-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="f69be-126">errorCode</span></span>|<span data-ttu-id="f69be-127">Int32</span><span class="sxs-lookup"><span data-stu-id="f69be-127">Int32</span></span>|<span data-ttu-id="f69be-128">RotateBitLockerKeys 操作错误代码</span><span class="sxs-lookup"><span data-stu-id="f69be-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="f69be-129">关系</span><span class="sxs-lookup"><span data-stu-id="f69be-129">Relationships</span></span>
<span data-ttu-id="f69be-130">无</span><span class="sxs-lookup"><span data-stu-id="f69be-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f69be-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f69be-131">JSON Representation</span></span>
<span data-ttu-id="f69be-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f69be-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rotateBitLockerKeysDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rotateBitLockerKeysDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```




