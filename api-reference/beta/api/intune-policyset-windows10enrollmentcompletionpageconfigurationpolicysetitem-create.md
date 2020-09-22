---
title: 创建 windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: 创建新的 windows10EnrollmentCompletionPageConfigurationPolicySetItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 078a1d677a7ccaa29877c0a8a83ba1792e1ebd77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972047"
---
# <a name="create-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="89bed-103">创建 windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="89bed-103">Create windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

<span data-ttu-id="89bed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89bed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89bed-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89bed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89bed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89bed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89bed-107">创建新的 [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89bed-107">Create a new [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89bed-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="89bed-108">Prerequisites</span></span>
<span data-ttu-id="89bed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89bed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89bed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89bed-111">Permission type</span></span>|<span data-ttu-id="89bed-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89bed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89bed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89bed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89bed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89bed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89bed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89bed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89bed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89bed-116">Not supported.</span></span>|
|<span data-ttu-id="89bed-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89bed-117">Application</span></span>|<span data-ttu-id="89bed-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89bed-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89bed-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89bed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="89bed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89bed-120">Request headers</span></span>
|<span data-ttu-id="89bed-121">标头</span><span class="sxs-lookup"><span data-stu-id="89bed-121">Header</span></span>|<span data-ttu-id="89bed-122">值</span><span class="sxs-lookup"><span data-stu-id="89bed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89bed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89bed-123">Authorization</span></span>|<span data-ttu-id="89bed-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89bed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89bed-125">接受</span><span class="sxs-lookup"><span data-stu-id="89bed-125">Accept</span></span>|<span data-ttu-id="89bed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89bed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89bed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89bed-127">Request body</span></span>
<span data-ttu-id="89bed-128">在请求正文中，提供 windows10EnrollmentCompletionPageConfigurationPolicySetItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89bed-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="89bed-129">下表显示创建 windows10EnrollmentCompletionPageConfigurationPolicySetItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89bed-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="89bed-130">属性</span><span class="sxs-lookup"><span data-stu-id="89bed-130">Property</span></span>|<span data-ttu-id="89bed-131">类型</span><span class="sxs-lookup"><span data-stu-id="89bed-131">Type</span></span>|<span data-ttu-id="89bed-132">说明</span><span class="sxs-lookup"><span data-stu-id="89bed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89bed-133">id</span><span class="sxs-lookup"><span data-stu-id="89bed-133">id</span></span>|<span data-ttu-id="89bed-134">String</span><span class="sxs-lookup"><span data-stu-id="89bed-134">String</span></span>|<span data-ttu-id="89bed-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="89bed-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="89bed-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="89bed-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="89bed-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89bed-137">createdDateTime</span></span>|<span data-ttu-id="89bed-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89bed-138">DateTimeOffset</span></span>|<span data-ttu-id="89bed-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="89bed-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="89bed-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="89bed-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="89bed-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89bed-141">lastModifiedDateTime</span></span>|<span data-ttu-id="89bed-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89bed-142">DateTimeOffset</span></span>|<span data-ttu-id="89bed-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="89bed-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="89bed-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="89bed-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="89bed-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="89bed-145">payloadId</span></span>|<span data-ttu-id="89bed-146">String</span><span class="sxs-lookup"><span data-stu-id="89bed-146">String</span></span>|<span data-ttu-id="89bed-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="89bed-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="89bed-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="89bed-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="89bed-149">itemType</span><span class="sxs-lookup"><span data-stu-id="89bed-149">itemType</span></span>|<span data-ttu-id="89bed-150">String</span><span class="sxs-lookup"><span data-stu-id="89bed-150">String</span></span>|<span data-ttu-id="89bed-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="89bed-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="89bed-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="89bed-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="89bed-153">displayName</span><span class="sxs-lookup"><span data-stu-id="89bed-153">displayName</span></span>|<span data-ttu-id="89bed-154">String</span><span class="sxs-lookup"><span data-stu-id="89bed-154">String</span></span>|<span data-ttu-id="89bed-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="89bed-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="89bed-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="89bed-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="89bed-157">状态</span><span class="sxs-lookup"><span data-stu-id="89bed-157">status</span></span>|[<span data-ttu-id="89bed-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="89bed-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="89bed-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="89bed-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="89bed-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="89bed-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="89bed-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="89bed-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="89bed-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="89bed-162">errorCode</span></span>|[<span data-ttu-id="89bed-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="89bed-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="89bed-164">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="89bed-164">Error code if any occured.</span></span> <span data-ttu-id="89bed-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="89bed-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="89bed-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="89bed-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="89bed-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="89bed-167">guidedDeploymentTags</span></span>|<span data-ttu-id="89bed-168">String collection</span><span class="sxs-lookup"><span data-stu-id="89bed-168">String collection</span></span>|<span data-ttu-id="89bed-169">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="89bed-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="89bed-170">priority</span><span class="sxs-lookup"><span data-stu-id="89bed-170">priority</span></span>|<span data-ttu-id="89bed-171">Int32</span><span class="sxs-lookup"><span data-stu-id="89bed-171">Int32</span></span>|<span data-ttu-id="89bed-172">Windows10EnrollmentCompletionPageConfigurationPolicySetItem 的优先级。</span><span class="sxs-lookup"><span data-stu-id="89bed-172">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="89bed-173">响应</span><span class="sxs-lookup"><span data-stu-id="89bed-173">Response</span></span>
<span data-ttu-id="89bed-174">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89bed-174">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89bed-175">示例</span><span class="sxs-lookup"><span data-stu-id="89bed-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="89bed-176">请求</span><span class="sxs-lookup"><span data-stu-id="89bed-176">Request</span></span>
<span data-ttu-id="89bed-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89bed-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89bed-178">响应</span><span class="sxs-lookup"><span data-stu-id="89bed-178">Response</span></span>
<span data-ttu-id="89bed-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89bed-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






