---
title: 更新 managedAppProtectionPolicySetItem
description: 更新 managedAppProtectionPolicySetItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6402bf4ce476ec0276bb057ff3eb0624dde32faa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49305118"
---
# <a name="update-managedappprotectionpolicysetitem"></a><span data-ttu-id="abc6e-103">更新 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="abc6e-103">Update managedAppProtectionPolicySetItem</span></span>

<span data-ttu-id="abc6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abc6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abc6e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="abc6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abc6e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="abc6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abc6e-107">更新 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="abc6e-107">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abc6e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="abc6e-108">Prerequisites</span></span>
<span data-ttu-id="abc6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abc6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abc6e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="abc6e-111">Permission type</span></span>|<span data-ttu-id="abc6e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="abc6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abc6e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abc6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abc6e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abc6e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abc6e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abc6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abc6e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="abc6e-116">Not supported.</span></span>|
|<span data-ttu-id="abc6e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="abc6e-117">Application</span></span>|<span data-ttu-id="abc6e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abc6e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abc6e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abc6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="abc6e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="abc6e-120">Request headers</span></span>
|<span data-ttu-id="abc6e-121">标头</span><span class="sxs-lookup"><span data-stu-id="abc6e-121">Header</span></span>|<span data-ttu-id="abc6e-122">值</span><span class="sxs-lookup"><span data-stu-id="abc6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abc6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="abc6e-123">Authorization</span></span>|<span data-ttu-id="abc6e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="abc6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abc6e-125">接受</span><span class="sxs-lookup"><span data-stu-id="abc6e-125">Accept</span></span>|<span data-ttu-id="abc6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abc6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abc6e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="abc6e-127">Request body</span></span>
<span data-ttu-id="abc6e-128">在请求正文中，提供 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abc6e-128">In the request body, supply a JSON representation for the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

<span data-ttu-id="abc6e-129">下表显示创建 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="abc6e-129">The following table shows the properties that are required when you create the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>

|<span data-ttu-id="abc6e-130">属性</span><span class="sxs-lookup"><span data-stu-id="abc6e-130">Property</span></span>|<span data-ttu-id="abc6e-131">类型</span><span class="sxs-lookup"><span data-stu-id="abc6e-131">Type</span></span>|<span data-ttu-id="abc6e-132">说明</span><span class="sxs-lookup"><span data-stu-id="abc6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abc6e-133">id</span><span class="sxs-lookup"><span data-stu-id="abc6e-133">id</span></span>|<span data-ttu-id="abc6e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="abc6e-134">String</span></span>|<span data-ttu-id="abc6e-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="abc6e-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="abc6e-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abc6e-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abc6e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abc6e-137">createdDateTime</span></span>|<span data-ttu-id="abc6e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abc6e-138">DateTimeOffset</span></span>|<span data-ttu-id="abc6e-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="abc6e-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="abc6e-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abc6e-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abc6e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abc6e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="abc6e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abc6e-142">DateTimeOffset</span></span>|<span data-ttu-id="abc6e-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="abc6e-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="abc6e-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abc6e-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abc6e-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="abc6e-145">payloadId</span></span>|<span data-ttu-id="abc6e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="abc6e-146">String</span></span>|<span data-ttu-id="abc6e-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="abc6e-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="abc6e-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abc6e-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abc6e-149">itemType</span><span class="sxs-lookup"><span data-stu-id="abc6e-149">itemType</span></span>|<span data-ttu-id="abc6e-150">字符串</span><span class="sxs-lookup"><span data-stu-id="abc6e-150">String</span></span>|<span data-ttu-id="abc6e-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="abc6e-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="abc6e-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abc6e-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abc6e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="abc6e-153">displayName</span></span>|<span data-ttu-id="abc6e-154">字符串</span><span class="sxs-lookup"><span data-stu-id="abc6e-154">String</span></span>|<span data-ttu-id="abc6e-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="abc6e-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="abc6e-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="abc6e-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abc6e-157">status</span><span class="sxs-lookup"><span data-stu-id="abc6e-157">status</span></span>|[<span data-ttu-id="abc6e-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="abc6e-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="abc6e-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="abc6e-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="abc6e-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="abc6e-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="abc6e-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="abc6e-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="abc6e-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="abc6e-162">errorCode</span></span>|[<span data-ttu-id="abc6e-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="abc6e-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="abc6e-164">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="abc6e-164">Error code if any occured.</span></span> <span data-ttu-id="abc6e-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="abc6e-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="abc6e-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="abc6e-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="abc6e-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="abc6e-167">guidedDeploymentTags</span></span>|<span data-ttu-id="abc6e-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="abc6e-168">String collection</span></span>|<span data-ttu-id="abc6e-169">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="abc6e-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="abc6e-170">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="abc6e-170">targetedAppManagementLevels</span></span>|<span data-ttu-id="abc6e-171">字符串</span><span class="sxs-lookup"><span data-stu-id="abc6e-171">String</span></span>|<span data-ttu-id="abc6e-172">ManagedAppPolicySetItem 的 TargetedAppManagementLevels。</span><span class="sxs-lookup"><span data-stu-id="abc6e-172">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="abc6e-173">响应</span><span class="sxs-lookup"><span data-stu-id="abc6e-173">Response</span></span>
<span data-ttu-id="abc6e-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abc6e-174">If successful, this method returns a `200 OK` response code and an updated [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abc6e-175">示例</span><span class="sxs-lookup"><span data-stu-id="abc6e-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="abc6e-176">请求</span><span class="sxs-lookup"><span data-stu-id="abc6e-176">Request</span></span>
<span data-ttu-id="abc6e-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="abc6e-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```

### <a name="response"></a><span data-ttu-id="abc6e-178">响应</span><span class="sxs-lookup"><span data-stu-id="abc6e-178">Response</span></span>
<span data-ttu-id="abc6e-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="abc6e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 561

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "id": "e10d79c9-79c9-e10d-c979-0de1c9790de1",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```




