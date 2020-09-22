---
title: 创建 policySet
description: 创建新的 policySet 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93eb8bc0f8aa415190f5e0e4b3f0dbdc4fe317a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004849"
---
# <a name="create-policyset"></a><span data-ttu-id="b6e4f-103">创建 policySet</span><span class="sxs-lookup"><span data-stu-id="b6e4f-103">Create policySet</span></span>

<span data-ttu-id="b6e4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6e4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6e4f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6e4f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6e4f-107">创建新的 [policySet](../resources/intune-policyset-policyset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-107">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6e4f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6e4f-108">Prerequisites</span></span>
<span data-ttu-id="b6e4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6e4f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6e4f-111">Permission type</span></span>|<span data-ttu-id="b6e4f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6e4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6e4f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6e4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6e4f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e4f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6e4f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6e4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6e4f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-116">Not supported.</span></span>|
|<span data-ttu-id="b6e4f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6e4f-117">Application</span></span>|<span data-ttu-id="b6e4f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e4f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6e4f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6e4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="b6e4f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6e4f-120">Request headers</span></span>
|<span data-ttu-id="b6e4f-121">标头</span><span class="sxs-lookup"><span data-stu-id="b6e4f-121">Header</span></span>|<span data-ttu-id="b6e4f-122">值</span><span class="sxs-lookup"><span data-stu-id="b6e4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6e4f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6e4f-123">Authorization</span></span>|<span data-ttu-id="b6e4f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6e4f-125">接受</span><span class="sxs-lookup"><span data-stu-id="b6e4f-125">Accept</span></span>|<span data-ttu-id="b6e4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6e4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6e4f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6e4f-127">Request body</span></span>
<span data-ttu-id="b6e4f-128">在请求正文中，提供 policySet 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-128">In the request body, supply a JSON representation for the policySet object.</span></span>

<span data-ttu-id="b6e4f-129">下表显示创建 policySet 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-129">The following table shows the properties that are required when you create the policySet.</span></span>

|<span data-ttu-id="b6e4f-130">属性</span><span class="sxs-lookup"><span data-stu-id="b6e4f-130">Property</span></span>|<span data-ttu-id="b6e4f-131">类型</span><span class="sxs-lookup"><span data-stu-id="b6e4f-131">Type</span></span>|<span data-ttu-id="b6e4f-132">说明</span><span class="sxs-lookup"><span data-stu-id="b6e4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6e4f-133">id</span><span class="sxs-lookup"><span data-stu-id="b6e4f-133">id</span></span>|<span data-ttu-id="b6e4f-134">String</span><span class="sxs-lookup"><span data-stu-id="b6e4f-134">String</span></span>|<span data-ttu-id="b6e4f-135">PolicySet 的键。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-135">Key of the PolicySet.</span></span>|
|<span data-ttu-id="b6e4f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e4f-136">createdDateTime</span></span>|<span data-ttu-id="b6e4f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e4f-137">DateTimeOffset</span></span>|<span data-ttu-id="b6e4f-138">PolicySet 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-138">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="b6e4f-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e4f-139">lastModifiedDateTime</span></span>|<span data-ttu-id="b6e4f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e4f-140">DateTimeOffset</span></span>|<span data-ttu-id="b6e4f-141">PolicySet 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-141">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="b6e4f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b6e4f-142">displayName</span></span>|<span data-ttu-id="b6e4f-143">String</span><span class="sxs-lookup"><span data-stu-id="b6e4f-143">String</span></span>|<span data-ttu-id="b6e4f-144">PolicySet 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-144">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="b6e4f-145">description</span><span class="sxs-lookup"><span data-stu-id="b6e4f-145">description</span></span>|<span data-ttu-id="b6e4f-146">String</span><span class="sxs-lookup"><span data-stu-id="b6e4f-146">String</span></span>|<span data-ttu-id="b6e4f-147">PolicySet 的说明。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-147">Description of the PolicySet.</span></span>|
|<span data-ttu-id="b6e4f-148">状态</span><span class="sxs-lookup"><span data-stu-id="b6e4f-148">status</span></span>|[<span data-ttu-id="b6e4f-149">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b6e4f-149">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b6e4f-150">PolicySet 的验证/分配状态。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-150">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="b6e4f-151">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-151">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b6e4f-152">errorCode</span><span class="sxs-lookup"><span data-stu-id="b6e4f-152">errorCode</span></span>|[<span data-ttu-id="b6e4f-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="b6e4f-153">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b6e4f-154">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-154">Error code if any occured.</span></span> <span data-ttu-id="b6e4f-155">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-155">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b6e4f-156">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b6e4f-156">guidedDeploymentTags</span></span>|<span data-ttu-id="b6e4f-157">String collection</span><span class="sxs-lookup"><span data-stu-id="b6e4f-157">String collection</span></span>|<span data-ttu-id="b6e4f-158">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="b6e4f-158">Tags of the guided deployment</span></span>|
|<span data-ttu-id="b6e4f-159">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6e4f-159">roleScopeTags</span></span>|<span data-ttu-id="b6e4f-160">String collection</span><span class="sxs-lookup"><span data-stu-id="b6e4f-160">String collection</span></span>|<span data-ttu-id="b6e4f-161">PolicySet 的 RoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6e4f-161">RoleScopeTags of the PolicySet</span></span>|



## <a name="response"></a><span data-ttu-id="b6e4f-162">响应</span><span class="sxs-lookup"><span data-stu-id="b6e4f-162">Response</span></span>
<span data-ttu-id="b6e4f-163">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [policySet](../resources/intune-policyset-policyset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-163">If successful, this method returns a `201 Created` response code and a [policySet](../resources/intune-policyset-policyset.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6e4f-164">示例</span><span class="sxs-lookup"><span data-stu-id="b6e4f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6e4f-165">请求</span><span class="sxs-lookup"><span data-stu-id="b6e4f-165">Request</span></span>
<span data-ttu-id="b6e4f-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.policySet",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b6e4f-167">响应</span><span class="sxs-lookup"><span data-stu-id="b6e4f-167">Response</span></span>
<span data-ttu-id="b6e4f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6e4f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "653cb373-b373-653c-73b3-3c6573b33c65",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```






