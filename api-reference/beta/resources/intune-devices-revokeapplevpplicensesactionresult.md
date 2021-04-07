---
title: revokeAppleVppLicensesActionResult 资源类型
description: 撤销 Apple Vpp 许可证操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56fce51fb5de4066136199a99670c4767b6ad724
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611858"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="54a07-103">revokeAppleVppLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="54a07-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="54a07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54a07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54a07-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54a07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54a07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54a07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54a07-107">撤销 Apple Vpp 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="54a07-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="54a07-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54a07-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54a07-109">属性</span><span class="sxs-lookup"><span data-stu-id="54a07-109">Properties</span></span>
|<span data-ttu-id="54a07-110">属性</span><span class="sxs-lookup"><span data-stu-id="54a07-110">Property</span></span>|<span data-ttu-id="54a07-111">类型</span><span class="sxs-lookup"><span data-stu-id="54a07-111">Type</span></span>|<span data-ttu-id="54a07-112">Description</span><span class="sxs-lookup"><span data-stu-id="54a07-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54a07-113">actionName</span><span class="sxs-lookup"><span data-stu-id="54a07-113">actionName</span></span>|<span data-ttu-id="54a07-114">String</span><span class="sxs-lookup"><span data-stu-id="54a07-114">String</span></span>|<span data-ttu-id="54a07-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54a07-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="54a07-116">actionState</span><span class="sxs-lookup"><span data-stu-id="54a07-116">actionState</span></span>|[<span data-ttu-id="54a07-117">actionState</span><span class="sxs-lookup"><span data-stu-id="54a07-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="54a07-118">操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。</span><span class="sxs-lookup"><span data-stu-id="54a07-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="54a07-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="54a07-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="54a07-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="54a07-120">startDateTime</span></span>|<span data-ttu-id="54a07-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54a07-121">DateTimeOffset</span></span>|<span data-ttu-id="54a07-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54a07-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="54a07-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="54a07-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="54a07-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54a07-124">DateTimeOffset</span></span>|<span data-ttu-id="54a07-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="54a07-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="54a07-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="54a07-126">totalLicensesCount</span></span>|<span data-ttu-id="54a07-127">Int32</span><span class="sxs-lookup"><span data-stu-id="54a07-127">Int32</span></span>|<span data-ttu-id="54a07-128">关联的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="54a07-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="54a07-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="54a07-129">failedLicensesCount</span></span>|<span data-ttu-id="54a07-130">Int32</span><span class="sxs-lookup"><span data-stu-id="54a07-130">Int32</span></span>|<span data-ttu-id="54a07-131">未能撤销的 Apple Vpp 许可证总数</span><span class="sxs-lookup"><span data-stu-id="54a07-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="54a07-132">关系</span><span class="sxs-lookup"><span data-stu-id="54a07-132">Relationships</span></span>
<span data-ttu-id="54a07-133">无</span><span class="sxs-lookup"><span data-stu-id="54a07-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54a07-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54a07-134">JSON Representation</span></span>
<span data-ttu-id="54a07-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54a07-135">Here is a JSON representation of the resource.</span></span>
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




