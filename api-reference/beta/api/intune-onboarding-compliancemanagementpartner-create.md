---
title: 创建 complianceManagementPartner
description: 创建新的 complianceManagementPartner 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afedb4cb5b55aff57cd599364b2576e590fccd66
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803075"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="3ca18-103">创建 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3ca18-103">Create complianceManagementPartner</span></span>

> <span data-ttu-id="3ca18-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ca18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ca18-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ca18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ca18-106">创建新的[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3ca18-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ca18-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3ca18-107">Prerequisites</span></span>
<span data-ttu-id="3ca18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ca18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ca18-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ca18-110">Permission type</span></span>|<span data-ttu-id="3ca18-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3ca18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ca18-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ca18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ca18-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ca18-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3ca18-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ca18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ca18-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ca18-115">Not supported.</span></span>|
|<span data-ttu-id="3ca18-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ca18-116">Application</span></span>|<span data-ttu-id="3ca18-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ca18-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ca18-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ca18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="3ca18-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ca18-119">Request headers</span></span>
|<span data-ttu-id="3ca18-120">标头</span><span class="sxs-lookup"><span data-stu-id="3ca18-120">Header</span></span>|<span data-ttu-id="3ca18-121">值</span><span class="sxs-lookup"><span data-stu-id="3ca18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ca18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ca18-122">Authorization</span></span>|<span data-ttu-id="3ca18-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3ca18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ca18-124">接受</span><span class="sxs-lookup"><span data-stu-id="3ca18-124">Accept</span></span>|<span data-ttu-id="3ca18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ca18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ca18-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ca18-126">Request body</span></span>
<span data-ttu-id="3ca18-127">在请求正文中，提供 complianceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ca18-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="3ca18-128">下表显示创建 complianceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3ca18-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="3ca18-129">属性</span><span class="sxs-lookup"><span data-stu-id="3ca18-129">Property</span></span>|<span data-ttu-id="3ca18-130">类型</span><span class="sxs-lookup"><span data-stu-id="3ca18-130">Type</span></span>|<span data-ttu-id="3ca18-131">说明</span><span class="sxs-lookup"><span data-stu-id="3ca18-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ca18-132">id</span><span class="sxs-lookup"><span data-stu-id="3ca18-132">id</span></span>|<span data-ttu-id="3ca18-133">String</span><span class="sxs-lookup"><span data-stu-id="3ca18-133">String</span></span>|<span data-ttu-id="3ca18-134">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="3ca18-134">Id of the entity</span></span>|
|<span data-ttu-id="3ca18-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="3ca18-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="3ca18-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ca18-136">DateTimeOffset</span></span>|<span data-ttu-id="3ca18-137">Admin 载入到合规性管理合作伙伴之后的最后一次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="3ca18-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="3ca18-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="3ca18-138">partnerState</span></span>|[<span data-ttu-id="3ca18-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="3ca18-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="3ca18-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="3ca18-140">Partner state of this tenant.</span></span> <span data-ttu-id="3ca18-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="3ca18-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="3ca18-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3ca18-142">displayName</span></span>|<span data-ttu-id="3ca18-143">String</span><span class="sxs-lookup"><span data-stu-id="3ca18-143">String</span></span>|<span data-ttu-id="3ca18-144">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="3ca18-144">Partner display name</span></span>|
|<span data-ttu-id="3ca18-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="3ca18-145">macOsOnboarded</span></span>|<span data-ttu-id="3ca18-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="3ca18-146">Boolean</span></span>|<span data-ttu-id="3ca18-147">适用于 Mac 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="3ca18-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="3ca18-148">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="3ca18-148">windowsOnboarded</span></span>|<span data-ttu-id="3ca18-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="3ca18-149">Boolean</span></span>|<span data-ttu-id="3ca18-150">适用于 Windows 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="3ca18-150">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="3ca18-151">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="3ca18-151">androidOnboarded</span></span>|<span data-ttu-id="3ca18-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="3ca18-152">Boolean</span></span>|<span data-ttu-id="3ca18-153">适用于 Android 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="3ca18-153">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="3ca18-154">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="3ca18-154">iosOnboarded</span></span>|<span data-ttu-id="3ca18-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="3ca18-155">Boolean</span></span>|<span data-ttu-id="3ca18-156">适用于 ios 设备的合作伙伴载入。</span><span class="sxs-lookup"><span data-stu-id="3ca18-156">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="3ca18-157">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="3ca18-157">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="3ca18-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ca18-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3ca18-159">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="3ca18-159">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="3ca18-160">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="3ca18-160">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="3ca18-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ca18-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3ca18-162">通过合作伙伴注册 Windows 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="3ca18-162">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="3ca18-163">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="3ca18-163">androidEnrollmentAssignments</span></span>|<span data-ttu-id="3ca18-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ca18-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3ca18-165">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="3ca18-165">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="3ca18-166">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="3ca18-166">iosEnrollmentAssignments</span></span>|<span data-ttu-id="3ca18-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ca18-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3ca18-168">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="3ca18-168">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="3ca18-169">响应</span><span class="sxs-lookup"><span data-stu-id="3ca18-169">Response</span></span>
<span data-ttu-id="3ca18-170">如果成功，此方法在响应`201 Created`正文中返回响应代码和[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3ca18-170">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ca18-171">示例</span><span class="sxs-lookup"><span data-stu-id="3ca18-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ca18-172">请求</span><span class="sxs-lookup"><span data-stu-id="3ca18-172">Request</span></span>
<span data-ttu-id="3ca18-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ca18-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
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

### <a name="response"></a><span data-ttu-id="3ca18-174">响应</span><span class="sxs-lookup"><span data-stu-id="3ca18-174">Response</span></span>
<span data-ttu-id="3ca18-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ca18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




