---
title: 更新 windowsAutopilotDeploymentProfilePolicySetItem
description: 更新 windowsAutopilotDeploymentProfilePolicySetItem 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83421291e7e932d138cf78c45bd97cef27c4ca51
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536243"
---
# <a name="update-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="17b78-103">更新 windowsAutopilotDeploymentProfilePolicySetItem</span><span class="sxs-lookup"><span data-stu-id="17b78-103">Update windowsAutopilotDeploymentProfilePolicySetItem</span></span>

> <span data-ttu-id="17b78-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17b78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17b78-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17b78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17b78-106">更新[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17b78-106">Update the properties of a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17b78-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="17b78-107">Prerequisites</span></span>
<span data-ttu-id="17b78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b78-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="17b78-110">Permission type</span></span>|<span data-ttu-id="17b78-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="17b78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17b78-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17b78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17b78-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b78-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17b78-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17b78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17b78-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="17b78-115">Not supported.</span></span>|
|<span data-ttu-id="17b78-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="17b78-116">Application</span></span>|<span data-ttu-id="17b78-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b78-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17b78-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17b78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="17b78-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="17b78-119">Request headers</span></span>
|<span data-ttu-id="17b78-120">标头</span><span class="sxs-lookup"><span data-stu-id="17b78-120">Header</span></span>|<span data-ttu-id="17b78-121">值</span><span class="sxs-lookup"><span data-stu-id="17b78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17b78-122">授权</span><span class="sxs-lookup"><span data-stu-id="17b78-122">Authorization</span></span>|<span data-ttu-id="17b78-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="17b78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17b78-124">接受</span><span class="sxs-lookup"><span data-stu-id="17b78-124">Accept</span></span>|<span data-ttu-id="17b78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17b78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b78-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="17b78-126">Request body</span></span>
<span data-ttu-id="17b78-127">在请求正文中，提供[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17b78-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

<span data-ttu-id="17b78-128">下表显示创建[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="17b78-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span></span>

|<span data-ttu-id="17b78-129">属性</span><span class="sxs-lookup"><span data-stu-id="17b78-129">Property</span></span>|<span data-ttu-id="17b78-130">类型</span><span class="sxs-lookup"><span data-stu-id="17b78-130">Type</span></span>|<span data-ttu-id="17b78-131">说明</span><span class="sxs-lookup"><span data-stu-id="17b78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17b78-132">id</span><span class="sxs-lookup"><span data-stu-id="17b78-132">id</span></span>|<span data-ttu-id="17b78-133">字符串</span><span class="sxs-lookup"><span data-stu-id="17b78-133">String</span></span>|<span data-ttu-id="17b78-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="17b78-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="17b78-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="17b78-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="17b78-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17b78-136">createdDateTime</span></span>|<span data-ttu-id="17b78-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17b78-137">DateTimeOffset</span></span>|<span data-ttu-id="17b78-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="17b78-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="17b78-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="17b78-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="17b78-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17b78-140">lastModifiedDateTime</span></span>|<span data-ttu-id="17b78-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17b78-141">DateTimeOffset</span></span>|<span data-ttu-id="17b78-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="17b78-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="17b78-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="17b78-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="17b78-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="17b78-144">payloadId</span></span>|<span data-ttu-id="17b78-145">字符串</span><span class="sxs-lookup"><span data-stu-id="17b78-145">String</span></span>|<span data-ttu-id="17b78-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="17b78-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="17b78-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="17b78-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="17b78-148">itemType</span><span class="sxs-lookup"><span data-stu-id="17b78-148">itemType</span></span>|<span data-ttu-id="17b78-149">字符串</span><span class="sxs-lookup"><span data-stu-id="17b78-149">String</span></span>|<span data-ttu-id="17b78-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="17b78-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="17b78-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="17b78-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="17b78-152">displayName</span><span class="sxs-lookup"><span data-stu-id="17b78-152">displayName</span></span>|<span data-ttu-id="17b78-153">String</span><span class="sxs-lookup"><span data-stu-id="17b78-153">String</span></span>|<span data-ttu-id="17b78-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="17b78-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="17b78-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="17b78-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="17b78-156">status</span><span class="sxs-lookup"><span data-stu-id="17b78-156">status</span></span>|[<span data-ttu-id="17b78-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="17b78-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="17b78-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="17b78-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="17b78-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="17b78-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="17b78-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="17b78-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="17b78-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="17b78-161">errorCode</span></span>|[<span data-ttu-id="17b78-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="17b78-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="17b78-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="17b78-163">Error code if any occured.</span></span> <span data-ttu-id="17b78-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="17b78-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="17b78-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="17b78-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="17b78-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="17b78-166">guidedDeploymentTags</span></span>|<span data-ttu-id="17b78-167">String 集合</span><span class="sxs-lookup"><span data-stu-id="17b78-167">String collection</span></span>|<span data-ttu-id="17b78-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="17b78-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="17b78-169">响应</span><span class="sxs-lookup"><span data-stu-id="17b78-169">Response</span></span>
<span data-ttu-id="17b78-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17b78-170">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17b78-171">示例</span><span class="sxs-lookup"><span data-stu-id="17b78-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="17b78-172">请求</span><span class="sxs-lookup"><span data-stu-id="17b78-172">Request</span></span>
<span data-ttu-id="17b78-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17b78-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 328

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
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

### <a name="response"></a><span data-ttu-id="17b78-174">响应</span><span class="sxs-lookup"><span data-stu-id="17b78-174">Response</span></span>
<span data-ttu-id="17b78-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17b78-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "id": "850e84d8-84d8-850e-d884-0e85d8840e85",
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






