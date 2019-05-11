---
title: deviceManagementPartner 资源类型
description: 表示与设备管理合作伙伴的连接的实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd6b51584945ee1c6cb44584324c4b84ed0acc00
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940265"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="39c08-103">deviceManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="39c08-103">deviceManagementPartner resource type</span></span>

> <span data-ttu-id="39c08-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="39c08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39c08-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39c08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39c08-106">表示与设备管理合作伙伴的连接的实体。</span><span class="sxs-lookup"><span data-stu-id="39c08-106">Entity which represents a connection to device management partner.</span></span>

## <a name="methods"></a><span data-ttu-id="39c08-107">方法</span><span class="sxs-lookup"><span data-stu-id="39c08-107">Methods</span></span>
|<span data-ttu-id="39c08-108">方法</span><span class="sxs-lookup"><span data-stu-id="39c08-108">Method</span></span>|<span data-ttu-id="39c08-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="39c08-109">Return Type</span></span>|<span data-ttu-id="39c08-110">说明</span><span class="sxs-lookup"><span data-stu-id="39c08-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39c08-111">列出 deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="39c08-111">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="39c08-112">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39c08-112">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="39c08-113">列出 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39c08-113">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="39c08-114">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39c08-114">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="39c08-115">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39c08-115">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="39c08-116">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39c08-116">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="39c08-117">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39c08-117">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="39c08-118">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39c08-118">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="39c08-119">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39c08-119">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="39c08-120">删除 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39c08-120">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="39c08-121">无</span><span class="sxs-lookup"><span data-stu-id="39c08-121">None</span></span>|<span data-ttu-id="39c08-122">删除 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="39c08-122">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="39c08-123">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39c08-123">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="39c08-124">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39c08-124">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="39c08-125">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="39c08-125">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="39c08-126">属性</span><span class="sxs-lookup"><span data-stu-id="39c08-126">Properties</span></span>
|<span data-ttu-id="39c08-127">属性</span><span class="sxs-lookup"><span data-stu-id="39c08-127">Property</span></span>|<span data-ttu-id="39c08-128">类型</span><span class="sxs-lookup"><span data-stu-id="39c08-128">Type</span></span>|<span data-ttu-id="39c08-129">说明</span><span class="sxs-lookup"><span data-stu-id="39c08-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39c08-130">id</span><span class="sxs-lookup"><span data-stu-id="39c08-130">id</span></span>|<span data-ttu-id="39c08-131">String</span><span class="sxs-lookup"><span data-stu-id="39c08-131">String</span></span>|<span data-ttu-id="39c08-132">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="39c08-132">Id of the entity</span></span>|
|<span data-ttu-id="39c08-133">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="39c08-133">lastHeartbeatDateTime</span></span>|<span data-ttu-id="39c08-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39c08-134">DateTimeOffset</span></span>|<span data-ttu-id="39c08-135">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="39c08-135">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="39c08-136">partnerState</span><span class="sxs-lookup"><span data-stu-id="39c08-136">partnerState</span></span>|[<span data-ttu-id="39c08-137">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="39c08-137">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="39c08-138">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="39c08-138">Partner state of this tenant.</span></span> <span data-ttu-id="39c08-139">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="39c08-139">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="39c08-140">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="39c08-140">partnerAppType</span></span>|[<span data-ttu-id="39c08-141">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="39c08-141">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="39c08-142">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="39c08-142">Partner App type.</span></span> <span data-ttu-id="39c08-143">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="39c08-143">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="39c08-144">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="39c08-144">singleTenantAppId</span></span>|<span data-ttu-id="39c08-145">String</span><span class="sxs-lookup"><span data-stu-id="39c08-145">String</span></span>|<span data-ttu-id="39c08-146">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="39c08-146">Partner Single tenant App id</span></span>|
|<span data-ttu-id="39c08-147">displayName</span><span class="sxs-lookup"><span data-stu-id="39c08-147">displayName</span></span>|<span data-ttu-id="39c08-148">String</span><span class="sxs-lookup"><span data-stu-id="39c08-148">String</span></span>|<span data-ttu-id="39c08-149">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="39c08-149">Partner display name</span></span>|
|<span data-ttu-id="39c08-150">isConfigured</span><span class="sxs-lookup"><span data-stu-id="39c08-150">isConfigured</span></span>|<span data-ttu-id="39c08-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="39c08-151">Boolean</span></span>|<span data-ttu-id="39c08-152">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="39c08-152">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="39c08-153">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="39c08-153">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="39c08-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39c08-154">DateTimeOffset</span></span>|<span data-ttu-id="39c08-155">将删除 PartnerDevices 时, UTC 格式的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="39c08-155">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="39c08-156">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="39c08-156">This will become obselete soon.</span></span>|
|<span data-ttu-id="39c08-157">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="39c08-157">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="39c08-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39c08-158">DateTimeOffset</span></span>|<span data-ttu-id="39c08-159">PartnerDevices 将被标记为不符合时的 UTC 格式的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="39c08-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="39c08-160">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="39c08-160">This will become obselete soon.</span></span>|
|<span data-ttu-id="39c08-161">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="39c08-161">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="39c08-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39c08-162">DateTimeOffset</span></span>|<span data-ttu-id="39c08-163">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="39c08-163">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="39c08-164">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="39c08-164">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="39c08-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39c08-165">DateTimeOffset</span></span>|<span data-ttu-id="39c08-166">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="39c08-166">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|

## <a name="relationships"></a><span data-ttu-id="39c08-167">关系</span><span class="sxs-lookup"><span data-stu-id="39c08-167">Relationships</span></span>
<span data-ttu-id="39c08-168">无</span><span class="sxs-lookup"><span data-stu-id="39c08-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39c08-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39c08-169">JSON Representation</span></span>
<span data-ttu-id="39c08-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39c08-170">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```




