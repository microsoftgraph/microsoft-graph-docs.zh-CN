---
title: deviceManagementIntentUserState 资源类型
description: 表示意向的用户状态的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fef4bd7995cf822af39743fe6f61028813b4a389
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943261"
---
# <a name="devicemanagementintentuserstate-resource-type"></a><span data-ttu-id="00697-103">deviceManagementIntentUserState 资源类型</span><span class="sxs-lookup"><span data-stu-id="00697-103">deviceManagementIntentUserState resource type</span></span>

> <span data-ttu-id="00697-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00697-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00697-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00697-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00697-106">表示意向的用户状态的实体</span><span class="sxs-lookup"><span data-stu-id="00697-106">Entity that represents user state for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="00697-107">方法</span><span class="sxs-lookup"><span data-stu-id="00697-107">Methods</span></span>
|<span data-ttu-id="00697-108">方法</span><span class="sxs-lookup"><span data-stu-id="00697-108">Method</span></span>|<span data-ttu-id="00697-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="00697-109">Return Type</span></span>|<span data-ttu-id="00697-110">说明</span><span class="sxs-lookup"><span data-stu-id="00697-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00697-111">列出 deviceManagementIntentUserStates</span><span class="sxs-lookup"><span data-stu-id="00697-111">List deviceManagementIntentUserStates</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|<span data-ttu-id="00697-112">[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="00697-112">[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) collection</span></span>|<span data-ttu-id="00697-113">列出[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00697-113">List properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects.</span></span>|
|[<span data-ttu-id="00697-114">获取 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="00697-114">Get deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[<span data-ttu-id="00697-115">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="00697-115">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="00697-116">读取[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00697-116">Read properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|
|[<span data-ttu-id="00697-117">创建 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="00697-117">Create deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[<span data-ttu-id="00697-118">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="00697-118">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="00697-119">创建新的[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00697-119">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|
|[<span data-ttu-id="00697-120">删除 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="00697-120">Delete deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|<span data-ttu-id="00697-121">无</span><span class="sxs-lookup"><span data-stu-id="00697-121">None</span></span>|<span data-ttu-id="00697-122">删除[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="00697-122">Deletes a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>|
|[<span data-ttu-id="00697-123">更新 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="00697-123">Update deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[<span data-ttu-id="00697-124">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="00697-124">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="00697-125">更新[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00697-125">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00697-126">属性</span><span class="sxs-lookup"><span data-stu-id="00697-126">Properties</span></span>
|<span data-ttu-id="00697-127">属性</span><span class="sxs-lookup"><span data-stu-id="00697-127">Property</span></span>|<span data-ttu-id="00697-128">类型</span><span class="sxs-lookup"><span data-stu-id="00697-128">Type</span></span>|<span data-ttu-id="00697-129">说明</span><span class="sxs-lookup"><span data-stu-id="00697-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00697-130">id</span><span class="sxs-lookup"><span data-stu-id="00697-130">id</span></span>|<span data-ttu-id="00697-131">String</span><span class="sxs-lookup"><span data-stu-id="00697-131">String</span></span>|<span data-ttu-id="00697-132">ID</span><span class="sxs-lookup"><span data-stu-id="00697-132">The ID</span></span>|
|<span data-ttu-id="00697-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00697-133">userPrincipalName</span></span>|<span data-ttu-id="00697-134">String</span><span class="sxs-lookup"><span data-stu-id="00697-134">String</span></span>|<span data-ttu-id="00697-135">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="00697-135">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="00697-136">userName</span><span class="sxs-lookup"><span data-stu-id="00697-136">userName</span></span>|<span data-ttu-id="00697-137">String</span><span class="sxs-lookup"><span data-stu-id="00697-137">String</span></span>|<span data-ttu-id="00697-138">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="00697-138">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="00697-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="00697-139">deviceCount</span></span>|<span data-ttu-id="00697-140">Int32</span><span class="sxs-lookup"><span data-stu-id="00697-140">Int32</span></span>|<span data-ttu-id="00697-141">属于某个意图的用户的设备计数</span><span class="sxs-lookup"><span data-stu-id="00697-141">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="00697-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="00697-142">lastReportedDateTime</span></span>|<span data-ttu-id="00697-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00697-143">DateTimeOffset</span></span>|<span data-ttu-id="00697-144">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="00697-144">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="00697-145">state</span><span class="sxs-lookup"><span data-stu-id="00697-145">state</span></span>|[<span data-ttu-id="00697-146">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="00697-146">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="00697-147">意图的用户状态。</span><span class="sxs-lookup"><span data-stu-id="00697-147">User state for an intent.</span></span> <span data-ttu-id="00697-148">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="00697-148">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00697-149">关系</span><span class="sxs-lookup"><span data-stu-id="00697-149">Relationships</span></span>
<span data-ttu-id="00697-150">无</span><span class="sxs-lookup"><span data-stu-id="00697-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00697-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00697-151">JSON Representation</span></span>
<span data-ttu-id="00697-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00697-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```




