---
title: revokeAppleVppLicensesActionResult 资源类型
description: 撤销 Apple Vpp 许可证操作结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc3c289a01578e1d707d0a1780fa76c9a675ac33
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783877"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="9cf89-103">revokeAppleVppLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="9cf89-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="9cf89-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9cf89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf89-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9cf89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf89-106">撤销 Apple Vpp 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="9cf89-106">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="9cf89-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9cf89-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9cf89-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cf89-108">Properties</span></span>
|<span data-ttu-id="9cf89-109">属性</span><span class="sxs-lookup"><span data-stu-id="9cf89-109">Property</span></span>|<span data-ttu-id="9cf89-110">类型</span><span class="sxs-lookup"><span data-stu-id="9cf89-110">Type</span></span>|<span data-ttu-id="9cf89-111">说明</span><span class="sxs-lookup"><span data-stu-id="9cf89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf89-112">actionName</span><span class="sxs-lookup"><span data-stu-id="9cf89-112">actionName</span></span>|<span data-ttu-id="9cf89-113">String</span><span class="sxs-lookup"><span data-stu-id="9cf89-113">String</span></span>|<span data-ttu-id="9cf89-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9cf89-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9cf89-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9cf89-115">actionState</span></span>|[<span data-ttu-id="9cf89-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9cf89-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9cf89-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9cf89-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9cf89-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="9cf89-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9cf89-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9cf89-119">startDateTime</span></span>|<span data-ttu-id="9cf89-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cf89-120">DateTimeOffset</span></span>|<span data-ttu-id="9cf89-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9cf89-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9cf89-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cf89-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="9cf89-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cf89-123">DateTimeOffset</span></span>|<span data-ttu-id="9cf89-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9cf89-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9cf89-125">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="9cf89-125">totalLicensesCount</span></span>|<span data-ttu-id="9cf89-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf89-126">Int32</span></span>|<span data-ttu-id="9cf89-127">关联的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="9cf89-127">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="9cf89-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="9cf89-128">failedLicensesCount</span></span>|<span data-ttu-id="9cf89-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf89-129">Int32</span></span>|<span data-ttu-id="9cf89-130">无法吊销的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="9cf89-130">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cf89-131">关系</span><span class="sxs-lookup"><span data-stu-id="9cf89-131">Relationships</span></span>
<span data-ttu-id="9cf89-132">无</span><span class="sxs-lookup"><span data-stu-id="9cf89-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cf89-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cf89-133">JSON Representation</span></span>
<span data-ttu-id="9cf89-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cf89-134">Here is a JSON representation of the resource.</span></span>
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



