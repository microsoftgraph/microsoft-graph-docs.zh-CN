---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3da6540d616d088037285ba1a2c29b6cc0d07faa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027389"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="696b7-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="696b7-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="696b7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="696b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="696b7-105">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="696b7-105">Reset passcode action result</span></span>


<span data-ttu-id="696b7-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="696b7-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="696b7-107">属性</span><span class="sxs-lookup"><span data-stu-id="696b7-107">Properties</span></span>
|<span data-ttu-id="696b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="696b7-108">Property</span></span>|<span data-ttu-id="696b7-109">类型</span><span class="sxs-lookup"><span data-stu-id="696b7-109">Type</span></span>|<span data-ttu-id="696b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="696b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="696b7-111">actionName</span><span class="sxs-lookup"><span data-stu-id="696b7-111">actionName</span></span>|<span data-ttu-id="696b7-112">String</span><span class="sxs-lookup"><span data-stu-id="696b7-112">String</span></span>|<span data-ttu-id="696b7-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="696b7-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="696b7-114">actionState</span><span class="sxs-lookup"><span data-stu-id="696b7-114">actionState</span></span>|[<span data-ttu-id="696b7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="696b7-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="696b7-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="696b7-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="696b7-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="696b7-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="696b7-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="696b7-118">startDateTime</span></span>|<span data-ttu-id="696b7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696b7-119">DateTimeOffset</span></span>|<span data-ttu-id="696b7-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="696b7-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="696b7-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="696b7-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="696b7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696b7-122">DateTimeOffset</span></span>|<span data-ttu-id="696b7-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="696b7-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="696b7-124">密码</span><span class="sxs-lookup"><span data-stu-id="696b7-124">passcode</span></span>|<span data-ttu-id="696b7-125">String</span><span class="sxs-lookup"><span data-stu-id="696b7-125">String</span></span>|<span data-ttu-id="696b7-126">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="696b7-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="696b7-127">关系</span><span class="sxs-lookup"><span data-stu-id="696b7-127">Relationships</span></span>
<span data-ttu-id="696b7-128">无</span><span class="sxs-lookup"><span data-stu-id="696b7-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="696b7-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="696b7-129">JSON Representation</span></span>
<span data-ttu-id="696b7-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="696b7-130">Here is a JSON representation of the resource.</span></span>
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



