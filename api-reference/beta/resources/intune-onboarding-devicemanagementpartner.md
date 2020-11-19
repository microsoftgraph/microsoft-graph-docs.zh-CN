---
title: deviceManagementPartner 资源类型
description: 表示与设备管理合作伙伴的连接的实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 77559b60882dc160628f2bb7a31a1e0cb8eeec3d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272176"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="6784e-103">deviceManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="6784e-103">deviceManagementPartner resource type</span></span>

<span data-ttu-id="6784e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6784e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6784e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6784e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6784e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6784e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6784e-107">表示与设备管理合作伙伴的连接的实体。</span><span class="sxs-lookup"><span data-stu-id="6784e-107">Entity which represents a connection to device management partner.</span></span>

## <a name="methods"></a><span data-ttu-id="6784e-108">方法</span><span class="sxs-lookup"><span data-stu-id="6784e-108">Methods</span></span>
|<span data-ttu-id="6784e-109">方法</span><span class="sxs-lookup"><span data-stu-id="6784e-109">Method</span></span>|<span data-ttu-id="6784e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6784e-110">Return Type</span></span>|<span data-ttu-id="6784e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6784e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6784e-112">列出 deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="6784e-112">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="6784e-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6784e-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="6784e-114">列出 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6784e-114">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="6784e-115">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6784e-115">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="6784e-116">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6784e-116">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="6784e-117">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6784e-117">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="6784e-118">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6784e-118">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="6784e-119">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6784e-119">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="6784e-120">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6784e-120">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="6784e-121">删除 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6784e-121">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="6784e-122">无</span><span class="sxs-lookup"><span data-stu-id="6784e-122">None</span></span>|<span data-ttu-id="6784e-123">删除 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="6784e-123">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="6784e-124">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6784e-124">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="6784e-125">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6784e-125">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="6784e-126">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6784e-126">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6784e-127">属性</span><span class="sxs-lookup"><span data-stu-id="6784e-127">Properties</span></span>
|<span data-ttu-id="6784e-128">属性</span><span class="sxs-lookup"><span data-stu-id="6784e-128">Property</span></span>|<span data-ttu-id="6784e-129">类型</span><span class="sxs-lookup"><span data-stu-id="6784e-129">Type</span></span>|<span data-ttu-id="6784e-130">说明</span><span class="sxs-lookup"><span data-stu-id="6784e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6784e-131">id</span><span class="sxs-lookup"><span data-stu-id="6784e-131">id</span></span>|<span data-ttu-id="6784e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="6784e-132">String</span></span>|<span data-ttu-id="6784e-133">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="6784e-133">Id of the entity</span></span>|
|<span data-ttu-id="6784e-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="6784e-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="6784e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6784e-135">DateTimeOffset</span></span>|<span data-ttu-id="6784e-136">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="6784e-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="6784e-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="6784e-137">partnerState</span></span>|[<span data-ttu-id="6784e-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="6784e-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="6784e-139">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="6784e-139">Partner state of this tenant.</span></span> <span data-ttu-id="6784e-140">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="6784e-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="6784e-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="6784e-141">partnerAppType</span></span>|[<span data-ttu-id="6784e-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="6784e-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="6784e-143">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="6784e-143">Partner App type.</span></span> <span data-ttu-id="6784e-144">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="6784e-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="6784e-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="6784e-145">singleTenantAppId</span></span>|<span data-ttu-id="6784e-146">String</span><span class="sxs-lookup"><span data-stu-id="6784e-146">String</span></span>|<span data-ttu-id="6784e-147">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="6784e-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="6784e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="6784e-148">displayName</span></span>|<span data-ttu-id="6784e-149">字符串</span><span class="sxs-lookup"><span data-stu-id="6784e-149">String</span></span>|<span data-ttu-id="6784e-150">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="6784e-150">Partner display name</span></span>|
|<span data-ttu-id="6784e-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="6784e-151">isConfigured</span></span>|<span data-ttu-id="6784e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="6784e-152">Boolean</span></span>|<span data-ttu-id="6784e-153">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6784e-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="6784e-154">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="6784e-154">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="6784e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6784e-155">DateTimeOffset</span></span>|<span data-ttu-id="6784e-156">将删除 PartnerDevices 时，UTC 格式的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="6784e-156">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="6784e-157">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="6784e-157">This will become obselete soon.</span></span>|
|<span data-ttu-id="6784e-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="6784e-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="6784e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6784e-159">DateTimeOffset</span></span>|<span data-ttu-id="6784e-160">PartnerDevices 将被标记为不符合时的 UTC 格式的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6784e-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="6784e-161">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="6784e-161">This will become obselete soon.</span></span>|
|<span data-ttu-id="6784e-162">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="6784e-162">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="6784e-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6784e-163">DateTimeOffset</span></span>|<span data-ttu-id="6784e-164">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="6784e-164">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="6784e-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="6784e-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="6784e-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6784e-166">DateTimeOffset</span></span>|<span data-ttu-id="6784e-167">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="6784e-167">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="6784e-168">groupsRequiringPartnerEnrollment</span><span class="sxs-lookup"><span data-stu-id="6784e-168">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="6784e-169">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6784e-169">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="6784e-170">指定注册是否通过合作伙伴的用户组。</span><span class="sxs-lookup"><span data-stu-id="6784e-170">User groups that specifies whether enrollment is through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6784e-171">关系</span><span class="sxs-lookup"><span data-stu-id="6784e-171">Relationships</span></span>
<span data-ttu-id="6784e-172">无</span><span class="sxs-lookup"><span data-stu-id="6784e-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6784e-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6784e-173">JSON Representation</span></span>
<span data-ttu-id="6784e-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6784e-174">Here is a JSON representation of the resource.</span></span>
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
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String"
      }
    }
  ]
}
```




