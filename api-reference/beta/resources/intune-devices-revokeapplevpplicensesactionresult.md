---
title: revokeAppleVppLicensesActionResult 资源类型
description: 撤销 Apple Vpp 许可证操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10b26592c859ba58ad4759492c34ca3626be32dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999631"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="2f4b0-103">revokeAppleVppLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f4b0-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="2f4b0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f4b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f4b0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f4b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f4b0-106">撤销 Apple Vpp 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="2f4b0-106">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="2f4b0-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f4b0-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2f4b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f4b0-108">Properties</span></span>
|<span data-ttu-id="2f4b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f4b0-109">Property</span></span>|<span data-ttu-id="2f4b0-110">类型</span><span class="sxs-lookup"><span data-stu-id="2f4b0-110">Type</span></span>|<span data-ttu-id="2f4b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f4b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f4b0-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2f4b0-112">actionName</span></span>|<span data-ttu-id="2f4b0-113">String</span><span class="sxs-lookup"><span data-stu-id="2f4b0-113">String</span></span>|<span data-ttu-id="2f4b0-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f4b0-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f4b0-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2f4b0-115">actionState</span></span>|[<span data-ttu-id="2f4b0-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2f4b0-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2f4b0-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2f4b0-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2f4b0-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="2f4b0-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2f4b0-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2f4b0-119">startDateTime</span></span>|<span data-ttu-id="2f4b0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f4b0-120">DateTimeOffset</span></span>|<span data-ttu-id="2f4b0-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f4b0-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f4b0-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f4b0-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2f4b0-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f4b0-123">DateTimeOffset</span></span>|<span data-ttu-id="2f4b0-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f4b0-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f4b0-125">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="2f4b0-125">totalLicensesCount</span></span>|<span data-ttu-id="2f4b0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="2f4b0-126">Int32</span></span>|<span data-ttu-id="2f4b0-127">关联的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="2f4b0-127">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="2f4b0-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="2f4b0-128">failedLicensesCount</span></span>|<span data-ttu-id="2f4b0-129">Int32</span><span class="sxs-lookup"><span data-stu-id="2f4b0-129">Int32</span></span>|<span data-ttu-id="2f4b0-130">无法吊销的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="2f4b0-130">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f4b0-131">关系</span><span class="sxs-lookup"><span data-stu-id="2f4b0-131">Relationships</span></span>
<span data-ttu-id="2f4b0-132">无</span><span class="sxs-lookup"><span data-stu-id="2f4b0-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f4b0-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f4b0-133">JSON Representation</span></span>
<span data-ttu-id="2f4b0-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f4b0-134">Here is a JSON representation of the resource.</span></span>
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





