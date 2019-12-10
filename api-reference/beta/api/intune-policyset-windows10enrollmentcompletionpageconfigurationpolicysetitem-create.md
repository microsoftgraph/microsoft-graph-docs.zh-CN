---
title: 创建 windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: 创建新的 windows10EnrollmentCompletionPageConfigurationPolicySetItem 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f00ddbdfe3995d00150ae68e394fd431d5962e6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940852"
---
# <a name="create-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="c2040-103">创建 windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="c2040-103">Create windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

> <span data-ttu-id="c2040-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2040-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2040-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2040-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2040-106">创建新的[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2040-106">Create a new [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2040-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c2040-107">Prerequisites</span></span>
<span data-ttu-id="c2040-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2040-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2040-110">Permission type</span></span>|<span data-ttu-id="c2040-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c2040-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2040-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2040-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2040-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2040-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2040-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2040-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2040-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2040-115">Not supported.</span></span>|
|<span data-ttu-id="c2040-116">Application</span><span class="sxs-lookup"><span data-stu-id="c2040-116">Application</span></span>|<span data-ttu-id="c2040-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2040-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2040-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2040-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="c2040-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2040-119">Request headers</span></span>
|<span data-ttu-id="c2040-120">标头</span><span class="sxs-lookup"><span data-stu-id="c2040-120">Header</span></span>|<span data-ttu-id="c2040-121">值</span><span class="sxs-lookup"><span data-stu-id="c2040-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2040-122">授权</span><span class="sxs-lookup"><span data-stu-id="c2040-122">Authorization</span></span>|<span data-ttu-id="c2040-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c2040-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2040-124">接受</span><span class="sxs-lookup"><span data-stu-id="c2040-124">Accept</span></span>|<span data-ttu-id="c2040-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2040-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2040-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2040-126">Request body</span></span>
<span data-ttu-id="c2040-127">在请求正文中，提供 windows10EnrollmentCompletionPageConfigurationPolicySetItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2040-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="c2040-128">下表显示创建 windows10EnrollmentCompletionPageConfigurationPolicySetItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c2040-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="c2040-129">属性</span><span class="sxs-lookup"><span data-stu-id="c2040-129">Property</span></span>|<span data-ttu-id="c2040-130">类型</span><span class="sxs-lookup"><span data-stu-id="c2040-130">Type</span></span>|<span data-ttu-id="c2040-131">说明</span><span class="sxs-lookup"><span data-stu-id="c2040-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2040-132">id</span><span class="sxs-lookup"><span data-stu-id="c2040-132">id</span></span>|<span data-ttu-id="c2040-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c2040-133">String</span></span>|<span data-ttu-id="c2040-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="c2040-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="c2040-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2040-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c2040-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2040-136">createdDateTime</span></span>|<span data-ttu-id="c2040-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2040-137">DateTimeOffset</span></span>|<span data-ttu-id="c2040-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="c2040-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="c2040-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2040-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c2040-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2040-140">lastModifiedDateTime</span></span>|<span data-ttu-id="c2040-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2040-141">DateTimeOffset</span></span>|<span data-ttu-id="c2040-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="c2040-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="c2040-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2040-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c2040-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="c2040-144">payloadId</span></span>|<span data-ttu-id="c2040-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c2040-145">String</span></span>|<span data-ttu-id="c2040-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="c2040-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="c2040-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2040-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c2040-148">itemType</span><span class="sxs-lookup"><span data-stu-id="c2040-148">itemType</span></span>|<span data-ttu-id="c2040-149">字符串</span><span class="sxs-lookup"><span data-stu-id="c2040-149">String</span></span>|<span data-ttu-id="c2040-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="c2040-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="c2040-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2040-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c2040-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c2040-152">displayName</span></span>|<span data-ttu-id="c2040-153">String</span><span class="sxs-lookup"><span data-stu-id="c2040-153">String</span></span>|<span data-ttu-id="c2040-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="c2040-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="c2040-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2040-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c2040-156">状态</span><span class="sxs-lookup"><span data-stu-id="c2040-156">status</span></span>|[<span data-ttu-id="c2040-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="c2040-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="c2040-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="c2040-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="c2040-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="c2040-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="c2040-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="c2040-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="c2040-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="c2040-161">errorCode</span></span>|[<span data-ttu-id="c2040-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="c2040-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="c2040-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="c2040-163">Error code if any occured.</span></span> <span data-ttu-id="c2040-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="c2040-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="c2040-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="c2040-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="c2040-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="c2040-166">guidedDeploymentTags</span></span>|<span data-ttu-id="c2040-167">String collection</span><span class="sxs-lookup"><span data-stu-id="c2040-167">String collection</span></span>|<span data-ttu-id="c2040-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="c2040-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c2040-169">priority</span><span class="sxs-lookup"><span data-stu-id="c2040-169">priority</span></span>|<span data-ttu-id="c2040-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c2040-170">Int32</span></span>|<span data-ttu-id="c2040-171">Windows10EnrollmentCompletionPageConfigurationPolicySetItem 的优先级。</span><span class="sxs-lookup"><span data-stu-id="c2040-171">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="c2040-172">响应</span><span class="sxs-lookup"><span data-stu-id="c2040-172">Response</span></span>
<span data-ttu-id="c2040-173">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2040-173">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2040-174">示例</span><span class="sxs-lookup"><span data-stu-id="c2040-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2040-175">请求</span><span class="sxs-lookup"><span data-stu-id="c2040-175">Request</span></span>
<span data-ttu-id="c2040-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2040-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="c2040-177">响应</span><span class="sxs-lookup"><span data-stu-id="c2040-177">Response</span></span>
<span data-ttu-id="c2040-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2040-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "id": "ebfb1dbb-1dbb-ebfb-bb1d-fbebbb1dfbeb",
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
  "priority": 8
}
```





