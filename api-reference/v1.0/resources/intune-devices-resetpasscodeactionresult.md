---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 81a30b36ac418d5553c7387fea22a172926a73ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824855"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="da457-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="da457-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="da457-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="da457-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da457-105">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="da457-105">Reset passcode action result</span></span>

<span data-ttu-id="da457-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="da457-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="da457-107">属性</span><span class="sxs-lookup"><span data-stu-id="da457-107">Properties</span></span>
|<span data-ttu-id="da457-108">属性</span><span class="sxs-lookup"><span data-stu-id="da457-108">Property</span></span>|<span data-ttu-id="da457-109">类型</span><span class="sxs-lookup"><span data-stu-id="da457-109">Type</span></span>|<span data-ttu-id="da457-110">说明</span><span class="sxs-lookup"><span data-stu-id="da457-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da457-111">actionName</span><span class="sxs-lookup"><span data-stu-id="da457-111">actionName</span></span>|<span data-ttu-id="da457-112">String</span><span class="sxs-lookup"><span data-stu-id="da457-112">String</span></span>|<span data-ttu-id="da457-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="da457-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="da457-114">actionState</span><span class="sxs-lookup"><span data-stu-id="da457-114">actionState</span></span>|[<span data-ttu-id="da457-115">actionState</span><span class="sxs-lookup"><span data-stu-id="da457-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="da457-116">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="da457-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="da457-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="da457-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="da457-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da457-118">startDateTime</span></span>|<span data-ttu-id="da457-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da457-119">DateTimeOffset</span></span>|<span data-ttu-id="da457-120">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="da457-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="da457-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="da457-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="da457-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da457-122">DateTimeOffset</span></span>|<span data-ttu-id="da457-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="da457-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="da457-124">密码</span><span class="sxs-lookup"><span data-stu-id="da457-124">passcode</span></span>|<span data-ttu-id="da457-125">String</span><span class="sxs-lookup"><span data-stu-id="da457-125">String</span></span>|<span data-ttu-id="da457-126">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="da457-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="da457-127">关系</span><span class="sxs-lookup"><span data-stu-id="da457-127">Relationships</span></span>
<span data-ttu-id="da457-128">无</span><span class="sxs-lookup"><span data-stu-id="da457-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="da457-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da457-129">JSON Representation</span></span>
<span data-ttu-id="da457-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da457-130">Here is a JSON representation of the resource.</span></span>
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



