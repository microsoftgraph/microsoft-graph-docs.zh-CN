---
title: 创建 deviceManagementPartner
description: 创建新的 deviceManagementPartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54851dee4415d97a6f430ef6ffaa361b5d16d2de
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791824"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="49709-103">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="49709-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="49709-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49709-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49709-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49709-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49709-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49709-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49709-107">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49709-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49709-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="49709-108">Prerequisites</span></span>
<span data-ttu-id="49709-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49709-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="49709-111">Permission type</span></span>|<span data-ttu-id="49709-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="49709-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49709-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49709-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49709-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49709-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49709-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49709-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49709-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49709-116">Not supported.</span></span>|
|<span data-ttu-id="49709-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="49709-117">Application</span></span>|<span data-ttu-id="49709-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49709-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49709-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49709-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="49709-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="49709-120">Request headers</span></span>
|<span data-ttu-id="49709-121">标头</span><span class="sxs-lookup"><span data-stu-id="49709-121">Header</span></span>|<span data-ttu-id="49709-122">值</span><span class="sxs-lookup"><span data-stu-id="49709-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49709-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49709-123">Authorization</span></span>|<span data-ttu-id="49709-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="49709-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49709-125">接受</span><span class="sxs-lookup"><span data-stu-id="49709-125">Accept</span></span>|<span data-ttu-id="49709-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49709-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49709-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="49709-127">Request body</span></span>
<span data-ttu-id="49709-128">在请求正文中，提供 deviceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49709-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="49709-129">下表显示创建 deviceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="49709-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="49709-130">属性</span><span class="sxs-lookup"><span data-stu-id="49709-130">Property</span></span>|<span data-ttu-id="49709-131">类型</span><span class="sxs-lookup"><span data-stu-id="49709-131">Type</span></span>|<span data-ttu-id="49709-132">说明</span><span class="sxs-lookup"><span data-stu-id="49709-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49709-133">id</span><span class="sxs-lookup"><span data-stu-id="49709-133">id</span></span>|<span data-ttu-id="49709-134">String</span><span class="sxs-lookup"><span data-stu-id="49709-134">String</span></span>|<span data-ttu-id="49709-135">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="49709-135">Id of the entity</span></span>|
|<span data-ttu-id="49709-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="49709-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="49709-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49709-137">DateTimeOffset</span></span>|<span data-ttu-id="49709-138">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="49709-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="49709-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="49709-139">partnerState</span></span>|[<span data-ttu-id="49709-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="49709-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="49709-141">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="49709-141">Partner state of this tenant.</span></span> <span data-ttu-id="49709-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="49709-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="49709-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="49709-143">partnerAppType</span></span>|[<span data-ttu-id="49709-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="49709-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="49709-145">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="49709-145">Partner App type.</span></span> <span data-ttu-id="49709-146">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="49709-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="49709-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="49709-147">singleTenantAppId</span></span>|<span data-ttu-id="49709-148">String</span><span class="sxs-lookup"><span data-stu-id="49709-148">String</span></span>|<span data-ttu-id="49709-149">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="49709-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="49709-150">displayName</span><span class="sxs-lookup"><span data-stu-id="49709-150">displayName</span></span>|<span data-ttu-id="49709-151">String</span><span class="sxs-lookup"><span data-stu-id="49709-151">String</span></span>|<span data-ttu-id="49709-152">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="49709-152">Partner display name</span></span>|
|<span data-ttu-id="49709-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="49709-153">isConfigured</span></span>|<span data-ttu-id="49709-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="49709-154">Boolean</span></span>|<span data-ttu-id="49709-155">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="49709-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="49709-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="49709-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="49709-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49709-157">DateTimeOffset</span></span>|<span data-ttu-id="49709-158">将删除 PartnerDevices 时，UTC 格式的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="49709-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="49709-159">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="49709-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="49709-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="49709-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="49709-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49709-161">DateTimeOffset</span></span>|<span data-ttu-id="49709-162">PartnerDevices 将被标记为不符合时的 UTC 格式的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="49709-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="49709-163">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="49709-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="49709-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="49709-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="49709-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49709-165">DateTimeOffset</span></span>|<span data-ttu-id="49709-166">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="49709-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="49709-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="49709-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="49709-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49709-168">DateTimeOffset</span></span>|<span data-ttu-id="49709-169">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="49709-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="49709-170">groupsRequiringPartnerEnrollment</span><span class="sxs-lookup"><span data-stu-id="49709-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="49709-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="49709-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="49709-172">指定注册是否通过合作伙伴的用户组。</span><span class="sxs-lookup"><span data-stu-id="49709-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="49709-173">响应</span><span class="sxs-lookup"><span data-stu-id="49709-173">Response</span></span>
<span data-ttu-id="49709-174">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49709-174">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49709-175">示例</span><span class="sxs-lookup"><span data-stu-id="49709-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="49709-176">请求</span><span class="sxs-lookup"><span data-stu-id="49709-176">Request</span></span>
<span data-ttu-id="49709-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49709-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 1072

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="49709-178">响应</span><span class="sxs-lookup"><span data-stu-id="49709-178">Response</span></span>
<span data-ttu-id="49709-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49709-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1121

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



