---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e526370ca86792ed30a5f5e24a4be244d73441b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920840"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="5357f-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="5357f-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="5357f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5357f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5357f-105">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="5357f-105">Reset passcode action result</span></span>

<span data-ttu-id="5357f-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5357f-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5357f-107">属性</span><span class="sxs-lookup"><span data-stu-id="5357f-107">Properties</span></span>
|<span data-ttu-id="5357f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5357f-108">Property</span></span>|<span data-ttu-id="5357f-109">类型</span><span class="sxs-lookup"><span data-stu-id="5357f-109">Type</span></span>|<span data-ttu-id="5357f-110">说明</span><span class="sxs-lookup"><span data-stu-id="5357f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5357f-111">actionName</span><span class="sxs-lookup"><span data-stu-id="5357f-111">actionName</span></span>|<span data-ttu-id="5357f-112">String</span><span class="sxs-lookup"><span data-stu-id="5357f-112">String</span></span>|<span data-ttu-id="5357f-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5357f-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5357f-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5357f-114">actionState</span></span>|[<span data-ttu-id="5357f-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5357f-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="5357f-116">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="5357f-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="5357f-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="5357f-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5357f-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5357f-118">startDateTime</span></span>|<span data-ttu-id="5357f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5357f-119">DateTimeOffset</span></span>|<span data-ttu-id="5357f-120">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5357f-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5357f-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5357f-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="5357f-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5357f-122">DateTimeOffset</span></span>|<span data-ttu-id="5357f-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5357f-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5357f-124">密码</span><span class="sxs-lookup"><span data-stu-id="5357f-124">passcode</span></span>|<span data-ttu-id="5357f-125">String</span><span class="sxs-lookup"><span data-stu-id="5357f-125">String</span></span>|<span data-ttu-id="5357f-126">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="5357f-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="5357f-127">关系</span><span class="sxs-lookup"><span data-stu-id="5357f-127">Relationships</span></span>
<span data-ttu-id="5357f-128">无</span><span class="sxs-lookup"><span data-stu-id="5357f-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5357f-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5357f-129">JSON Representation</span></span>
<span data-ttu-id="5357f-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5357f-130">Here is a JSON representation of the resource.</span></span>
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



