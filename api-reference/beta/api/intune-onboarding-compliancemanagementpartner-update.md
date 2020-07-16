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
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="c6072-103">更新 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c6072-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="c6072-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6072-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6072-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6072-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6072-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6072-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6072-107">更新[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6072-107">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6072-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6072-108">Prerequisites</span></span>
<span data-ttu-id="c6072-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6072-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6072-111">Permission type</span></span>|<span data-ttu-id="c6072-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6072-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6072-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6072-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6072-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6072-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6072-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6072-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6072-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6072-116">Not supported.</span></span>|
|<span data-ttu-id="c6072-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6072-117">Application</span></span>|<span data-ttu-id="c6072-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6072-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6072-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6072-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="c6072-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6072-120">Request headers</span></span>
|<span data-ttu-id="c6072-121">标头</span><span class="sxs-lookup"><span data-stu-id="c6072-121">Header</span></span>|<span data-ttu-id="c6072-122">值</span><span class="sxs-lookup"><span data-stu-id="c6072-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6072-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6072-123">Authorization</span></span>|<span data-ttu-id="c6072-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6072-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6072-125">接受</span><span class="sxs-lookup"><span data-stu-id="c6072-125">Accept</span></span>|<span data-ttu-id="c6072-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6072-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6072-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6072-127">Request body</span></span>
<span data-ttu-id="c6072-128">在请求正文中，提供[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6072-128">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="c6072-129">下表显示创建[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6072-129">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="c6072-130">属性</span><span class="sxs-lookup"><span data-stu-id="c6072-130">Property</span></span>|<span data-ttu-id="c6072-131">类型</span><span class="sxs-lookup"><span data-stu-id="c6072-131">Type</span></span>|<span data-ttu-id="c6072-132">说明</span><span class="sxs-lookup"><span data-stu-id="c6072-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6072-133">id</span><span class="sxs-lookup"><span data-stu-id="c6072-133">id</span></span>|<span data-ttu-id="c6072-134">String</span><span class="sxs-lookup"><span data-stu-id="c6072-134">String</span></span>|<span data-ttu-id="c6072-135">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="c6072-135">Id of the entity</span></span>|
|<span data-ttu-id="c6072-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c6072-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c6072-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6072-137">DateTimeOffset</span></span>|<span data-ttu-id="c6072-138">Admin 载入到合规性管理合作伙伴之后的最后一次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="c6072-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="c6072-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="c6072-139">partnerState</span></span>|[<span data-ttu-id="c6072-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c6072-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c6072-141">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="c6072-141">Partner state of this tenant.</span></span> <span data-ttu-id="c6072-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="c6072-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c6072-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c6072-143">displayName</span></span>|<span data-ttu-id="c6072-144">String</span><span class="sxs-lookup"><span data-stu-id="c6072-144">String</span></span>|<span data-ttu-id="c6072-145">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="c6072-145">Partner display name</span></span>|
|<span data-ttu-id="c6072-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6072-146">macOsOnboarded</span></span>|<span data-ttu-id="c6072-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="c6072-147">Boolean</span></span>|<span data-ttu-id="c6072-148">适用于 Mac 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c6072-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="c6072-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6072-149">windowsOnboarded</span></span>|<span data-ttu-id="c6072-150">布尔值</span><span class="sxs-lookup"><span data-stu-id="c6072-150">Boolean</span></span>|<span data-ttu-id="c6072-151">适用于 Windows 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c6072-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="c6072-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6072-152">androidOnboarded</span></span>|<span data-ttu-id="c6072-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="c6072-153">Boolean</span></span>|<span data-ttu-id="c6072-154">适用于 Android 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c6072-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="c6072-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="c6072-155">iosOnboarded</span></span>|<span data-ttu-id="c6072-156">布尔值</span><span class="sxs-lookup"><span data-stu-id="c6072-156">Boolean</span></span>|<span data-ttu-id="c6072-157">适用于 ios 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c6072-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="c6072-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6072-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="c6072-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6072-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6072-160">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c6072-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="c6072-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6072-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="c6072-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6072-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6072-163">通过合作伙伴注册 Windows 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c6072-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="c6072-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6072-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="c6072-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6072-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6072-166">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c6072-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="c6072-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6072-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="c6072-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6072-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c6072-169">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c6072-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c6072-170">响应</span><span class="sxs-lookup"><span data-stu-id="c6072-170">Response</span></span>
<span data-ttu-id="c6072-171">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6072-171">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6072-172">示例</span><span class="sxs-lookup"><span data-stu-id="c6072-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6072-173">请求</span><span class="sxs-lookup"><span data-stu-id="c6072-173">Request</span></span>
<span data-ttu-id="c6072-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6072-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6072-175">响应</span><span class="sxs-lookup"><span data-stu-id="c6072-175">Response</span></span>
<span data-ttu-id="c6072-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6072-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



