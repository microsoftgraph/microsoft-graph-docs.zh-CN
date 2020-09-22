---
title: 创建 complianceManagementPartner
description: 创建新的 complianceManagementPartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc19f43993281fb3ffe2543d8bfaf96a9f3b06ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972110"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="c83d5-103">创建 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c83d5-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="c83d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c83d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c83d5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c83d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c83d5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c83d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c83d5-107">创建新的 [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c83d5-107">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c83d5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c83d5-108">Prerequisites</span></span>
<span data-ttu-id="c83d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c83d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c83d5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c83d5-111">Permission type</span></span>|<span data-ttu-id="c83d5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c83d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c83d5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c83d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c83d5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c83d5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c83d5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c83d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c83d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c83d5-116">Not supported.</span></span>|
|<span data-ttu-id="c83d5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c83d5-117">Application</span></span>|<span data-ttu-id="c83d5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c83d5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c83d5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c83d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="c83d5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c83d5-120">Request headers</span></span>
|<span data-ttu-id="c83d5-121">标头</span><span class="sxs-lookup"><span data-stu-id="c83d5-121">Header</span></span>|<span data-ttu-id="c83d5-122">值</span><span class="sxs-lookup"><span data-stu-id="c83d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c83d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c83d5-123">Authorization</span></span>|<span data-ttu-id="c83d5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c83d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c83d5-125">接受</span><span class="sxs-lookup"><span data-stu-id="c83d5-125">Accept</span></span>|<span data-ttu-id="c83d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c83d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c83d5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c83d5-127">Request body</span></span>
<span data-ttu-id="c83d5-128">在请求正文中，提供 complianceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c83d5-128">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="c83d5-129">下表显示创建 complianceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c83d5-129">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="c83d5-130">属性</span><span class="sxs-lookup"><span data-stu-id="c83d5-130">Property</span></span>|<span data-ttu-id="c83d5-131">类型</span><span class="sxs-lookup"><span data-stu-id="c83d5-131">Type</span></span>|<span data-ttu-id="c83d5-132">说明</span><span class="sxs-lookup"><span data-stu-id="c83d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c83d5-133">id</span><span class="sxs-lookup"><span data-stu-id="c83d5-133">id</span></span>|<span data-ttu-id="c83d5-134">String</span><span class="sxs-lookup"><span data-stu-id="c83d5-134">String</span></span>|<span data-ttu-id="c83d5-135">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="c83d5-135">Id of the entity</span></span>|
|<span data-ttu-id="c83d5-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c83d5-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c83d5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83d5-137">DateTimeOffset</span></span>|<span data-ttu-id="c83d5-138">Admin 载入到合规性管理合作伙伴之后的最后一次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="c83d5-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="c83d5-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="c83d5-139">partnerState</span></span>|[<span data-ttu-id="c83d5-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c83d5-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c83d5-141">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="c83d5-141">Partner state of this tenant.</span></span> <span data-ttu-id="c83d5-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="c83d5-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c83d5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c83d5-143">displayName</span></span>|<span data-ttu-id="c83d5-144">String</span><span class="sxs-lookup"><span data-stu-id="c83d5-144">String</span></span>|<span data-ttu-id="c83d5-145">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="c83d5-145">Partner display name</span></span>|
|<span data-ttu-id="c83d5-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c83d5-146">macOsOnboarded</span></span>|<span data-ttu-id="c83d5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83d5-147">Boolean</span></span>|<span data-ttu-id="c83d5-148">适用于 Mac 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c83d5-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="c83d5-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="c83d5-149">windowsOnboarded</span></span>|<span data-ttu-id="c83d5-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83d5-150">Boolean</span></span>|<span data-ttu-id="c83d5-151">适用于 Windows 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c83d5-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="c83d5-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="c83d5-152">androidOnboarded</span></span>|<span data-ttu-id="c83d5-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83d5-153">Boolean</span></span>|<span data-ttu-id="c83d5-154">适用于 Android 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c83d5-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="c83d5-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="c83d5-155">iosOnboarded</span></span>|<span data-ttu-id="c83d5-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83d5-156">Boolean</span></span>|<span data-ttu-id="c83d5-157">适用于 ios 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="c83d5-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="c83d5-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c83d5-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="c83d5-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c83d5-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c83d5-160">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c83d5-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="c83d5-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c83d5-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="c83d5-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c83d5-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c83d5-163">通过合作伙伴注册 Windows 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c83d5-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="c83d5-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c83d5-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="c83d5-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c83d5-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c83d5-166">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c83d5-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="c83d5-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="c83d5-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="c83d5-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c83d5-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c83d5-169">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="c83d5-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c83d5-170">响应</span><span class="sxs-lookup"><span data-stu-id="c83d5-170">Response</span></span>
<span data-ttu-id="c83d5-171">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c83d5-171">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c83d5-172">示例</span><span class="sxs-lookup"><span data-stu-id="c83d5-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="c83d5-173">请求</span><span class="sxs-lookup"><span data-stu-id="c83d5-173">Request</span></span>
<span data-ttu-id="c83d5-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c83d5-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
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

### <a name="response"></a><span data-ttu-id="c83d5-175">响应</span><span class="sxs-lookup"><span data-stu-id="c83d5-175">Response</span></span>
<span data-ttu-id="c83d5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c83d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






