---
title: 更新 complianceManagementPartner
description: 更新 complianceManagementPartner 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5e8befa9726114ff6159a545db5d8f20b58123b
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086681"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="bf0d8-103">更新 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="bf0d8-103">Update complianceManagementPartner</span></span>

> <span data-ttu-id="bf0d8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf0d8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf0d8-106">更新[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-106">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf0d8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf0d8-107">Prerequisites</span></span>
<span data-ttu-id="bf0d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf0d8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf0d8-110">Permission type</span></span>|<span data-ttu-id="bf0d8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf0d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf0d8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf0d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf0d8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf0d8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf0d8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf0d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf0d8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-115">Not supported.</span></span>|
|<span data-ttu-id="bf0d8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf0d8-116">Application</span></span>|<span data-ttu-id="bf0d8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf0d8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf0d8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf0d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="bf0d8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf0d8-119">Request headers</span></span>
|<span data-ttu-id="bf0d8-120">标头</span><span class="sxs-lookup"><span data-stu-id="bf0d8-120">Header</span></span>|<span data-ttu-id="bf0d8-121">值</span><span class="sxs-lookup"><span data-stu-id="bf0d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf0d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf0d8-122">Authorization</span></span>|<span data-ttu-id="bf0d8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf0d8-124">接受</span><span class="sxs-lookup"><span data-stu-id="bf0d8-124">Accept</span></span>|<span data-ttu-id="bf0d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf0d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf0d8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf0d8-126">Request body</span></span>
<span data-ttu-id="bf0d8-127">在请求正文中，提供[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-127">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="bf0d8-128">下表显示创建[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-128">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="bf0d8-129">属性</span><span class="sxs-lookup"><span data-stu-id="bf0d8-129">Property</span></span>|<span data-ttu-id="bf0d8-130">类型</span><span class="sxs-lookup"><span data-stu-id="bf0d8-130">Type</span></span>|<span data-ttu-id="bf0d8-131">说明</span><span class="sxs-lookup"><span data-stu-id="bf0d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf0d8-132">id</span><span class="sxs-lookup"><span data-stu-id="bf0d8-132">id</span></span>|<span data-ttu-id="bf0d8-133">String</span><span class="sxs-lookup"><span data-stu-id="bf0d8-133">String</span></span>|<span data-ttu-id="bf0d8-134">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="bf0d8-134">Id of the entity</span></span>|
|<span data-ttu-id="bf0d8-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="bf0d8-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="bf0d8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf0d8-136">DateTimeOffset</span></span>|<span data-ttu-id="bf0d8-137">Admin 载入到合规性管理合作伙伴之后的最后一次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="bf0d8-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="bf0d8-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="bf0d8-138">partnerState</span></span>|[<span data-ttu-id="bf0d8-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="bf0d8-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="bf0d8-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-140">Partner state of this tenant.</span></span> <span data-ttu-id="bf0d8-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="bf0d8-142">displayName</span><span class="sxs-lookup"><span data-stu-id="bf0d8-142">displayName</span></span>|<span data-ttu-id="bf0d8-143">String</span><span class="sxs-lookup"><span data-stu-id="bf0d8-143">String</span></span>|<span data-ttu-id="bf0d8-144">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="bf0d8-144">Partner display name</span></span>|
|<span data-ttu-id="bf0d8-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="bf0d8-145">macOsOnboarded</span></span>|<span data-ttu-id="bf0d8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf0d8-146">Boolean</span></span>|<span data-ttu-id="bf0d8-147">适用于 Mac 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="bf0d8-148">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="bf0d8-148">windowsOnboarded</span></span>|<span data-ttu-id="bf0d8-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf0d8-149">Boolean</span></span>|<span data-ttu-id="bf0d8-150">适用于 Windows 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-150">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="bf0d8-151">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="bf0d8-151">androidOnboarded</span></span>|<span data-ttu-id="bf0d8-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf0d8-152">Boolean</span></span>|<span data-ttu-id="bf0d8-153">适用于 Android 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-153">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="bf0d8-154">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="bf0d8-154">iosOnboarded</span></span>|<span data-ttu-id="bf0d8-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf0d8-155">Boolean</span></span>|<span data-ttu-id="bf0d8-156">适用于 ios 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-156">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="bf0d8-157">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="bf0d8-157">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="bf0d8-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf0d8-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="bf0d8-159">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-159">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="bf0d8-160">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="bf0d8-160">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="bf0d8-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf0d8-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="bf0d8-162">通过合作伙伴注册 Windows 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-162">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="bf0d8-163">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="bf0d8-163">androidEnrollmentAssignments</span></span>|<span data-ttu-id="bf0d8-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf0d8-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="bf0d8-165">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-165">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="bf0d8-166">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="bf0d8-166">iosEnrollmentAssignments</span></span>|<span data-ttu-id="bf0d8-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf0d8-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="bf0d8-168">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-168">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="bf0d8-169">响应</span><span class="sxs-lookup"><span data-stu-id="bf0d8-169">Response</span></span>
<span data-ttu-id="bf0d8-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-170">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf0d8-171">示例</span><span class="sxs-lookup"><span data-stu-id="bf0d8-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf0d8-172">请求</span><span class="sxs-lookup"><span data-stu-id="bf0d8-172">Request</span></span>
<span data-ttu-id="bf0d8-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 1244

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bf0d8-174">响应</span><span class="sxs-lookup"><span data-stu-id="bf0d8-174">Response</span></span>
<span data-ttu-id="bf0d8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf0d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1293

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```






