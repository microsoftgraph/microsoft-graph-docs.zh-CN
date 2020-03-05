---
title: resetPasscodeActionResult 资源类型
description: 重置密码操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e7ff89fb85192a873595cb362c3e6031b834a7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524933"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="04886-103">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="04886-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="04886-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="04886-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04886-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04886-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04886-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04886-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04886-107">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="04886-107">Reset passcode action result</span></span>


<span data-ttu-id="04886-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="04886-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04886-109">属性</span><span class="sxs-lookup"><span data-stu-id="04886-109">Properties</span></span>
|<span data-ttu-id="04886-110">属性</span><span class="sxs-lookup"><span data-stu-id="04886-110">Property</span></span>|<span data-ttu-id="04886-111">类型</span><span class="sxs-lookup"><span data-stu-id="04886-111">Type</span></span>|<span data-ttu-id="04886-112">说明</span><span class="sxs-lookup"><span data-stu-id="04886-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04886-113">actionName</span><span class="sxs-lookup"><span data-stu-id="04886-113">actionName</span></span>|<span data-ttu-id="04886-114">String</span><span class="sxs-lookup"><span data-stu-id="04886-114">String</span></span>|<span data-ttu-id="04886-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="04886-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="04886-116">actionState</span><span class="sxs-lookup"><span data-stu-id="04886-116">actionState</span></span>|[<span data-ttu-id="04886-117">actionState</span><span class="sxs-lookup"><span data-stu-id="04886-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="04886-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="04886-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="04886-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="04886-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="04886-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="04886-120">startDateTime</span></span>|<span data-ttu-id="04886-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04886-121">DateTimeOffset</span></span>|<span data-ttu-id="04886-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="04886-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="04886-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="04886-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="04886-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04886-124">DateTimeOffset</span></span>|<span data-ttu-id="04886-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="04886-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="04886-126">密码</span><span class="sxs-lookup"><span data-stu-id="04886-126">passcode</span></span>|<span data-ttu-id="04886-127">String</span><span class="sxs-lookup"><span data-stu-id="04886-127">String</span></span>|<span data-ttu-id="04886-128">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="04886-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="04886-129">关系</span><span class="sxs-lookup"><span data-stu-id="04886-129">Relationships</span></span>
<span data-ttu-id="04886-130">无</span><span class="sxs-lookup"><span data-stu-id="04886-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04886-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04886-131">JSON Representation</span></span>
<span data-ttu-id="04886-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04886-132">Here is a JSON representation of the resource.</span></span>
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



