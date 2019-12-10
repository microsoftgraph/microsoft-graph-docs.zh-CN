---
title: 更新 enrollmentRestrictionsConfigurationPolicySetItem
description: 更新 enrollmentRestrictionsConfigurationPolicySetItem 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8fdb6a42022fc00173273b04cbbd0b2506273a6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941160"
---
# <a name="update-enrollmentrestrictionsconfigurationpolicysetitem"></a><span data-ttu-id="21321-103">更新 enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="21321-103">Update enrollmentRestrictionsConfigurationPolicySetItem</span></span>

> <span data-ttu-id="21321-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21321-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21321-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21321-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21321-106">更新[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="21321-106">Update the properties of a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21321-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="21321-107">Prerequisites</span></span>
<span data-ttu-id="21321-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21321-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21321-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="21321-110">Permission type</span></span>|<span data-ttu-id="21321-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="21321-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21321-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21321-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21321-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21321-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21321-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21321-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21321-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="21321-115">Not supported.</span></span>|
|<span data-ttu-id="21321-116">Application</span><span class="sxs-lookup"><span data-stu-id="21321-116">Application</span></span>|<span data-ttu-id="21321-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21321-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21321-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21321-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="21321-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="21321-119">Request headers</span></span>
|<span data-ttu-id="21321-120">标头</span><span class="sxs-lookup"><span data-stu-id="21321-120">Header</span></span>|<span data-ttu-id="21321-121">值</span><span class="sxs-lookup"><span data-stu-id="21321-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21321-122">授权</span><span class="sxs-lookup"><span data-stu-id="21321-122">Authorization</span></span>|<span data-ttu-id="21321-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21321-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21321-124">接受</span><span class="sxs-lookup"><span data-stu-id="21321-124">Accept</span></span>|<span data-ttu-id="21321-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21321-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21321-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="21321-126">Request body</span></span>
<span data-ttu-id="21321-127">在请求正文中，提供[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21321-127">In the request body, supply a JSON representation for the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="21321-128">下表显示创建[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="21321-128">The following table shows the properties that are required when you create the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="21321-129">属性</span><span class="sxs-lookup"><span data-stu-id="21321-129">Property</span></span>|<span data-ttu-id="21321-130">类型</span><span class="sxs-lookup"><span data-stu-id="21321-130">Type</span></span>|<span data-ttu-id="21321-131">说明</span><span class="sxs-lookup"><span data-stu-id="21321-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21321-132">id</span><span class="sxs-lookup"><span data-stu-id="21321-132">id</span></span>|<span data-ttu-id="21321-133">字符串</span><span class="sxs-lookup"><span data-stu-id="21321-133">String</span></span>|<span data-ttu-id="21321-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="21321-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="21321-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="21321-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="21321-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21321-136">createdDateTime</span></span>|<span data-ttu-id="21321-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21321-137">DateTimeOffset</span></span>|<span data-ttu-id="21321-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="21321-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="21321-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="21321-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="21321-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21321-140">lastModifiedDateTime</span></span>|<span data-ttu-id="21321-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21321-141">DateTimeOffset</span></span>|<span data-ttu-id="21321-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="21321-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="21321-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="21321-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="21321-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="21321-144">payloadId</span></span>|<span data-ttu-id="21321-145">字符串</span><span class="sxs-lookup"><span data-stu-id="21321-145">String</span></span>|<span data-ttu-id="21321-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="21321-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="21321-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="21321-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="21321-148">itemType</span><span class="sxs-lookup"><span data-stu-id="21321-148">itemType</span></span>|<span data-ttu-id="21321-149">字符串</span><span class="sxs-lookup"><span data-stu-id="21321-149">String</span></span>|<span data-ttu-id="21321-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="21321-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="21321-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="21321-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="21321-152">displayName</span><span class="sxs-lookup"><span data-stu-id="21321-152">displayName</span></span>|<span data-ttu-id="21321-153">String</span><span class="sxs-lookup"><span data-stu-id="21321-153">String</span></span>|<span data-ttu-id="21321-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="21321-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="21321-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="21321-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="21321-156">状态</span><span class="sxs-lookup"><span data-stu-id="21321-156">status</span></span>|[<span data-ttu-id="21321-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="21321-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="21321-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="21321-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="21321-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="21321-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="21321-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="21321-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="21321-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="21321-161">errorCode</span></span>|[<span data-ttu-id="21321-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="21321-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="21321-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="21321-163">Error code if any occured.</span></span> <span data-ttu-id="21321-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="21321-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="21321-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="21321-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="21321-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="21321-166">guidedDeploymentTags</span></span>|<span data-ttu-id="21321-167">String collection</span><span class="sxs-lookup"><span data-stu-id="21321-167">String collection</span></span>|<span data-ttu-id="21321-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="21321-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="21321-169">priority</span><span class="sxs-lookup"><span data-stu-id="21321-169">priority</span></span>|<span data-ttu-id="21321-170">Int32</span><span class="sxs-lookup"><span data-stu-id="21321-170">Int32</span></span>|<span data-ttu-id="21321-171">EnrollmentRestrictionsConfigurationPolicySetItem 的优先级。</span><span class="sxs-lookup"><span data-stu-id="21321-171">Priority of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|
|<span data-ttu-id="21321-172">limit</span><span class="sxs-lookup"><span data-stu-id="21321-172">limit</span></span>|<span data-ttu-id="21321-173">Int32</span><span class="sxs-lookup"><span data-stu-id="21321-173">Int32</span></span>|<span data-ttu-id="21321-174">EnrollmentRestrictionsConfigurationPolicySetItem 的限制。</span><span class="sxs-lookup"><span data-stu-id="21321-174">Limit of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="21321-175">响应</span><span class="sxs-lookup"><span data-stu-id="21321-175">Response</span></span>
<span data-ttu-id="21321-176">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="21321-176">If successful, this method returns a `200 OK` response code and an updated [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21321-177">示例</span><span class="sxs-lookup"><span data-stu-id="21321-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="21321-178">请求</span><span class="sxs-lookup"><span data-stu-id="21321-178">Request</span></span>
<span data-ttu-id="21321-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21321-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="21321-180">响应</span><span class="sxs-lookup"><span data-stu-id="21321-180">Response</span></span>
<span data-ttu-id="21321-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21321-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
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
  "priority": 8,
  "limit": 5
}
```





