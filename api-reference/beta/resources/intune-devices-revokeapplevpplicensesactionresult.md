---
title: revokeAppleVppLicensesActionResult 资源类型
description: 撤销 Apple Vpp 许可证操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 696901900f3bad4829bd4b51018992d25e99aefc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524926"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="6619b-103">revokeAppleVppLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="6619b-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="6619b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6619b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6619b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6619b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6619b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6619b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6619b-107">撤销 Apple Vpp 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="6619b-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="6619b-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6619b-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6619b-109">属性</span><span class="sxs-lookup"><span data-stu-id="6619b-109">Properties</span></span>
|<span data-ttu-id="6619b-110">属性</span><span class="sxs-lookup"><span data-stu-id="6619b-110">Property</span></span>|<span data-ttu-id="6619b-111">类型</span><span class="sxs-lookup"><span data-stu-id="6619b-111">Type</span></span>|<span data-ttu-id="6619b-112">说明</span><span class="sxs-lookup"><span data-stu-id="6619b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6619b-113">actionName</span><span class="sxs-lookup"><span data-stu-id="6619b-113">actionName</span></span>|<span data-ttu-id="6619b-114">String</span><span class="sxs-lookup"><span data-stu-id="6619b-114">String</span></span>|<span data-ttu-id="6619b-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6619b-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6619b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6619b-116">actionState</span></span>|[<span data-ttu-id="6619b-117">actionState</span><span class="sxs-lookup"><span data-stu-id="6619b-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6619b-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="6619b-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6619b-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="6619b-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6619b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6619b-120">startDateTime</span></span>|<span data-ttu-id="6619b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6619b-121">DateTimeOffset</span></span>|<span data-ttu-id="6619b-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6619b-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6619b-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6619b-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="6619b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6619b-124">DateTimeOffset</span></span>|<span data-ttu-id="6619b-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6619b-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6619b-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6619b-126">totalLicensesCount</span></span>|<span data-ttu-id="6619b-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6619b-127">Int32</span></span>|<span data-ttu-id="6619b-128">关联的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="6619b-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="6619b-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6619b-129">failedLicensesCount</span></span>|<span data-ttu-id="6619b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6619b-130">Int32</span></span>|<span data-ttu-id="6619b-131">无法吊销的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="6619b-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="6619b-132">关系</span><span class="sxs-lookup"><span data-stu-id="6619b-132">Relationships</span></span>
<span data-ttu-id="6619b-133">无</span><span class="sxs-lookup"><span data-stu-id="6619b-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6619b-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6619b-134">JSON Representation</span></span>
<span data-ttu-id="6619b-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6619b-135">Here is a JSON representation of the resource.</span></span>
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



