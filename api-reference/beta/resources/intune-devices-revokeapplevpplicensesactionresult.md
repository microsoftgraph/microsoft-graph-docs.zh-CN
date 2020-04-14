---
title: revokeAppleVppLicensesActionResult 资源类型
description: 撤销 Apple Vpp 许可证操作结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68a01df03814ea2fd0b52ecfc681490777b46d54
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383149"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="fd74c-103">revokeAppleVppLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd74c-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="fd74c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd74c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd74c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd74c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd74c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd74c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd74c-107">撤销 Apple Vpp 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="fd74c-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="fd74c-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fd74c-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd74c-109">属性</span><span class="sxs-lookup"><span data-stu-id="fd74c-109">Properties</span></span>
|<span data-ttu-id="fd74c-110">属性</span><span class="sxs-lookup"><span data-stu-id="fd74c-110">Property</span></span>|<span data-ttu-id="fd74c-111">类型</span><span class="sxs-lookup"><span data-stu-id="fd74c-111">Type</span></span>|<span data-ttu-id="fd74c-112">说明</span><span class="sxs-lookup"><span data-stu-id="fd74c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd74c-113">actionName</span><span class="sxs-lookup"><span data-stu-id="fd74c-113">actionName</span></span>|<span data-ttu-id="fd74c-114">String</span><span class="sxs-lookup"><span data-stu-id="fd74c-114">String</span></span>|<span data-ttu-id="fd74c-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fd74c-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fd74c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="fd74c-116">actionState</span></span>|[<span data-ttu-id="fd74c-117">actionState</span><span class="sxs-lookup"><span data-stu-id="fd74c-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fd74c-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="fd74c-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="fd74c-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="fd74c-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fd74c-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fd74c-120">startDateTime</span></span>|<span data-ttu-id="fd74c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd74c-121">DateTimeOffset</span></span>|<span data-ttu-id="fd74c-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fd74c-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fd74c-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd74c-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="fd74c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd74c-124">DateTimeOffset</span></span>|<span data-ttu-id="fd74c-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fd74c-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fd74c-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="fd74c-126">totalLicensesCount</span></span>|<span data-ttu-id="fd74c-127">Int32</span><span class="sxs-lookup"><span data-stu-id="fd74c-127">Int32</span></span>|<span data-ttu-id="fd74c-128">关联的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="fd74c-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="fd74c-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="fd74c-129">failedLicensesCount</span></span>|<span data-ttu-id="fd74c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="fd74c-130">Int32</span></span>|<span data-ttu-id="fd74c-131">无法吊销的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="fd74c-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd74c-132">关系</span><span class="sxs-lookup"><span data-stu-id="fd74c-132">Relationships</span></span>
<span data-ttu-id="fd74c-133">无</span><span class="sxs-lookup"><span data-stu-id="fd74c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd74c-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd74c-134">JSON Representation</span></span>
<span data-ttu-id="fd74c-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd74c-135">Here is a JSON representation of the resource.</span></span>
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



