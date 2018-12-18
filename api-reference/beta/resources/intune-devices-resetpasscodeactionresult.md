---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: tfitzmac
ms.openlocfilehash: 24d7a6f259f456c742c4317763dd9cefe8d185a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301108"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="15fbc-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="15fbc-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="15fbc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="15fbc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15fbc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="15fbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15fbc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="15fbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15fbc-107">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="15fbc-107">Reset passcode action result</span></span>

<span data-ttu-id="15fbc-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="15fbc-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15fbc-109">属性</span><span class="sxs-lookup"><span data-stu-id="15fbc-109">Properties</span></span>
|<span data-ttu-id="15fbc-110">属性</span><span class="sxs-lookup"><span data-stu-id="15fbc-110">Property</span></span>|<span data-ttu-id="15fbc-111">类型</span><span class="sxs-lookup"><span data-stu-id="15fbc-111">Type</span></span>|<span data-ttu-id="15fbc-112">说明</span><span class="sxs-lookup"><span data-stu-id="15fbc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15fbc-113">actionName</span><span class="sxs-lookup"><span data-stu-id="15fbc-113">actionName</span></span>|<span data-ttu-id="15fbc-114">String</span><span class="sxs-lookup"><span data-stu-id="15fbc-114">String</span></span>|<span data-ttu-id="15fbc-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="15fbc-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="15fbc-116">actionState</span><span class="sxs-lookup"><span data-stu-id="15fbc-116">actionState</span></span>|[<span data-ttu-id="15fbc-117">actionState</span><span class="sxs-lookup"><span data-stu-id="15fbc-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="15fbc-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="15fbc-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="15fbc-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="15fbc-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="15fbc-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="15fbc-120">startDateTime</span></span>|<span data-ttu-id="15fbc-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15fbc-121">DateTimeOffset</span></span>|<span data-ttu-id="15fbc-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="15fbc-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="15fbc-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="15fbc-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="15fbc-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15fbc-124">DateTimeOffset</span></span>|<span data-ttu-id="15fbc-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="15fbc-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="15fbc-126">密码</span><span class="sxs-lookup"><span data-stu-id="15fbc-126">passcode</span></span>|<span data-ttu-id="15fbc-127">String</span><span class="sxs-lookup"><span data-stu-id="15fbc-127">String</span></span>|<span data-ttu-id="15fbc-128">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="15fbc-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="15fbc-129">关系</span><span class="sxs-lookup"><span data-stu-id="15fbc-129">Relationships</span></span>
<span data-ttu-id="15fbc-130">无</span><span class="sxs-lookup"><span data-stu-id="15fbc-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15fbc-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15fbc-131">JSON Representation</span></span>
<span data-ttu-id="15fbc-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15fbc-132">Here is a JSON representation of the resource.</span></span>
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





