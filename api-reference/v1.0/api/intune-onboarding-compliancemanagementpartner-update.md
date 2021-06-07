---
title: 更新 complianceManagementPartner
description: 更新 complianceManagementPartner 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ee817e2c8212dc0d8fe71f661da1af4747220a1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759056"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="6227a-103">更新 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6227a-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="6227a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6227a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6227a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6227a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6227a-106">更新 [complianceManagementPartner 对象](../resources/intune-onboarding-compliancemanagementpartner.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6227a-106">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6227a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6227a-107">Prerequisites</span></span>
<span data-ttu-id="6227a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6227a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6227a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6227a-110">Permission type</span></span>|<span data-ttu-id="6227a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6227a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6227a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6227a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6227a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6227a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6227a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6227a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6227a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6227a-115">Not supported.</span></span>|
|<span data-ttu-id="6227a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6227a-116">Application</span></span>|<span data-ttu-id="6227a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6227a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6227a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6227a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="6227a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6227a-119">Request headers</span></span>
|<span data-ttu-id="6227a-120">标头</span><span class="sxs-lookup"><span data-stu-id="6227a-120">Header</span></span>|<span data-ttu-id="6227a-121">值</span><span class="sxs-lookup"><span data-stu-id="6227a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6227a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6227a-122">Authorization</span></span>|<span data-ttu-id="6227a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6227a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6227a-124">接受</span><span class="sxs-lookup"><span data-stu-id="6227a-124">Accept</span></span>|<span data-ttu-id="6227a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6227a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6227a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6227a-126">Request body</span></span>
<span data-ttu-id="6227a-127">在请求正文中，提供 [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6227a-127">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="6227a-128">下表显示创建 [complianceManagementPartner 时所需的属性](../resources/intune-onboarding-compliancemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="6227a-128">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="6227a-129">属性</span><span class="sxs-lookup"><span data-stu-id="6227a-129">Property</span></span>|<span data-ttu-id="6227a-130">类型</span><span class="sxs-lookup"><span data-stu-id="6227a-130">Type</span></span>|<span data-ttu-id="6227a-131">说明</span><span class="sxs-lookup"><span data-stu-id="6227a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6227a-132">id</span><span class="sxs-lookup"><span data-stu-id="6227a-132">id</span></span>|<span data-ttu-id="6227a-133">String</span><span class="sxs-lookup"><span data-stu-id="6227a-133">String</span></span>|<span data-ttu-id="6227a-134">实体的 ID</span><span class="sxs-lookup"><span data-stu-id="6227a-134">Id of the entity</span></span>|
|<span data-ttu-id="6227a-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="6227a-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="6227a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6227a-136">DateTimeOffset</span></span>|<span data-ttu-id="6227a-137">管理员载入合规性管理合作伙伴后最后检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="6227a-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="6227a-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="6227a-138">partnerState</span></span>|[<span data-ttu-id="6227a-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="6227a-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="6227a-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="6227a-140">Partner state of this tenant.</span></span> <span data-ttu-id="6227a-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="6227a-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="6227a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="6227a-142">displayName</span></span>|<span data-ttu-id="6227a-143">String</span><span class="sxs-lookup"><span data-stu-id="6227a-143">String</span></span>|<span data-ttu-id="6227a-144">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="6227a-144">Partner display name</span></span>|
|<span data-ttu-id="6227a-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="6227a-145">macOsOnboarded</span></span>|<span data-ttu-id="6227a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6227a-146">Boolean</span></span>|<span data-ttu-id="6227a-147">为 Mac 设备载入的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="6227a-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="6227a-148">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="6227a-148">androidOnboarded</span></span>|<span data-ttu-id="6227a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6227a-149">Boolean</span></span>|<span data-ttu-id="6227a-150">针对 Android 设备加入的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="6227a-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="6227a-151">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="6227a-151">iosOnboarded</span></span>|<span data-ttu-id="6227a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="6227a-152">Boolean</span></span>|<span data-ttu-id="6227a-153">为 ios 设备载入的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="6227a-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="6227a-154">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="6227a-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="6227a-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6227a-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="6227a-156">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="6227a-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="6227a-157">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="6227a-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="6227a-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6227a-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="6227a-159">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="6227a-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="6227a-160">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="6227a-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="6227a-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6227a-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="6227a-162">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="6227a-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="6227a-163">响应</span><span class="sxs-lookup"><span data-stu-id="6227a-163">Response</span></span>
<span data-ttu-id="6227a-164">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6227a-164">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6227a-165">示例</span><span class="sxs-lookup"><span data-stu-id="6227a-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="6227a-166">请求</span><span class="sxs-lookup"><span data-stu-id="6227a-166">Request</span></span>
<span data-ttu-id="6227a-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6227a-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 1186

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6227a-168">响应</span><span class="sxs-lookup"><span data-stu-id="6227a-168">Response</span></span>
<span data-ttu-id="6227a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6227a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1235

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




