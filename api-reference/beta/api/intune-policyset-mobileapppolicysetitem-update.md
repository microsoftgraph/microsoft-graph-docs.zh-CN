---
title: 更新 mobileAppPolicySetItem
description: 更新 mobileAppPolicySetItem 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ac03bc2949b08a70b0413c372a8a522bda3975a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802151"
---
# <a name="update-mobileapppolicysetitem"></a><span data-ttu-id="d5822-103">更新 mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="d5822-103">Update mobileAppPolicySetItem</span></span>

> <span data-ttu-id="d5822-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5822-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5822-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5822-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5822-106">更新[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d5822-106">Update the properties of a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5822-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5822-107">Prerequisites</span></span>
<span data-ttu-id="d5822-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5822-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5822-110">Permission type</span></span>|<span data-ttu-id="d5822-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5822-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5822-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5822-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5822-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5822-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5822-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5822-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5822-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5822-115">Not supported.</span></span>|
|<span data-ttu-id="d5822-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5822-116">Application</span></span>|<span data-ttu-id="d5822-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5822-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5822-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5822-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d5822-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5822-119">Request headers</span></span>
|<span data-ttu-id="d5822-120">标头</span><span class="sxs-lookup"><span data-stu-id="d5822-120">Header</span></span>|<span data-ttu-id="d5822-121">值</span><span class="sxs-lookup"><span data-stu-id="d5822-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5822-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5822-122">Authorization</span></span>|<span data-ttu-id="d5822-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5822-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5822-124">接受</span><span class="sxs-lookup"><span data-stu-id="d5822-124">Accept</span></span>|<span data-ttu-id="d5822-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5822-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5822-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5822-126">Request body</span></span>
<span data-ttu-id="d5822-127">在请求正文中，提供[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5822-127">In the request body, supply a JSON representation for the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

<span data-ttu-id="d5822-128">下表显示创建[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5822-128">The following table shows the properties that are required when you create the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).</span></span>

|<span data-ttu-id="d5822-129">属性</span><span class="sxs-lookup"><span data-stu-id="d5822-129">Property</span></span>|<span data-ttu-id="d5822-130">类型</span><span class="sxs-lookup"><span data-stu-id="d5822-130">Type</span></span>|<span data-ttu-id="d5822-131">说明</span><span class="sxs-lookup"><span data-stu-id="d5822-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5822-132">id</span><span class="sxs-lookup"><span data-stu-id="d5822-132">id</span></span>|<span data-ttu-id="d5822-133">String</span><span class="sxs-lookup"><span data-stu-id="d5822-133">String</span></span>|<span data-ttu-id="d5822-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="d5822-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="d5822-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5822-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d5822-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5822-136">createdDateTime</span></span>|<span data-ttu-id="d5822-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5822-137">DateTimeOffset</span></span>|<span data-ttu-id="d5822-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="d5822-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="d5822-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5822-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d5822-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5822-140">lastModifiedDateTime</span></span>|<span data-ttu-id="d5822-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5822-141">DateTimeOffset</span></span>|<span data-ttu-id="d5822-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="d5822-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="d5822-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5822-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d5822-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="d5822-144">payloadId</span></span>|<span data-ttu-id="d5822-145">String</span><span class="sxs-lookup"><span data-stu-id="d5822-145">String</span></span>|<span data-ttu-id="d5822-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="d5822-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="d5822-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5822-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d5822-148">itemType</span><span class="sxs-lookup"><span data-stu-id="d5822-148">itemType</span></span>|<span data-ttu-id="d5822-149">String</span><span class="sxs-lookup"><span data-stu-id="d5822-149">String</span></span>|<span data-ttu-id="d5822-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="d5822-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="d5822-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5822-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d5822-152">displayName</span><span class="sxs-lookup"><span data-stu-id="d5822-152">displayName</span></span>|<span data-ttu-id="d5822-153">String</span><span class="sxs-lookup"><span data-stu-id="d5822-153">String</span></span>|<span data-ttu-id="d5822-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="d5822-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="d5822-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5822-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d5822-156">状态</span><span class="sxs-lookup"><span data-stu-id="d5822-156">status</span></span>|[<span data-ttu-id="d5822-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="d5822-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="d5822-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="d5822-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="d5822-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d5822-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d5822-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d5822-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="d5822-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="d5822-161">errorCode</span></span>|[<span data-ttu-id="d5822-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="d5822-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="d5822-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="d5822-163">Error code if any occured.</span></span> <span data-ttu-id="d5822-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d5822-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d5822-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="d5822-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="d5822-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="d5822-166">guidedDeploymentTags</span></span>|<span data-ttu-id="d5822-167">String collection</span><span class="sxs-lookup"><span data-stu-id="d5822-167">String collection</span></span>|<span data-ttu-id="d5822-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="d5822-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d5822-169">intent</span><span class="sxs-lookup"><span data-stu-id="d5822-169">intent</span></span>|[<span data-ttu-id="d5822-170">installIntent</span><span class="sxs-lookup"><span data-stu-id="d5822-170">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="d5822-171">MobileAppPolicySetItem 的安装意图。</span><span class="sxs-lookup"><span data-stu-id="d5822-171">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="d5822-172">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="d5822-172">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="d5822-173">settings</span><span class="sxs-lookup"><span data-stu-id="d5822-173">settings</span></span>|[<span data-ttu-id="d5822-174">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d5822-174">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="d5822-175">MobileAppPolicySetItem 的设置。</span><span class="sxs-lookup"><span data-stu-id="d5822-175">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="d5822-176">响应</span><span class="sxs-lookup"><span data-stu-id="d5822-176">Response</span></span>
<span data-ttu-id="d5822-177">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5822-177">If successful, this method returns a `200 OK` response code and an updated [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5822-178">示例</span><span class="sxs-lookup"><span data-stu-id="d5822-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5822-179">请求</span><span class="sxs-lookup"><span data-stu-id="d5822-179">Request</span></span>
<span data-ttu-id="d5822-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5822-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="d5822-181">响应</span><span class="sxs-lookup"><span data-stu-id="d5822-181">Response</span></span>
<span data-ttu-id="d5822-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5822-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
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
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```




