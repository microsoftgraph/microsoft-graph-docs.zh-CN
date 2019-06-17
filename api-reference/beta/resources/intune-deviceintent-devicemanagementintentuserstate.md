---
title: deviceManagementIntentUserState 资源类型
description: 表示意向的用户状态的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 381be56c44ba46c11d09a483bbace20b8b842e6b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963980"
---
# <a name="devicemanagementintentuserstate-resource-type"></a><span data-ttu-id="10e26-103">deviceManagementIntentUserState 资源类型</span><span class="sxs-lookup"><span data-stu-id="10e26-103">deviceManagementIntentUserState resource type</span></span>

> <span data-ttu-id="10e26-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10e26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10e26-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10e26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10e26-106">表示意向的用户状态的实体</span><span class="sxs-lookup"><span data-stu-id="10e26-106">Entity that represents user state for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="10e26-107">方法</span><span class="sxs-lookup"><span data-stu-id="10e26-107">Methods</span></span>
|<span data-ttu-id="10e26-108">方法</span><span class="sxs-lookup"><span data-stu-id="10e26-108">Method</span></span>|<span data-ttu-id="10e26-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="10e26-109">Return Type</span></span>|<span data-ttu-id="10e26-110">说明</span><span class="sxs-lookup"><span data-stu-id="10e26-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10e26-111">列出 deviceManagementIntentUserStates</span><span class="sxs-lookup"><span data-stu-id="10e26-111">List deviceManagementIntentUserStates</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|<span data-ttu-id="10e26-112">[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="10e26-112">[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) collection</span></span>|<span data-ttu-id="10e26-113">列出[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10e26-113">List properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects.</span></span>|
|[<span data-ttu-id="10e26-114">获取 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="10e26-114">Get deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[<span data-ttu-id="10e26-115">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="10e26-115">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="10e26-116">读取[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10e26-116">Read properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|
|[<span data-ttu-id="10e26-117">创建 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="10e26-117">Create deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[<span data-ttu-id="10e26-118">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="10e26-118">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="10e26-119">创建新的[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10e26-119">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|
|[<span data-ttu-id="10e26-120">删除 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="10e26-120">Delete deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|<span data-ttu-id="10e26-121">无</span><span class="sxs-lookup"><span data-stu-id="10e26-121">None</span></span>|<span data-ttu-id="10e26-122">删除[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="10e26-122">Deletes a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>|
|[<span data-ttu-id="10e26-123">更新 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="10e26-123">Update deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[<span data-ttu-id="10e26-124">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="10e26-124">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="10e26-125">更新[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10e26-125">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10e26-126">属性</span><span class="sxs-lookup"><span data-stu-id="10e26-126">Properties</span></span>
|<span data-ttu-id="10e26-127">属性</span><span class="sxs-lookup"><span data-stu-id="10e26-127">Property</span></span>|<span data-ttu-id="10e26-128">类型</span><span class="sxs-lookup"><span data-stu-id="10e26-128">Type</span></span>|<span data-ttu-id="10e26-129">说明</span><span class="sxs-lookup"><span data-stu-id="10e26-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10e26-130">id</span><span class="sxs-lookup"><span data-stu-id="10e26-130">id</span></span>|<span data-ttu-id="10e26-131">String</span><span class="sxs-lookup"><span data-stu-id="10e26-131">String</span></span>|<span data-ttu-id="10e26-132">ID</span><span class="sxs-lookup"><span data-stu-id="10e26-132">The ID</span></span>|
|<span data-ttu-id="10e26-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10e26-133">userPrincipalName</span></span>|<span data-ttu-id="10e26-134">String</span><span class="sxs-lookup"><span data-stu-id="10e26-134">String</span></span>|<span data-ttu-id="10e26-135">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="10e26-135">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="10e26-136">userName</span><span class="sxs-lookup"><span data-stu-id="10e26-136">userName</span></span>|<span data-ttu-id="10e26-137">String</span><span class="sxs-lookup"><span data-stu-id="10e26-137">String</span></span>|<span data-ttu-id="10e26-138">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="10e26-138">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="10e26-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="10e26-139">deviceCount</span></span>|<span data-ttu-id="10e26-140">Int32</span><span class="sxs-lookup"><span data-stu-id="10e26-140">Int32</span></span>|<span data-ttu-id="10e26-141">属于某个意图的用户的设备计数</span><span class="sxs-lookup"><span data-stu-id="10e26-141">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="10e26-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="10e26-142">lastReportedDateTime</span></span>|<span data-ttu-id="10e26-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e26-143">DateTimeOffset</span></span>|<span data-ttu-id="10e26-144">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="10e26-144">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="10e26-145">state</span><span class="sxs-lookup"><span data-stu-id="10e26-145">state</span></span>|[<span data-ttu-id="10e26-146">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="10e26-146">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="10e26-147">意图的用户状态。</span><span class="sxs-lookup"><span data-stu-id="10e26-147">User state for an intent.</span></span> <span data-ttu-id="10e26-148">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="10e26-148">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10e26-149">关系</span><span class="sxs-lookup"><span data-stu-id="10e26-149">Relationships</span></span>
<span data-ttu-id="10e26-150">无</span><span class="sxs-lookup"><span data-stu-id="10e26-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10e26-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10e26-151">JSON Representation</span></span>
<span data-ttu-id="10e26-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10e26-152">Here is a JSON representation of the resource.</span></span>
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





