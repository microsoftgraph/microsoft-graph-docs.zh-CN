---
title: revokeAppleVppLicensesActionResult 资源类型
description: 取消 Apple Vpp 许可证操作结果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cd77bee330e919ab51927af0773d913099cea6e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419224"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="cb2a7-103">revokeAppleVppLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb2a7-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="cb2a7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cb2a7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb2a7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cb2a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb2a7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb2a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb2a7-107">取消 Apple Vpp 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="cb2a7-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="cb2a7-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb2a7-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb2a7-109">属性</span><span class="sxs-lookup"><span data-stu-id="cb2a7-109">Properties</span></span>
|<span data-ttu-id="cb2a7-110">属性</span><span class="sxs-lookup"><span data-stu-id="cb2a7-110">Property</span></span>|<span data-ttu-id="cb2a7-111">类型</span><span class="sxs-lookup"><span data-stu-id="cb2a7-111">Type</span></span>|<span data-ttu-id="cb2a7-112">说明</span><span class="sxs-lookup"><span data-stu-id="cb2a7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb2a7-113">actionName</span><span class="sxs-lookup"><span data-stu-id="cb2a7-113">actionName</span></span>|<span data-ttu-id="cb2a7-114">String</span><span class="sxs-lookup"><span data-stu-id="cb2a7-114">String</span></span>|<span data-ttu-id="cb2a7-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb2a7-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cb2a7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cb2a7-116">actionState</span></span>|[<span data-ttu-id="cb2a7-117">actionState</span><span class="sxs-lookup"><span data-stu-id="cb2a7-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cb2a7-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="cb2a7-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="cb2a7-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="cb2a7-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cb2a7-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cb2a7-120">startDateTime</span></span>|<span data-ttu-id="cb2a7-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb2a7-121">DateTimeOffset</span></span>|<span data-ttu-id="cb2a7-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb2a7-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cb2a7-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb2a7-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="cb2a7-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb2a7-124">DateTimeOffset</span></span>|<span data-ttu-id="cb2a7-125">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb2a7-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cb2a7-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="cb2a7-126">totalLicensesCount</span></span>|<span data-ttu-id="cb2a7-127">Int32</span><span class="sxs-lookup"><span data-stu-id="cb2a7-127">Int32</span></span>|<span data-ttu-id="cb2a7-128">Apple Vpp 许可证关联总数</span><span class="sxs-lookup"><span data-stu-id="cb2a7-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="cb2a7-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="cb2a7-129">failedLicensesCount</span></span>|<span data-ttu-id="cb2a7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="cb2a7-130">Int32</span></span>|<span data-ttu-id="cb2a7-131">无法撤消的 Apple Vpp 许可证的总数</span><span class="sxs-lookup"><span data-stu-id="cb2a7-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb2a7-132">关系</span><span class="sxs-lookup"><span data-stu-id="cb2a7-132">Relationships</span></span>
<span data-ttu-id="cb2a7-133">无</span><span class="sxs-lookup"><span data-stu-id="cb2a7-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb2a7-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb2a7-134">JSON Representation</span></span>
<span data-ttu-id="cb2a7-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb2a7-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```




