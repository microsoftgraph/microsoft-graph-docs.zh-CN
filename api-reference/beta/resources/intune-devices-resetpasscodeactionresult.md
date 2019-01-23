---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5c022d2531bd1576ab7e336193d2f488f5f89f98
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407044"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="6c5d2-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c5d2-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="6c5d2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6c5d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c5d2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c5d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c5d2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c5d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c5d2-107">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="6c5d2-107">Reset passcode action result</span></span>


<span data-ttu-id="6c5d2-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6c5d2-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6c5d2-109">属性</span><span class="sxs-lookup"><span data-stu-id="6c5d2-109">Properties</span></span>
|<span data-ttu-id="6c5d2-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c5d2-110">Property</span></span>|<span data-ttu-id="6c5d2-111">类型</span><span class="sxs-lookup"><span data-stu-id="6c5d2-111">Type</span></span>|<span data-ttu-id="6c5d2-112">说明</span><span class="sxs-lookup"><span data-stu-id="6c5d2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c5d2-113">actionName</span><span class="sxs-lookup"><span data-stu-id="6c5d2-113">actionName</span></span>|<span data-ttu-id="6c5d2-114">String</span><span class="sxs-lookup"><span data-stu-id="6c5d2-114">String</span></span>|<span data-ttu-id="6c5d2-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6c5d2-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6c5d2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6c5d2-116">actionState</span></span>|[<span data-ttu-id="6c5d2-117">actionState</span><span class="sxs-lookup"><span data-stu-id="6c5d2-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6c5d2-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="6c5d2-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6c5d2-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="6c5d2-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6c5d2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6c5d2-120">startDateTime</span></span>|<span data-ttu-id="6c5d2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c5d2-121">DateTimeOffset</span></span>|<span data-ttu-id="6c5d2-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6c5d2-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6c5d2-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c5d2-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="6c5d2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c5d2-124">DateTimeOffset</span></span>|<span data-ttu-id="6c5d2-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6c5d2-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6c5d2-126">密码</span><span class="sxs-lookup"><span data-stu-id="6c5d2-126">passcode</span></span>|<span data-ttu-id="6c5d2-127">String</span><span class="sxs-lookup"><span data-stu-id="6c5d2-127">String</span></span>|<span data-ttu-id="6c5d2-128">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="6c5d2-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c5d2-129">关系</span><span class="sxs-lookup"><span data-stu-id="6c5d2-129">Relationships</span></span>
<span data-ttu-id="6c5d2-130">无</span><span class="sxs-lookup"><span data-stu-id="6c5d2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c5d2-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c5d2-131">JSON Representation</span></span>
<span data-ttu-id="6c5d2-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c5d2-132">Here is a JSON representation of the resource.</span></span>
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




