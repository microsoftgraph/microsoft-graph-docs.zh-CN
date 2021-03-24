---
title: 创建 deviceCompliancePolicyPolicySetItem
description: 创建新的 deviceCompliancePolicyPolicySetItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b15ab0f6116a82ca5b9414e40c8fa97dd4e146c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125175"
---
# <a name="create-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="3c463-103">创建 deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="3c463-103">Create deviceCompliancePolicyPolicySetItem</span></span>

<span data-ttu-id="3c463-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c463-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c463-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c463-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c463-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c463-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c463-107">创建新的 [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c463-107">Create a new [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c463-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c463-108">Prerequisites</span></span>
<span data-ttu-id="3c463-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c463-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c463-111">Permission type</span></span>|<span data-ttu-id="3c463-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c463-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c463-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c463-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c463-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c463-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c463-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c463-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c463-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c463-116">Not supported.</span></span>|
|<span data-ttu-id="3c463-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c463-117">Application</span></span>|<span data-ttu-id="3c463-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c463-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c463-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c463-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="3c463-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c463-120">Request headers</span></span>
|<span data-ttu-id="3c463-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c463-121">Header</span></span>|<span data-ttu-id="3c463-122">值</span><span class="sxs-lookup"><span data-stu-id="3c463-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c463-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c463-123">Authorization</span></span>|<span data-ttu-id="3c463-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c463-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c463-125">接受</span><span class="sxs-lookup"><span data-stu-id="3c463-125">Accept</span></span>|<span data-ttu-id="3c463-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c463-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c463-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c463-127">Request body</span></span>
<span data-ttu-id="3c463-128">在请求正文中，提供 deviceCompliancePolicyPolicySetItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c463-128">In the request body, supply a JSON representation for the deviceCompliancePolicyPolicySetItem object.</span></span>

<span data-ttu-id="3c463-129">下表显示创建 deviceCompliancePolicyPolicySetItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c463-129">The following table shows the properties that are required when you create the deviceCompliancePolicyPolicySetItem.</span></span>

|<span data-ttu-id="3c463-130">属性</span><span class="sxs-lookup"><span data-stu-id="3c463-130">Property</span></span>|<span data-ttu-id="3c463-131">类型</span><span class="sxs-lookup"><span data-stu-id="3c463-131">Type</span></span>|<span data-ttu-id="3c463-132">说明</span><span class="sxs-lookup"><span data-stu-id="3c463-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c463-133">id</span><span class="sxs-lookup"><span data-stu-id="3c463-133">id</span></span>|<span data-ttu-id="3c463-134">String</span><span class="sxs-lookup"><span data-stu-id="3c463-134">String</span></span>|<span data-ttu-id="3c463-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="3c463-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="3c463-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c463-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3c463-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c463-137">createdDateTime</span></span>|<span data-ttu-id="3c463-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c463-138">DateTimeOffset</span></span>|<span data-ttu-id="3c463-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="3c463-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="3c463-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c463-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3c463-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c463-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3c463-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c463-142">DateTimeOffset</span></span>|<span data-ttu-id="3c463-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="3c463-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="3c463-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c463-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3c463-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="3c463-145">payloadId</span></span>|<span data-ttu-id="3c463-146">String</span><span class="sxs-lookup"><span data-stu-id="3c463-146">String</span></span>|<span data-ttu-id="3c463-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="3c463-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="3c463-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c463-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3c463-149">itemType</span><span class="sxs-lookup"><span data-stu-id="3c463-149">itemType</span></span>|<span data-ttu-id="3c463-150">String</span><span class="sxs-lookup"><span data-stu-id="3c463-150">String</span></span>|<span data-ttu-id="3c463-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="3c463-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="3c463-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c463-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3c463-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3c463-153">displayName</span></span>|<span data-ttu-id="3c463-154">String</span><span class="sxs-lookup"><span data-stu-id="3c463-154">String</span></span>|<span data-ttu-id="3c463-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="3c463-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="3c463-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c463-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3c463-157">状态</span><span class="sxs-lookup"><span data-stu-id="3c463-157">status</span></span>|[<span data-ttu-id="3c463-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="3c463-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="3c463-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="3c463-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="3c463-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="3c463-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3c463-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="3c463-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="3c463-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="3c463-162">errorCode</span></span>|[<span data-ttu-id="3c463-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="3c463-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="3c463-164">错误代码（如果发生了任何错误）。</span><span class="sxs-lookup"><span data-stu-id="3c463-164">Error code if any occured.</span></span> <span data-ttu-id="3c463-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="3c463-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3c463-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="3c463-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="3c463-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="3c463-167">guidedDeploymentTags</span></span>|<span data-ttu-id="3c463-168">String collection</span><span class="sxs-lookup"><span data-stu-id="3c463-168">String collection</span></span>|<span data-ttu-id="3c463-169">引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c463-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3c463-170">响应</span><span class="sxs-lookup"><span data-stu-id="3c463-170">Response</span></span>
<span data-ttu-id="3c463-171">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c463-171">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c463-172">示例</span><span class="sxs-lookup"><span data-stu-id="3c463-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c463-173">请求</span><span class="sxs-lookup"><span data-stu-id="3c463-173">Request</span></span>
<span data-ttu-id="3c463-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c463-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="3c463-175">响应</span><span class="sxs-lookup"><span data-stu-id="3c463-175">Response</span></span>
<span data-ttu-id="3c463-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c463-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




