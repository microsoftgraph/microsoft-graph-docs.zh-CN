---
title: 创建 policySet
description: 创建新的 policySet 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e085eb0ae86d6a93895b4c88d17664abc84536ee
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537399"
---
# <a name="create-policyset"></a><span data-ttu-id="633b1-103">创建 policySet</span><span class="sxs-lookup"><span data-stu-id="633b1-103">Create policySet</span></span>

> <span data-ttu-id="633b1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="633b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="633b1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="633b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="633b1-106">创建新的[policySet](../resources/intune-policyset-policyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="633b1-106">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="633b1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="633b1-107">Prerequisites</span></span>
<span data-ttu-id="633b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="633b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="633b1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="633b1-110">Permission type</span></span>|<span data-ttu-id="633b1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="633b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="633b1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="633b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="633b1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633b1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="633b1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="633b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="633b1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="633b1-115">Not supported.</span></span>|
|<span data-ttu-id="633b1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="633b1-116">Application</span></span>|<span data-ttu-id="633b1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633b1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="633b1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="633b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="633b1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="633b1-119">Request headers</span></span>
|<span data-ttu-id="633b1-120">标头</span><span class="sxs-lookup"><span data-stu-id="633b1-120">Header</span></span>|<span data-ttu-id="633b1-121">值</span><span class="sxs-lookup"><span data-stu-id="633b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="633b1-122">授权</span><span class="sxs-lookup"><span data-stu-id="633b1-122">Authorization</span></span>|<span data-ttu-id="633b1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="633b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="633b1-124">接受</span><span class="sxs-lookup"><span data-stu-id="633b1-124">Accept</span></span>|<span data-ttu-id="633b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="633b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="633b1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="633b1-126">Request body</span></span>
<span data-ttu-id="633b1-127">在请求正文中，提供 policySet 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="633b1-127">In the request body, supply a JSON representation for the policySet object.</span></span>

<span data-ttu-id="633b1-128">下表显示创建 policySet 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="633b1-128">The following table shows the properties that are required when you create the policySet.</span></span>

|<span data-ttu-id="633b1-129">属性</span><span class="sxs-lookup"><span data-stu-id="633b1-129">Property</span></span>|<span data-ttu-id="633b1-130">类型</span><span class="sxs-lookup"><span data-stu-id="633b1-130">Type</span></span>|<span data-ttu-id="633b1-131">说明</span><span class="sxs-lookup"><span data-stu-id="633b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="633b1-132">id</span><span class="sxs-lookup"><span data-stu-id="633b1-132">id</span></span>|<span data-ttu-id="633b1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="633b1-133">String</span></span>|<span data-ttu-id="633b1-134">PolicySet 的键。</span><span class="sxs-lookup"><span data-stu-id="633b1-134">Key of the PolicySet.</span></span>|
|<span data-ttu-id="633b1-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="633b1-135">createdDateTime</span></span>|<span data-ttu-id="633b1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="633b1-136">DateTimeOffset</span></span>|<span data-ttu-id="633b1-137">PolicySet 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="633b1-137">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="633b1-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="633b1-138">lastModifiedDateTime</span></span>|<span data-ttu-id="633b1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="633b1-139">DateTimeOffset</span></span>|<span data-ttu-id="633b1-140">PolicySet 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="633b1-140">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="633b1-141">displayName</span><span class="sxs-lookup"><span data-stu-id="633b1-141">displayName</span></span>|<span data-ttu-id="633b1-142">String</span><span class="sxs-lookup"><span data-stu-id="633b1-142">String</span></span>|<span data-ttu-id="633b1-143">PolicySet 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="633b1-143">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="633b1-144">说明</span><span class="sxs-lookup"><span data-stu-id="633b1-144">description</span></span>|<span data-ttu-id="633b1-145">String</span><span class="sxs-lookup"><span data-stu-id="633b1-145">String</span></span>|<span data-ttu-id="633b1-146">PolicySet 的说明。</span><span class="sxs-lookup"><span data-stu-id="633b1-146">Description of the PolicySet.</span></span>|
|<span data-ttu-id="633b1-147">status</span><span class="sxs-lookup"><span data-stu-id="633b1-147">status</span></span>|[<span data-ttu-id="633b1-148">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="633b1-148">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="633b1-149">PolicySet 的验证/分配状态。</span><span class="sxs-lookup"><span data-stu-id="633b1-149">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="633b1-150">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="633b1-150">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="633b1-151">errorCode</span><span class="sxs-lookup"><span data-stu-id="633b1-151">errorCode</span></span>|[<span data-ttu-id="633b1-152">errorCode</span><span class="sxs-lookup"><span data-stu-id="633b1-152">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="633b1-153">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="633b1-153">Error code if any occured.</span></span> <span data-ttu-id="633b1-154">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="633b1-154">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="633b1-155">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="633b1-155">guidedDeploymentTags</span></span>|<span data-ttu-id="633b1-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="633b1-156">String collection</span></span>|<span data-ttu-id="633b1-157">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="633b1-157">Tags of the guided deployment</span></span>|
|<span data-ttu-id="633b1-158">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="633b1-158">roleScopeTags</span></span>|<span data-ttu-id="633b1-159">String 集合</span><span class="sxs-lookup"><span data-stu-id="633b1-159">String collection</span></span>|<span data-ttu-id="633b1-160">PolicySet 的 RoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="633b1-160">RoleScopeTags of the PolicySet</span></span>|



## <a name="response"></a><span data-ttu-id="633b1-161">响应</span><span class="sxs-lookup"><span data-stu-id="633b1-161">Response</span></span>
<span data-ttu-id="633b1-162">如果成功，此方法在响应`201 Created`正文中返回响应代码和[policySet](../resources/intune-policyset-policyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="633b1-162">If successful, this method returns a `201 Created` response code and a [policySet](../resources/intune-policyset-policyset.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="633b1-163">示例</span><span class="sxs-lookup"><span data-stu-id="633b1-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="633b1-164">请求</span><span class="sxs-lookup"><span data-stu-id="633b1-164">Request</span></span>
<span data-ttu-id="633b1-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="633b1-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="633b1-166">响应</span><span class="sxs-lookup"><span data-stu-id="633b1-166">Response</span></span>
<span data-ttu-id="633b1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="633b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






