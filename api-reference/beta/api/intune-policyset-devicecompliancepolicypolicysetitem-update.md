---
title: 更新 deviceCompliancePolicyPolicySetItem
description: 更新 deviceCompliancePolicyPolicySetItem 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20145f98d06b631e78b4fe51d347c10e54e0de15
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802431"
---
# <a name="update-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="b5788-103">更新 deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="b5788-103">Update deviceCompliancePolicyPolicySetItem</span></span>

> <span data-ttu-id="b5788-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5788-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5788-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5788-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5788-106">更新[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5788-106">Update the properties of a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5788-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5788-107">Prerequisites</span></span>
<span data-ttu-id="b5788-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5788-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5788-110">Permission type</span></span>|<span data-ttu-id="b5788-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5788-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5788-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5788-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5788-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5788-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5788-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5788-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5788-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5788-115">Not supported.</span></span>|
|<span data-ttu-id="b5788-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5788-116">Application</span></span>|<span data-ttu-id="b5788-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5788-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5788-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5788-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="b5788-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5788-119">Request headers</span></span>
|<span data-ttu-id="b5788-120">标头</span><span class="sxs-lookup"><span data-stu-id="b5788-120">Header</span></span>|<span data-ttu-id="b5788-121">值</span><span class="sxs-lookup"><span data-stu-id="b5788-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5788-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5788-122">Authorization</span></span>|<span data-ttu-id="b5788-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5788-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5788-124">接受</span><span class="sxs-lookup"><span data-stu-id="b5788-124">Accept</span></span>|<span data-ttu-id="b5788-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5788-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5788-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5788-126">Request body</span></span>
<span data-ttu-id="b5788-127">在请求正文中，提供[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5788-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

<span data-ttu-id="b5788-128">下表显示创建[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5788-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).</span></span>

|<span data-ttu-id="b5788-129">属性</span><span class="sxs-lookup"><span data-stu-id="b5788-129">Property</span></span>|<span data-ttu-id="b5788-130">类型</span><span class="sxs-lookup"><span data-stu-id="b5788-130">Type</span></span>|<span data-ttu-id="b5788-131">说明</span><span class="sxs-lookup"><span data-stu-id="b5788-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5788-132">id</span><span class="sxs-lookup"><span data-stu-id="b5788-132">id</span></span>|<span data-ttu-id="b5788-133">String</span><span class="sxs-lookup"><span data-stu-id="b5788-133">String</span></span>|<span data-ttu-id="b5788-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="b5788-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b5788-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5788-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b5788-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5788-136">createdDateTime</span></span>|<span data-ttu-id="b5788-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5788-137">DateTimeOffset</span></span>|<span data-ttu-id="b5788-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="b5788-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="b5788-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5788-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b5788-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5788-140">lastModifiedDateTime</span></span>|<span data-ttu-id="b5788-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5788-141">DateTimeOffset</span></span>|<span data-ttu-id="b5788-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b5788-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="b5788-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5788-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b5788-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="b5788-144">payloadId</span></span>|<span data-ttu-id="b5788-145">String</span><span class="sxs-lookup"><span data-stu-id="b5788-145">String</span></span>|<span data-ttu-id="b5788-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="b5788-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="b5788-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5788-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b5788-148">itemType</span><span class="sxs-lookup"><span data-stu-id="b5788-148">itemType</span></span>|<span data-ttu-id="b5788-149">String</span><span class="sxs-lookup"><span data-stu-id="b5788-149">String</span></span>|<span data-ttu-id="b5788-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="b5788-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="b5788-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5788-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b5788-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b5788-152">displayName</span></span>|<span data-ttu-id="b5788-153">String</span><span class="sxs-lookup"><span data-stu-id="b5788-153">String</span></span>|<span data-ttu-id="b5788-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="b5788-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="b5788-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5788-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b5788-156">状态</span><span class="sxs-lookup"><span data-stu-id="b5788-156">status</span></span>|[<span data-ttu-id="b5788-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b5788-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b5788-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="b5788-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="b5788-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b5788-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b5788-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b5788-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b5788-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="b5788-161">errorCode</span></span>|[<span data-ttu-id="b5788-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="b5788-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b5788-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="b5788-163">Error code if any occured.</span></span> <span data-ttu-id="b5788-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b5788-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b5788-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="b5788-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b5788-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b5788-166">guidedDeploymentTags</span></span>|<span data-ttu-id="b5788-167">String collection</span><span class="sxs-lookup"><span data-stu-id="b5788-167">String collection</span></span>|<span data-ttu-id="b5788-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="b5788-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b5788-169">响应</span><span class="sxs-lookup"><span data-stu-id="b5788-169">Response</span></span>
<span data-ttu-id="b5788-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5788-170">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5788-171">示例</span><span class="sxs-lookup"><span data-stu-id="b5788-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5788-172">请求</span><span class="sxs-lookup"><span data-stu-id="b5788-172">Request</span></span>
<span data-ttu-id="b5788-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5788-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b5788-174">响应</span><span class="sxs-lookup"><span data-stu-id="b5788-174">Response</span></span>
<span data-ttu-id="b5788-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5788-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
  "id": "5c0bc827-c827-5c0b-27c8-0b5c27c80b5c",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```




