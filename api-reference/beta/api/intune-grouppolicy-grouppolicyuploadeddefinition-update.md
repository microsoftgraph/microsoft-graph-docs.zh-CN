---
title: 更新 groupPolicyUploadedDefinition
description: 更新 groupPolicyUploadedDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5421ecaa9c7d3b91ed71a5602a0d06130c2fee0e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000467"
---
# <a name="update-grouppolicyuploadeddefinition"></a><span data-ttu-id="d6623-103">更新 groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="d6623-103">Update groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="d6623-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6623-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6623-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6623-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6623-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6623-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6623-107">更新 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6623-107">Update the properties of a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6623-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6623-108">Prerequisites</span></span>
<span data-ttu-id="d6623-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6623-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6623-111">Permission type</span></span>|<span data-ttu-id="d6623-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6623-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6623-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6623-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6623-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6623-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6623-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6623-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6623-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6623-116">Not supported.</span></span>|
|<span data-ttu-id="d6623-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6623-117">Application</span></span>|<span data-ttu-id="d6623-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6623-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6623-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6623-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="d6623-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6623-120">Request headers</span></span>
|<span data-ttu-id="d6623-121">标头</span><span class="sxs-lookup"><span data-stu-id="d6623-121">Header</span></span>|<span data-ttu-id="d6623-122">值</span><span class="sxs-lookup"><span data-stu-id="d6623-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6623-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6623-123">Authorization</span></span>|<span data-ttu-id="d6623-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6623-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6623-125">接受</span><span class="sxs-lookup"><span data-stu-id="d6623-125">Accept</span></span>|<span data-ttu-id="d6623-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6623-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6623-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6623-127">Request body</span></span>
<span data-ttu-id="d6623-128">在请求正文中，提供 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6623-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

<span data-ttu-id="d6623-129">下表显示创建 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d6623-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span></span>

|<span data-ttu-id="d6623-130">属性</span><span class="sxs-lookup"><span data-stu-id="d6623-130">Property</span></span>|<span data-ttu-id="d6623-131">类型</span><span class="sxs-lookup"><span data-stu-id="d6623-131">Type</span></span>|<span data-ttu-id="d6623-132">说明</span><span class="sxs-lookup"><span data-stu-id="d6623-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6623-133">classType</span><span class="sxs-lookup"><span data-stu-id="d6623-133">classType</span></span>|[<span data-ttu-id="d6623-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="d6623-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="d6623-135">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="d6623-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="d6623-136">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="d6623-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="d6623-137">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="d6623-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="d6623-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d6623-138">displayName</span></span>|<span data-ttu-id="d6623-139">String</span><span class="sxs-lookup"><span data-stu-id="d6623-139">String</span></span>|<span data-ttu-id="d6623-140">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="d6623-140">The localized policy name.</span></span> <span data-ttu-id="d6623-141">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6623-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="d6623-142">explainText</span><span class="sxs-lookup"><span data-stu-id="d6623-142">explainText</span></span>|<span data-ttu-id="d6623-143">String</span><span class="sxs-lookup"><span data-stu-id="d6623-143">String</span></span>|<span data-ttu-id="d6623-144">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="d6623-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="d6623-145">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="d6623-145">The default value is empty.</span></span> <span data-ttu-id="d6623-146">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6623-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="d6623-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="d6623-147">categoryPath</span></span>|<span data-ttu-id="d6623-148">String</span><span class="sxs-lookup"><span data-stu-id="d6623-148">String</span></span>|<span data-ttu-id="d6623-149">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="d6623-149">The localized full category path for the policy.</span></span> <span data-ttu-id="d6623-150">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6623-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="d6623-151">supportedOn</span><span class="sxs-lookup"><span data-stu-id="d6623-151">supportedOn</span></span>|<span data-ttu-id="d6623-152">String</span><span class="sxs-lookup"><span data-stu-id="d6623-152">String</span></span>|<span data-ttu-id="d6623-153">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="d6623-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="d6623-154">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6623-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="d6623-155">policyType</span><span class="sxs-lookup"><span data-stu-id="d6623-155">policyType</span></span>|[<span data-ttu-id="d6623-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="d6623-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="d6623-157">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="d6623-157">Specifies the type of group policy.</span></span> <span data-ttu-id="d6623-158">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="d6623-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="d6623-159">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="d6623-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="d6623-160">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="d6623-160">groupPolicyCategoryId</span></span>|<span data-ttu-id="d6623-161">Guid</span><span class="sxs-lookup"><span data-stu-id="d6623-161">Guid</span></span>|<span data-ttu-id="d6623-162">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)的父类别的类别 id</span><span class="sxs-lookup"><span data-stu-id="d6623-162">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="d6623-163">id</span><span class="sxs-lookup"><span data-stu-id="d6623-163">id</span></span>|<span data-ttu-id="d6623-164">String</span><span class="sxs-lookup"><span data-stu-id="d6623-164">String</span></span>|<span data-ttu-id="d6623-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d6623-165">Key of the entity.</span></span> <span data-ttu-id="d6623-166">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6623-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="d6623-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6623-167">lastModifiedDateTime</span></span>|<span data-ttu-id="d6623-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6623-168">DateTimeOffset</span></span>|<span data-ttu-id="d6623-169">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d6623-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="d6623-170">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6623-170">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d6623-171">响应</span><span class="sxs-lookup"><span data-stu-id="d6623-171">Response</span></span>
<span data-ttu-id="d6623-172">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6623-172">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6623-173">示例</span><span class="sxs-lookup"><span data-stu-id="d6623-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6623-174">请求</span><span class="sxs-lookup"><span data-stu-id="d6623-174">Request</span></span>
<span data-ttu-id="d6623-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6623-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d"
}
```

### <a name="response"></a><span data-ttu-id="d6623-176">响应</span><span class="sxs-lookup"><span data-stu-id="d6623-176">Response</span></span>
<span data-ttu-id="d6623-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6623-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






