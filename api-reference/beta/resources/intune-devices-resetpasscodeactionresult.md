---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ead49e3c73dc65ebbc139fc7d1fd37743fe98be3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844707"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="d9fa8-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9fa8-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="d9fa8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9fa8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9fa8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9fa8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9fa8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9fa8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9fa8-107">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="d9fa8-107">Reset passcode action result</span></span>

<span data-ttu-id="d9fa8-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9fa8-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9fa8-109">属性</span><span class="sxs-lookup"><span data-stu-id="d9fa8-109">Properties</span></span>
|<span data-ttu-id="d9fa8-110">属性</span><span class="sxs-lookup"><span data-stu-id="d9fa8-110">Property</span></span>|<span data-ttu-id="d9fa8-111">类型</span><span class="sxs-lookup"><span data-stu-id="d9fa8-111">Type</span></span>|<span data-ttu-id="d9fa8-112">说明</span><span class="sxs-lookup"><span data-stu-id="d9fa8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9fa8-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d9fa8-113">actionName</span></span>|<span data-ttu-id="d9fa8-114">String</span><span class="sxs-lookup"><span data-stu-id="d9fa8-114">String</span></span>|<span data-ttu-id="d9fa8-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9fa8-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d9fa8-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d9fa8-116">actionState</span></span>|[<span data-ttu-id="d9fa8-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d9fa8-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d9fa8-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d9fa8-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d9fa8-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d9fa8-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d9fa8-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d9fa8-120">startDateTime</span></span>|<span data-ttu-id="d9fa8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9fa8-121">DateTimeOffset</span></span>|<span data-ttu-id="d9fa8-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9fa8-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d9fa8-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9fa8-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d9fa8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9fa8-124">DateTimeOffset</span></span>|<span data-ttu-id="d9fa8-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9fa8-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d9fa8-126">密码</span><span class="sxs-lookup"><span data-stu-id="d9fa8-126">passcode</span></span>|<span data-ttu-id="d9fa8-127">String</span><span class="sxs-lookup"><span data-stu-id="d9fa8-127">String</span></span>|<span data-ttu-id="d9fa8-128">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="d9fa8-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="d9fa8-129">关系</span><span class="sxs-lookup"><span data-stu-id="d9fa8-129">Relationships</span></span>
<span data-ttu-id="d9fa8-130">无</span><span class="sxs-lookup"><span data-stu-id="d9fa8-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9fa8-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9fa8-131">JSON Representation</span></span>
<span data-ttu-id="d9fa8-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9fa8-132">Here is a JSON representation of the resource.</span></span>
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





