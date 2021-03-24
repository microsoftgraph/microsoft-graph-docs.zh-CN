---
title: 更新 deviceManagementPartner
description: 更新 deviceManagementPartner 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e75644c57fdee030bd0fc8858d49ed7f0625dbe2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145451"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="ac949-103">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ac949-103">Update deviceManagementPartner</span></span>

<span data-ttu-id="ac949-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac949-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac949-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ac949-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac949-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac949-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac949-107">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ac949-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac949-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ac949-108">Prerequisites</span></span>
<span data-ttu-id="ac949-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac949-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac949-111">Permission type</span></span>|<span data-ttu-id="ac949-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac949-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac949-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac949-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac949-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac949-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ac949-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac949-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac949-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac949-116">Not supported.</span></span>|
|<span data-ttu-id="ac949-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac949-117">Application</span></span>|<span data-ttu-id="ac949-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac949-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac949-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac949-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="ac949-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac949-120">Request headers</span></span>
|<span data-ttu-id="ac949-121">标头</span><span class="sxs-lookup"><span data-stu-id="ac949-121">Header</span></span>|<span data-ttu-id="ac949-122">值</span><span class="sxs-lookup"><span data-stu-id="ac949-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac949-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac949-123">Authorization</span></span>|<span data-ttu-id="ac949-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ac949-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac949-125">接受</span><span class="sxs-lookup"><span data-stu-id="ac949-125">Accept</span></span>|<span data-ttu-id="ac949-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac949-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac949-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac949-127">Request body</span></span>
<span data-ttu-id="ac949-128">在请求正文中，提供 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac949-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="ac949-129">下表显示创建 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ac949-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="ac949-130">属性</span><span class="sxs-lookup"><span data-stu-id="ac949-130">Property</span></span>|<span data-ttu-id="ac949-131">类型</span><span class="sxs-lookup"><span data-stu-id="ac949-131">Type</span></span>|<span data-ttu-id="ac949-132">说明</span><span class="sxs-lookup"><span data-stu-id="ac949-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac949-133">id</span><span class="sxs-lookup"><span data-stu-id="ac949-133">id</span></span>|<span data-ttu-id="ac949-134">String</span><span class="sxs-lookup"><span data-stu-id="ac949-134">String</span></span>|<span data-ttu-id="ac949-135">实体的 ID</span><span class="sxs-lookup"><span data-stu-id="ac949-135">Id of the entity</span></span>|
|<span data-ttu-id="ac949-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="ac949-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="ac949-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac949-137">DateTimeOffset</span></span>|<span data-ttu-id="ac949-138">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="ac949-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="ac949-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="ac949-139">partnerState</span></span>|[<span data-ttu-id="ac949-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="ac949-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="ac949-141">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="ac949-141">Partner state of this tenant.</span></span> <span data-ttu-id="ac949-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="ac949-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="ac949-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="ac949-143">partnerAppType</span></span>|[<span data-ttu-id="ac949-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="ac949-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="ac949-145">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="ac949-145">Partner App type.</span></span> <span data-ttu-id="ac949-146">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="ac949-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="ac949-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="ac949-147">singleTenantAppId</span></span>|<span data-ttu-id="ac949-148">String</span><span class="sxs-lookup"><span data-stu-id="ac949-148">String</span></span>|<span data-ttu-id="ac949-149">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="ac949-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="ac949-150">displayName</span><span class="sxs-lookup"><span data-stu-id="ac949-150">displayName</span></span>|<span data-ttu-id="ac949-151">String</span><span class="sxs-lookup"><span data-stu-id="ac949-151">String</span></span>|<span data-ttu-id="ac949-152">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="ac949-152">Partner display name</span></span>|
|<span data-ttu-id="ac949-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="ac949-153">isConfigured</span></span>|<span data-ttu-id="ac949-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac949-154">Boolean</span></span>|<span data-ttu-id="ac949-155">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="ac949-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="ac949-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="ac949-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="ac949-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac949-157">DateTimeOffset</span></span>|<span data-ttu-id="ac949-158">将删除 PartnerDevices 的 DateTime（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="ac949-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="ac949-159">这将很快成为删除。</span><span class="sxs-lookup"><span data-stu-id="ac949-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="ac949-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="ac949-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="ac949-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac949-161">DateTimeOffset</span></span>|<span data-ttu-id="ac949-162">将 PartnerDevices 标记为"不兼容"的 DateTime（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="ac949-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="ac949-163">这将很快成为删除。</span><span class="sxs-lookup"><span data-stu-id="ac949-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="ac949-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac949-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="ac949-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac949-165">DateTimeOffset</span></span>|<span data-ttu-id="ac949-166">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="ac949-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="ac949-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="ac949-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="ac949-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac949-168">DateTimeOffset</span></span>|<span data-ttu-id="ac949-169">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="ac949-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="ac949-170">groupsRequiringPartnerEnrollment</span><span class="sxs-lookup"><span data-stu-id="ac949-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="ac949-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ac949-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="ac949-172">指定是否通过合作伙伴注册的用户组。</span><span class="sxs-lookup"><span data-stu-id="ac949-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="ac949-173">响应</span><span class="sxs-lookup"><span data-stu-id="ac949-173">Response</span></span>
<span data-ttu-id="ac949-174">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac949-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac949-175">示例</span><span class="sxs-lookup"><span data-stu-id="ac949-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac949-176">请求</span><span class="sxs-lookup"><span data-stu-id="ac949-176">Request</span></span>
<span data-ttu-id="ac949-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac949-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 1140

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ac949-178">响应</span><span class="sxs-lookup"><span data-stu-id="ac949-178">Response</span></span>
<span data-ttu-id="ac949-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac949-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1189

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




