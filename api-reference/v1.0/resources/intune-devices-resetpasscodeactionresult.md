---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 456bbc92dba168501fe3114e831665f8e2efce50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530286"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="2f034-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f034-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="2f034-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f034-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f034-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f034-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f034-106">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="2f034-106">Reset passcode action result</span></span>


<span data-ttu-id="2f034-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f034-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2f034-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f034-108">Properties</span></span>
|<span data-ttu-id="2f034-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f034-109">Property</span></span>|<span data-ttu-id="2f034-110">类型</span><span class="sxs-lookup"><span data-stu-id="2f034-110">Type</span></span>|<span data-ttu-id="2f034-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f034-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f034-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2f034-112">actionName</span></span>|<span data-ttu-id="2f034-113">字符串</span><span class="sxs-lookup"><span data-stu-id="2f034-113">String</span></span>|<span data-ttu-id="2f034-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f034-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f034-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2f034-115">actionState</span></span>|[<span data-ttu-id="2f034-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2f034-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="2f034-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2f034-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2f034-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="2f034-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2f034-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2f034-119">startDateTime</span></span>|<span data-ttu-id="2f034-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f034-120">DateTimeOffset</span></span>|<span data-ttu-id="2f034-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f034-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f034-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f034-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2f034-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f034-123">DateTimeOffset</span></span>|<span data-ttu-id="2f034-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f034-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f034-125">密码</span><span class="sxs-lookup"><span data-stu-id="2f034-125">passcode</span></span>|<span data-ttu-id="2f034-126">String</span><span class="sxs-lookup"><span data-stu-id="2f034-126">String</span></span>|<span data-ttu-id="2f034-127">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="2f034-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="2f034-128">关系</span><span class="sxs-lookup"><span data-stu-id="2f034-128">Relationships</span></span>
<span data-ttu-id="2f034-129">无</span><span class="sxs-lookup"><span data-stu-id="2f034-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f034-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f034-130">JSON Representation</span></span>
<span data-ttu-id="2f034-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f034-131">Here is a JSON representation of the resource.</span></span>
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




