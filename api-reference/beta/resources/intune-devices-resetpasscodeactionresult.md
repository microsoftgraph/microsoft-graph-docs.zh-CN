---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f7d6c3c8f2d339fa499fe09b5b1981833b2f020
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578776"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="c5ab6-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5ab6-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="c5ab6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5ab6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5ab6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5ab6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5ab6-106">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="c5ab6-106">Reset passcode action result</span></span>


<span data-ttu-id="c5ab6-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c5ab6-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5ab6-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5ab6-108">Properties</span></span>
|<span data-ttu-id="c5ab6-109">属性</span><span class="sxs-lookup"><span data-stu-id="c5ab6-109">Property</span></span>|<span data-ttu-id="c5ab6-110">类型</span><span class="sxs-lookup"><span data-stu-id="c5ab6-110">Type</span></span>|<span data-ttu-id="c5ab6-111">说明</span><span class="sxs-lookup"><span data-stu-id="c5ab6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5ab6-112">actionName</span><span class="sxs-lookup"><span data-stu-id="c5ab6-112">actionName</span></span>|<span data-ttu-id="c5ab6-113">String</span><span class="sxs-lookup"><span data-stu-id="c5ab6-113">String</span></span>|<span data-ttu-id="c5ab6-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c5ab6-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c5ab6-115">actionState</span><span class="sxs-lookup"><span data-stu-id="c5ab6-115">actionState</span></span>|[<span data-ttu-id="c5ab6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c5ab6-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c5ab6-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="c5ab6-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c5ab6-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="c5ab6-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c5ab6-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ab6-119">startDateTime</span></span>|<span data-ttu-id="c5ab6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ab6-120">DateTimeOffset</span></span>|<span data-ttu-id="c5ab6-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c5ab6-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c5ab6-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ab6-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="c5ab6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ab6-123">DateTimeOffset</span></span>|<span data-ttu-id="c5ab6-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c5ab6-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c5ab6-125">密码</span><span class="sxs-lookup"><span data-stu-id="c5ab6-125">passcode</span></span>|<span data-ttu-id="c5ab6-126">String</span><span class="sxs-lookup"><span data-stu-id="c5ab6-126">String</span></span>|<span data-ttu-id="c5ab6-127">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="c5ab6-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="c5ab6-128">关系</span><span class="sxs-lookup"><span data-stu-id="c5ab6-128">Relationships</span></span>
<span data-ttu-id="c5ab6-129">无</span><span class="sxs-lookup"><span data-stu-id="c5ab6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5ab6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5ab6-130">JSON Representation</span></span>
<span data-ttu-id="c5ab6-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5ab6-131">Here is a JSON representation of the resource.</span></span>
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





