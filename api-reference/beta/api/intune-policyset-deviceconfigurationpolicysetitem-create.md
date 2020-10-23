---
title: 创建 deviceConfigurationPolicySetItem
description: 创建新的 deviceConfigurationPolicySetItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25a3688ecbf0090a40702db58a5d01588801fe70
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732776"
---
# <a name="create-deviceconfigurationpolicysetitem"></a><span data-ttu-id="4d3ab-103">创建 deviceConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="4d3ab-103">Create deviceConfigurationPolicySetItem</span></span>

<span data-ttu-id="4d3ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d3ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d3ab-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d3ab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d3ab-107">创建新的 [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-107">Create a new [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d3ab-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d3ab-108">Prerequisites</span></span>
<span data-ttu-id="4d3ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d3ab-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d3ab-111">Permission type</span></span>|<span data-ttu-id="4d3ab-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d3ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d3ab-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d3ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d3ab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d3ab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d3ab-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d3ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d3ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-116">Not supported.</span></span>|
|<span data-ttu-id="4d3ab-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d3ab-117">Application</span></span>|<span data-ttu-id="4d3ab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d3ab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d3ab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d3ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="4d3ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d3ab-120">Request headers</span></span>
|<span data-ttu-id="4d3ab-121">标头</span><span class="sxs-lookup"><span data-stu-id="4d3ab-121">Header</span></span>|<span data-ttu-id="4d3ab-122">值</span><span class="sxs-lookup"><span data-stu-id="4d3ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d3ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d3ab-123">Authorization</span></span>|<span data-ttu-id="4d3ab-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d3ab-125">接受</span><span class="sxs-lookup"><span data-stu-id="4d3ab-125">Accept</span></span>|<span data-ttu-id="4d3ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d3ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d3ab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d3ab-127">Request body</span></span>
<span data-ttu-id="4d3ab-128">在请求正文中，提供 deviceConfigurationPolicySetItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-128">In the request body, supply a JSON representation for the deviceConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="4d3ab-129">下表显示创建 deviceConfigurationPolicySetItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-129">The following table shows the properties that are required when you create the deviceConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="4d3ab-130">属性</span><span class="sxs-lookup"><span data-stu-id="4d3ab-130">Property</span></span>|<span data-ttu-id="4d3ab-131">类型</span><span class="sxs-lookup"><span data-stu-id="4d3ab-131">Type</span></span>|<span data-ttu-id="4d3ab-132">说明</span><span class="sxs-lookup"><span data-stu-id="4d3ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d3ab-133">id</span><span class="sxs-lookup"><span data-stu-id="4d3ab-133">id</span></span>|<span data-ttu-id="4d3ab-134">String</span><span class="sxs-lookup"><span data-stu-id="4d3ab-134">String</span></span>|<span data-ttu-id="4d3ab-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="4d3ab-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d3ab-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4d3ab-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d3ab-137">createdDateTime</span></span>|<span data-ttu-id="4d3ab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d3ab-138">DateTimeOffset</span></span>|<span data-ttu-id="4d3ab-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="4d3ab-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d3ab-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4d3ab-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d3ab-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4d3ab-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d3ab-142">DateTimeOffset</span></span>|<span data-ttu-id="4d3ab-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="4d3ab-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d3ab-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4d3ab-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="4d3ab-145">payloadId</span></span>|<span data-ttu-id="4d3ab-146">String</span><span class="sxs-lookup"><span data-stu-id="4d3ab-146">String</span></span>|<span data-ttu-id="4d3ab-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="4d3ab-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d3ab-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4d3ab-149">itemType</span><span class="sxs-lookup"><span data-stu-id="4d3ab-149">itemType</span></span>|<span data-ttu-id="4d3ab-150">String</span><span class="sxs-lookup"><span data-stu-id="4d3ab-150">String</span></span>|<span data-ttu-id="4d3ab-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="4d3ab-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d3ab-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4d3ab-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4d3ab-153">displayName</span></span>|<span data-ttu-id="4d3ab-154">String</span><span class="sxs-lookup"><span data-stu-id="4d3ab-154">String</span></span>|<span data-ttu-id="4d3ab-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="4d3ab-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d3ab-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4d3ab-157">status</span><span class="sxs-lookup"><span data-stu-id="4d3ab-157">status</span></span>|[<span data-ttu-id="4d3ab-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="4d3ab-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="4d3ab-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="4d3ab-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="4d3ab-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="4d3ab-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="4d3ab-162">errorCode</span></span>|[<span data-ttu-id="4d3ab-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="4d3ab-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="4d3ab-164">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-164">Error code if any occured.</span></span> <span data-ttu-id="4d3ab-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="4d3ab-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="4d3ab-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="4d3ab-167">guidedDeploymentTags</span></span>|<span data-ttu-id="4d3ab-168">String collection</span><span class="sxs-lookup"><span data-stu-id="4d3ab-168">String collection</span></span>|<span data-ttu-id="4d3ab-169">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="4d3ab-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4d3ab-170">响应</span><span class="sxs-lookup"><span data-stu-id="4d3ab-170">Response</span></span>
<span data-ttu-id="4d3ab-171">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-171">If successful, this method returns a `201 Created` response code and a [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d3ab-172">示例</span><span class="sxs-lookup"><span data-stu-id="4d3ab-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d3ab-173">请求</span><span class="sxs-lookup"><span data-stu-id="4d3ab-173">Request</span></span>
<span data-ttu-id="4d3ab-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d3ab-175">响应</span><span class="sxs-lookup"><span data-stu-id="4d3ab-175">Response</span></span>
<span data-ttu-id="4d3ab-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d3ab-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





