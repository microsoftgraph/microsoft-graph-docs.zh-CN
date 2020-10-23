---
title: 更新 windowsAutopilotDeploymentProfilePolicySetItem
description: 更新 windowsAutopilotDeploymentProfilePolicySetItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17f4932dec341b3b8165a46ecdaad3132686fa3d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690859"
---
# <a name="update-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="174a5-103">更新 windowsAutopilotDeploymentProfilePolicySetItem</span><span class="sxs-lookup"><span data-stu-id="174a5-103">Update windowsAutopilotDeploymentProfilePolicySetItem</span></span>

<span data-ttu-id="174a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="174a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="174a5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="174a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="174a5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="174a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="174a5-107">更新 [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="174a5-107">Update the properties of a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="174a5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="174a5-108">Prerequisites</span></span>
<span data-ttu-id="174a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="174a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="174a5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="174a5-111">Permission type</span></span>|<span data-ttu-id="174a5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="174a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="174a5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="174a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="174a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="174a5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="174a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="174a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="174a5-116">Not supported.</span></span>|
|<span data-ttu-id="174a5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="174a5-117">Application</span></span>|<span data-ttu-id="174a5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174a5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="174a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="174a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="174a5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="174a5-120">Request headers</span></span>
|<span data-ttu-id="174a5-121">标头</span><span class="sxs-lookup"><span data-stu-id="174a5-121">Header</span></span>|<span data-ttu-id="174a5-122">值</span><span class="sxs-lookup"><span data-stu-id="174a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="174a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="174a5-123">Authorization</span></span>|<span data-ttu-id="174a5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="174a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="174a5-125">接受</span><span class="sxs-lookup"><span data-stu-id="174a5-125">Accept</span></span>|<span data-ttu-id="174a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="174a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="174a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="174a5-127">Request body</span></span>
<span data-ttu-id="174a5-128">在请求正文中，提供 [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="174a5-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

<span data-ttu-id="174a5-129">下表显示创建 [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="174a5-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span></span>

|<span data-ttu-id="174a5-130">属性</span><span class="sxs-lookup"><span data-stu-id="174a5-130">Property</span></span>|<span data-ttu-id="174a5-131">类型</span><span class="sxs-lookup"><span data-stu-id="174a5-131">Type</span></span>|<span data-ttu-id="174a5-132">说明</span><span class="sxs-lookup"><span data-stu-id="174a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="174a5-133">id</span><span class="sxs-lookup"><span data-stu-id="174a5-133">id</span></span>|<span data-ttu-id="174a5-134">String</span><span class="sxs-lookup"><span data-stu-id="174a5-134">String</span></span>|<span data-ttu-id="174a5-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="174a5-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="174a5-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="174a5-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="174a5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="174a5-137">createdDateTime</span></span>|<span data-ttu-id="174a5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="174a5-138">DateTimeOffset</span></span>|<span data-ttu-id="174a5-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="174a5-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="174a5-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="174a5-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="174a5-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="174a5-141">lastModifiedDateTime</span></span>|<span data-ttu-id="174a5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="174a5-142">DateTimeOffset</span></span>|<span data-ttu-id="174a5-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="174a5-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="174a5-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="174a5-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="174a5-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="174a5-145">payloadId</span></span>|<span data-ttu-id="174a5-146">String</span><span class="sxs-lookup"><span data-stu-id="174a5-146">String</span></span>|<span data-ttu-id="174a5-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="174a5-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="174a5-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="174a5-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="174a5-149">itemType</span><span class="sxs-lookup"><span data-stu-id="174a5-149">itemType</span></span>|<span data-ttu-id="174a5-150">String</span><span class="sxs-lookup"><span data-stu-id="174a5-150">String</span></span>|<span data-ttu-id="174a5-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="174a5-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="174a5-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="174a5-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="174a5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="174a5-153">displayName</span></span>|<span data-ttu-id="174a5-154">String</span><span class="sxs-lookup"><span data-stu-id="174a5-154">String</span></span>|<span data-ttu-id="174a5-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="174a5-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="174a5-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="174a5-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="174a5-157">status</span><span class="sxs-lookup"><span data-stu-id="174a5-157">status</span></span>|[<span data-ttu-id="174a5-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="174a5-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="174a5-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="174a5-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="174a5-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="174a5-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="174a5-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="174a5-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="174a5-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="174a5-162">errorCode</span></span>|[<span data-ttu-id="174a5-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="174a5-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="174a5-164">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="174a5-164">Error code if any occured.</span></span> <span data-ttu-id="174a5-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="174a5-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="174a5-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="174a5-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="174a5-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="174a5-167">guidedDeploymentTags</span></span>|<span data-ttu-id="174a5-168">String collection</span><span class="sxs-lookup"><span data-stu-id="174a5-168">String collection</span></span>|<span data-ttu-id="174a5-169">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="174a5-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="174a5-170">响应</span><span class="sxs-lookup"><span data-stu-id="174a5-170">Response</span></span>
<span data-ttu-id="174a5-171">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="174a5-171">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="174a5-172">示例</span><span class="sxs-lookup"><span data-stu-id="174a5-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="174a5-173">请求</span><span class="sxs-lookup"><span data-stu-id="174a5-173">Request</span></span>
<span data-ttu-id="174a5-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="174a5-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="174a5-175">响应</span><span class="sxs-lookup"><span data-stu-id="174a5-175">Response</span></span>
<span data-ttu-id="174a5-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="174a5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





