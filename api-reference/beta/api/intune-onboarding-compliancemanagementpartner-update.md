---
title: 更新 complianceManagementPartner
description: 更新 complianceManagementPartner 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8cfa6c03236e7c75713eeb4c7c915a21fbef789
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135150"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="d3cf4-103">更新 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="d3cf4-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="d3cf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3cf4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3cf4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3cf4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3cf4-107">更新 [complianceManagementPartner 对象](../resources/intune-onboarding-compliancemanagementpartner.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-107">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3cf4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3cf4-108">Prerequisites</span></span>
<span data-ttu-id="d3cf4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3cf4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3cf4-111">Permission type</span></span>|<span data-ttu-id="d3cf4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3cf4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3cf4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3cf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3cf4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cf4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d3cf4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3cf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3cf4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-116">Not supported.</span></span>|
|<span data-ttu-id="d3cf4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3cf4-117">Application</span></span>|<span data-ttu-id="d3cf4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cf4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3cf4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3cf4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="d3cf4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3cf4-120">Request headers</span></span>
|<span data-ttu-id="d3cf4-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3cf4-121">Header</span></span>|<span data-ttu-id="d3cf4-122">值</span><span class="sxs-lookup"><span data-stu-id="d3cf4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3cf4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3cf4-123">Authorization</span></span>|<span data-ttu-id="d3cf4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3cf4-125">接受</span><span class="sxs-lookup"><span data-stu-id="d3cf4-125">Accept</span></span>|<span data-ttu-id="d3cf4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3cf4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3cf4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3cf4-127">Request body</span></span>
<span data-ttu-id="d3cf4-128">在请求正文中，提供 [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-128">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="d3cf4-129">下表显示创建 [complianceManagementPartner 时所需的属性](../resources/intune-onboarding-compliancemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-129">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="d3cf4-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3cf4-130">Property</span></span>|<span data-ttu-id="d3cf4-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3cf4-131">Type</span></span>|<span data-ttu-id="d3cf4-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3cf4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3cf4-133">id</span><span class="sxs-lookup"><span data-stu-id="d3cf4-133">id</span></span>|<span data-ttu-id="d3cf4-134">String</span><span class="sxs-lookup"><span data-stu-id="d3cf4-134">String</span></span>|<span data-ttu-id="d3cf4-135">实体的 ID</span><span class="sxs-lookup"><span data-stu-id="d3cf4-135">Id of the entity</span></span>|
|<span data-ttu-id="d3cf4-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="d3cf4-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="d3cf4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3cf4-137">DateTimeOffset</span></span>|<span data-ttu-id="d3cf4-138">管理员载入合规性管理合作伙伴后最后检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="d3cf4-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="d3cf4-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="d3cf4-139">partnerState</span></span>|[<span data-ttu-id="d3cf4-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="d3cf4-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="d3cf4-141">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-141">Partner state of this tenant.</span></span> <span data-ttu-id="d3cf4-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="d3cf4-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d3cf4-143">displayName</span></span>|<span data-ttu-id="d3cf4-144">String</span><span class="sxs-lookup"><span data-stu-id="d3cf4-144">String</span></span>|<span data-ttu-id="d3cf4-145">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="d3cf4-145">Partner display name</span></span>|
|<span data-ttu-id="d3cf4-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="d3cf4-146">macOsOnboarded</span></span>|<span data-ttu-id="d3cf4-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3cf4-147">Boolean</span></span>|<span data-ttu-id="d3cf4-148">为 Mac 设备载入的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="d3cf4-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="d3cf4-149">windowsOnboarded</span></span>|<span data-ttu-id="d3cf4-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3cf4-150">Boolean</span></span>|<span data-ttu-id="d3cf4-151">为 Windows 设备载入的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="d3cf4-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="d3cf4-152">androidOnboarded</span></span>|<span data-ttu-id="d3cf4-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3cf4-153">Boolean</span></span>|<span data-ttu-id="d3cf4-154">针对 Android 设备加入的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="d3cf4-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="d3cf4-155">iosOnboarded</span></span>|<span data-ttu-id="d3cf4-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3cf4-156">Boolean</span></span>|<span data-ttu-id="d3cf4-157">为 ios 设备载入的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="d3cf4-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="d3cf4-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="d3cf4-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3cf4-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d3cf4-160">通过合作伙伴注册 Mac 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="d3cf4-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="d3cf4-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="d3cf4-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3cf4-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d3cf4-163">通过合作伙伴注册 Windows 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="d3cf4-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="d3cf4-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="d3cf4-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3cf4-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d3cf4-166">通过合作伙伴注册 Android 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="d3cf4-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="d3cf4-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="d3cf4-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3cf4-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d3cf4-169">通过合作伙伴注册 ios 设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="d3cf4-170">响应</span><span class="sxs-lookup"><span data-stu-id="d3cf4-170">Response</span></span>
<span data-ttu-id="d3cf4-171">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-171">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3cf4-172">示例</span><span class="sxs-lookup"><span data-stu-id="d3cf4-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3cf4-173">请求</span><span class="sxs-lookup"><span data-stu-id="d3cf4-173">Request</span></span>
<span data-ttu-id="d3cf4-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 2216

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
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

### <a name="response"></a><span data-ttu-id="d3cf4-175">响应</span><span class="sxs-lookup"><span data-stu-id="d3cf4-175">Response</span></span>
<span data-ttu-id="d3cf4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3cf4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2265

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
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




