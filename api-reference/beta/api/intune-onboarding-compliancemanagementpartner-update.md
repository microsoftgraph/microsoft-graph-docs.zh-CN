---
title: 更新 complianceManagementPartner
description: 更新 complianceManagementPartner 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 349932132867d00708a400e82465c664db551f97
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791831"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="1ed2e-103">更新 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1ed2e-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="1ed2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ed2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ed2e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed2e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed2e-107">更新[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-107">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ed2e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ed2e-108">Prerequisites</span></span>
<span data-ttu-id="1ed2e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1ed2e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1ed2e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed2e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed2e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ed2e-111">Permission type</span></span>|<span data-ttu-id="1ed2e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ed2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ed2e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ed2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ed2e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed2e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1ed2e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ed2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-116">Not supported.</span></span>|
|<span data-ttu-id="1ed2e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ed2e-117">Application</span></span>|<span data-ttu-id="1ed2e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed2e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ed2e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ed2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="1ed2e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ed2e-120">Request headers</span></span>
|<span data-ttu-id="1ed2e-121">标头</span><span class="sxs-lookup"><span data-stu-id="1ed2e-121">Header</span></span>|<span data-ttu-id="1ed2e-122">值</span><span class="sxs-lookup"><span data-stu-id="1ed2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ed2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ed2e-123">Authorization</span></span>|<span data-ttu-id="1ed2e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ed2e-125">接受</span><span class="sxs-lookup"><span data-stu-id="1ed2e-125">Accept</span></span>|<span data-ttu-id="1ed2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed2e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ed2e-127">Request body</span></span>
<span data-ttu-id="1ed2e-128">在请求正文中，提供[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-128">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="1ed2e-129">下表显示创建[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-129">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="1ed2e-130">属性</span><span class="sxs-lookup"><span data-stu-id="1ed2e-130">Property</span></span>|<span data-ttu-id="1ed2e-131">类型</span><span class="sxs-lookup"><span data-stu-id="1ed2e-131">Type</span></span>|<span data-ttu-id="1ed2e-132">说明</span><span class="sxs-lookup"><span data-stu-id="1ed2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed2e-133">id</span><span class="sxs-lookup"><span data-stu-id="1ed2e-133">id</span></span>|<span data-ttu-id="1ed2e-134">String</span><span class="sxs-lookup"><span data-stu-id="1ed2e-134">String</span></span>|<span data-ttu-id="1ed2e-135">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="1ed2e-135">Id of the entity</span></span>|
|<span data-ttu-id="1ed2e-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed2e-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="1ed2e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed2e-137">DateTimeOffset</span></span>|<span data-ttu-id="1ed2e-138">Admin 载入到合规性管理合作伙伴之后的最后一次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="1ed2e-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="1ed2e-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="1ed2e-139">partnerState</span></span>|[<span data-ttu-id="1ed2e-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="1ed2e-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="1ed2e-141">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-141">Partner state of this tenant.</span></span> <span data-ttu-id="1ed2e-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="1ed2e-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1ed2e-143">displayName</span></span>|<span data-ttu-id="1ed2e-144">String</span><span class="sxs-lookup"><span data-stu-id="1ed2e-144">String</span></span>|<span data-ttu-id="1ed2e-145">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="1ed2e-145">Partner display name</span></span>|
|<span data-ttu-id="1ed2e-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="1ed2e-146">macOsOnboarded</span></span>|<span data-ttu-id="1ed2e-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="1ed2e-147">Boolean</span></span>|<span data-ttu-id="1ed2e-148">适用于 Mac 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="1ed2e-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="1ed2e-149">windowsOnboarded</span></span>|<span data-ttu-id="1ed2e-150">布尔值</span><span class="sxs-lookup"><span data-stu-id="1ed2e-150">Boolean</span></span>|<span data-ttu-id="1ed2e-151">适用于 Windows 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="1ed2e-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="1ed2e-152">androidOnboarded</span></span>|<span data-ttu-id="1ed2e-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="1ed2e-153">Boolean</span></span>|<span data-ttu-id="1ed2e-154">适用于 Android 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="1ed2e-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="1ed2e-155">iosOnboarded</span></span>|<span data-ttu-id="1ed2e-156">布尔值</span><span class="sxs-lookup"><span data-stu-id="1ed2e-156">Boolean</span></span>|<span data-ttu-id="1ed2e-157">适用于 ios 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="1ed2e-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1ed2e-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="1ed2e-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1ed2e-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1ed2e-160">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="1ed2e-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1ed2e-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="1ed2e-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1ed2e-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1ed2e-163">通过合作伙伴注册 Windows 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="1ed2e-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1ed2e-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="1ed2e-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1ed2e-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1ed2e-166">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="1ed2e-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1ed2e-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="1ed2e-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1ed2e-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1ed2e-169">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="1ed2e-170">响应</span><span class="sxs-lookup"><span data-stu-id="1ed2e-170">Response</span></span>
<span data-ttu-id="1ed2e-171">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-171">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed2e-172">示例</span><span class="sxs-lookup"><span data-stu-id="1ed2e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ed2e-173">请求</span><span class="sxs-lookup"><span data-stu-id="1ed2e-173">Request</span></span>
<span data-ttu-id="1ed2e-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ed2e-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 1944

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1ed2e-175">响应</span><span class="sxs-lookup"><span data-stu-id="1ed2e-175">Response</span></span>
<span data-ttu-id="1ed2e-176">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1ed2e-176">Here is an example of the response.</span></span> <span data-ttu-id="1ed2e-177">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1ed2e-177">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1ed2e-178">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1ed2e-178">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1993

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



