---
title: 创建 complianceManagementPartner
description: 创建新的 complianceManagementPartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c606f0fdf4fbf9f589c2aab2423373225f1bdf7c
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744124"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="cab2d-103">创建 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="cab2d-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="cab2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cab2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cab2d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cab2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cab2d-106">创建新的[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cab2d-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cab2d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cab2d-107">Prerequisites</span></span>
<span data-ttu-id="cab2d-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cab2d-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cab2d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cab2d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cab2d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cab2d-110">Permission type</span></span>|<span data-ttu-id="cab2d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cab2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cab2d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cab2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cab2d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab2d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cab2d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cab2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cab2d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cab2d-115">Not supported.</span></span>|
|<span data-ttu-id="cab2d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cab2d-116">Application</span></span>|<span data-ttu-id="cab2d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab2d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cab2d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cab2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="cab2d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cab2d-119">Request headers</span></span>
|<span data-ttu-id="cab2d-120">标头</span><span class="sxs-lookup"><span data-stu-id="cab2d-120">Header</span></span>|<span data-ttu-id="cab2d-121">值</span><span class="sxs-lookup"><span data-stu-id="cab2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cab2d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cab2d-122">Authorization</span></span>|<span data-ttu-id="cab2d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cab2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cab2d-124">接受</span><span class="sxs-lookup"><span data-stu-id="cab2d-124">Accept</span></span>|<span data-ttu-id="cab2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cab2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cab2d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cab2d-126">Request body</span></span>
<span data-ttu-id="cab2d-127">在请求正文中，提供 complianceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cab2d-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="cab2d-128">下表显示创建 complianceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cab2d-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="cab2d-129">属性</span><span class="sxs-lookup"><span data-stu-id="cab2d-129">Property</span></span>|<span data-ttu-id="cab2d-130">类型</span><span class="sxs-lookup"><span data-stu-id="cab2d-130">Type</span></span>|<span data-ttu-id="cab2d-131">说明</span><span class="sxs-lookup"><span data-stu-id="cab2d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cab2d-132">id</span><span class="sxs-lookup"><span data-stu-id="cab2d-132">id</span></span>|<span data-ttu-id="cab2d-133">String</span><span class="sxs-lookup"><span data-stu-id="cab2d-133">String</span></span>|<span data-ttu-id="cab2d-134">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="cab2d-134">Id of the entity</span></span>|
|<span data-ttu-id="cab2d-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="cab2d-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="cab2d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cab2d-136">DateTimeOffset</span></span>|<span data-ttu-id="cab2d-137">Admin 载入到合规性管理合作伙伴之后的最后一次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="cab2d-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="cab2d-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="cab2d-138">partnerState</span></span>|[<span data-ttu-id="cab2d-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="cab2d-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="cab2d-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="cab2d-140">Partner state of this tenant.</span></span> <span data-ttu-id="cab2d-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="cab2d-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="cab2d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="cab2d-142">displayName</span></span>|<span data-ttu-id="cab2d-143">String</span><span class="sxs-lookup"><span data-stu-id="cab2d-143">String</span></span>|<span data-ttu-id="cab2d-144">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="cab2d-144">Partner display name</span></span>|
|<span data-ttu-id="cab2d-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="cab2d-145">macOsOnboarded</span></span>|<span data-ttu-id="cab2d-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="cab2d-146">Boolean</span></span>|<span data-ttu-id="cab2d-147">适用于 Mac 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="cab2d-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="cab2d-148">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="cab2d-148">androidOnboarded</span></span>|<span data-ttu-id="cab2d-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="cab2d-149">Boolean</span></span>|<span data-ttu-id="cab2d-150">适用于 Android 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="cab2d-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="cab2d-151">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="cab2d-151">iosOnboarded</span></span>|<span data-ttu-id="cab2d-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="cab2d-152">Boolean</span></span>|<span data-ttu-id="cab2d-153">适用于 ios 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="cab2d-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="cab2d-154">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="cab2d-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="cab2d-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="cab2d-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="cab2d-156">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="cab2d-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="cab2d-157">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="cab2d-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="cab2d-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="cab2d-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="cab2d-159">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="cab2d-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="cab2d-160">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="cab2d-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="cab2d-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="cab2d-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="cab2d-162">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="cab2d-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="cab2d-163">响应</span><span class="sxs-lookup"><span data-stu-id="cab2d-163">Response</span></span>
<span data-ttu-id="cab2d-164">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cab2d-164">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cab2d-165">示例</span><span class="sxs-lookup"><span data-stu-id="cab2d-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="cab2d-166">请求</span><span class="sxs-lookup"><span data-stu-id="cab2d-166">Request</span></span>
<span data-ttu-id="cab2d-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cab2d-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 982

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
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

### <a name="response"></a><span data-ttu-id="cab2d-168">响应</span><span class="sxs-lookup"><span data-stu-id="cab2d-168">Response</span></span>
<span data-ttu-id="cab2d-169">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="cab2d-169">Here is an example of the response.</span></span> <span data-ttu-id="cab2d-170">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="cab2d-170">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cab2d-171">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="cab2d-171">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1031

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
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



