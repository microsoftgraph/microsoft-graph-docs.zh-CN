---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6725e0a51ad9b4053278dcf03c91236a7d820665
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091017"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="7e713-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e713-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="7e713-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e713-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e713-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e713-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e713-106">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="7e713-106">Reset passcode action result</span></span>


<span data-ttu-id="7e713-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7e713-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e713-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e713-108">Properties</span></span>
|<span data-ttu-id="7e713-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e713-109">Property</span></span>|<span data-ttu-id="7e713-110">类型</span><span class="sxs-lookup"><span data-stu-id="7e713-110">Type</span></span>|<span data-ttu-id="7e713-111">说明</span><span class="sxs-lookup"><span data-stu-id="7e713-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e713-112">actionName</span><span class="sxs-lookup"><span data-stu-id="7e713-112">actionName</span></span>|<span data-ttu-id="7e713-113">String</span><span class="sxs-lookup"><span data-stu-id="7e713-113">String</span></span>|<span data-ttu-id="7e713-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7e713-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7e713-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7e713-115">actionState</span></span>|[<span data-ttu-id="7e713-116">actionState</span><span class="sxs-lookup"><span data-stu-id="7e713-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7e713-117">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7e713-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7e713-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7e713-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7e713-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7e713-119">startDateTime</span></span>|<span data-ttu-id="7e713-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e713-120">DateTimeOffset</span></span>|<span data-ttu-id="7e713-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7e713-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7e713-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e713-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="7e713-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e713-123">DateTimeOffset</span></span>|<span data-ttu-id="7e713-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7e713-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7e713-125">密码</span><span class="sxs-lookup"><span data-stu-id="7e713-125">passcode</span></span>|<span data-ttu-id="7e713-126">String</span><span class="sxs-lookup"><span data-stu-id="7e713-126">String</span></span>|<span data-ttu-id="7e713-127">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="7e713-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="7e713-128">关系</span><span class="sxs-lookup"><span data-stu-id="7e713-128">Relationships</span></span>
<span data-ttu-id="7e713-129">无</span><span class="sxs-lookup"><span data-stu-id="7e713-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e713-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e713-130">JSON Representation</span></span>
<span data-ttu-id="7e713-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e713-131">Here is a JSON representation of the resource.</span></span>
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
  "passcode": "String"
}
```









