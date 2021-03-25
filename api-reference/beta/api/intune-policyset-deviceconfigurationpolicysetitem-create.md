---
title: 创建 deviceConfigurationPolicySetItem
description: 创建新的 deviceConfigurationPolicySetItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 292e617311f9b0897becd4808223186d077ec999
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158631"
---
# <a name="create-deviceconfigurationpolicysetitem"></a><span data-ttu-id="4473e-103">创建 deviceConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="4473e-103">Create deviceConfigurationPolicySetItem</span></span>

<span data-ttu-id="4473e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4473e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4473e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4473e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4473e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4473e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4473e-107">创建新的 [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4473e-107">Create a new [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4473e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4473e-108">Prerequisites</span></span>
<span data-ttu-id="4473e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4473e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4473e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4473e-111">Permission type</span></span>|<span data-ttu-id="4473e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4473e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4473e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4473e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4473e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4473e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4473e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4473e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4473e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4473e-116">Not supported.</span></span>|
|<span data-ttu-id="4473e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4473e-117">Application</span></span>|<span data-ttu-id="4473e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4473e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4473e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4473e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="4473e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4473e-120">Request headers</span></span>
|<span data-ttu-id="4473e-121">标头</span><span class="sxs-lookup"><span data-stu-id="4473e-121">Header</span></span>|<span data-ttu-id="4473e-122">值</span><span class="sxs-lookup"><span data-stu-id="4473e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4473e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4473e-123">Authorization</span></span>|<span data-ttu-id="4473e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4473e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4473e-125">接受</span><span class="sxs-lookup"><span data-stu-id="4473e-125">Accept</span></span>|<span data-ttu-id="4473e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4473e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4473e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4473e-127">Request body</span></span>
<span data-ttu-id="4473e-128">在请求正文中，提供 deviceConfigurationPolicySetItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4473e-128">In the request body, supply a JSON representation for the deviceConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="4473e-129">下表显示创建 deviceConfigurationPolicySetItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4473e-129">The following table shows the properties that are required when you create the deviceConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="4473e-130">属性</span><span class="sxs-lookup"><span data-stu-id="4473e-130">Property</span></span>|<span data-ttu-id="4473e-131">类型</span><span class="sxs-lookup"><span data-stu-id="4473e-131">Type</span></span>|<span data-ttu-id="4473e-132">说明</span><span class="sxs-lookup"><span data-stu-id="4473e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4473e-133">id</span><span class="sxs-lookup"><span data-stu-id="4473e-133">id</span></span>|<span data-ttu-id="4473e-134">String</span><span class="sxs-lookup"><span data-stu-id="4473e-134">String</span></span>|<span data-ttu-id="4473e-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="4473e-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="4473e-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4473e-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4473e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4473e-137">createdDateTime</span></span>|<span data-ttu-id="4473e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4473e-138">DateTimeOffset</span></span>|<span data-ttu-id="4473e-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="4473e-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="4473e-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4473e-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4473e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4473e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4473e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4473e-142">DateTimeOffset</span></span>|<span data-ttu-id="4473e-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="4473e-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="4473e-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4473e-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4473e-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="4473e-145">payloadId</span></span>|<span data-ttu-id="4473e-146">String</span><span class="sxs-lookup"><span data-stu-id="4473e-146">String</span></span>|<span data-ttu-id="4473e-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="4473e-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="4473e-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4473e-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4473e-149">itemType</span><span class="sxs-lookup"><span data-stu-id="4473e-149">itemType</span></span>|<span data-ttu-id="4473e-150">String</span><span class="sxs-lookup"><span data-stu-id="4473e-150">String</span></span>|<span data-ttu-id="4473e-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="4473e-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="4473e-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4473e-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4473e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4473e-153">displayName</span></span>|<span data-ttu-id="4473e-154">String</span><span class="sxs-lookup"><span data-stu-id="4473e-154">String</span></span>|<span data-ttu-id="4473e-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="4473e-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="4473e-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4473e-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4473e-157">状态</span><span class="sxs-lookup"><span data-stu-id="4473e-157">status</span></span>|[<span data-ttu-id="4473e-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="4473e-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="4473e-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="4473e-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="4473e-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4473e-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="4473e-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="4473e-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="4473e-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="4473e-162">errorCode</span></span>|[<span data-ttu-id="4473e-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="4473e-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="4473e-164">错误代码（如果发生了任何错误）。</span><span class="sxs-lookup"><span data-stu-id="4473e-164">Error code if any occured.</span></span> <span data-ttu-id="4473e-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4473e-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="4473e-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="4473e-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="4473e-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="4473e-167">guidedDeploymentTags</span></span>|<span data-ttu-id="4473e-168">String collection</span><span class="sxs-lookup"><span data-stu-id="4473e-168">String collection</span></span>|<span data-ttu-id="4473e-169">引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4473e-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4473e-170">响应</span><span class="sxs-lookup"><span data-stu-id="4473e-170">Response</span></span>
<span data-ttu-id="4473e-171">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4473e-171">If successful, this method returns a `201 Created` response code and a [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4473e-172">示例</span><span class="sxs-lookup"><span data-stu-id="4473e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4473e-173">请求</span><span class="sxs-lookup"><span data-stu-id="4473e-173">Request</span></span>
<span data-ttu-id="4473e-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4473e-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="4473e-175">响应</span><span class="sxs-lookup"><span data-stu-id="4473e-175">Response</span></span>
<span data-ttu-id="4473e-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4473e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 486

{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
  "id": "00b1197c-197c-00b1-7c19-b1007c19b100",
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




