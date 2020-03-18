---
title: 创建 groupPolicyUploadedDefinition
description: 创建新的 groupPolicyUploadedDefinition 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9cfc08f2af0fac9d421c253f123367bd65f9f4b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803762"
---
# <a name="create-grouppolicyuploadeddefinition"></a><span data-ttu-id="5e6f4-103">创建 groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="5e6f4-103">Create groupPolicyUploadedDefinition</span></span>

> <span data-ttu-id="5e6f4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e6f4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e6f4-106">创建新的[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-106">Create a new [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e6f4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e6f4-107">Prerequisites</span></span>
<span data-ttu-id="5e6f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e6f4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e6f4-110">Permission type</span></span>|<span data-ttu-id="5e6f4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e6f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e6f4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e6f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e6f4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e6f4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5e6f4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e6f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e6f4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-115">Not supported.</span></span>|
|<span data-ttu-id="5e6f4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e6f4-116">Application</span></span>|<span data-ttu-id="5e6f4-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e6f4-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e6f4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e6f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="5e6f4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e6f4-119">Request headers</span></span>
|<span data-ttu-id="5e6f4-120">标头</span><span class="sxs-lookup"><span data-stu-id="5e6f4-120">Header</span></span>|<span data-ttu-id="5e6f4-121">值</span><span class="sxs-lookup"><span data-stu-id="5e6f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e6f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e6f4-122">Authorization</span></span>|<span data-ttu-id="5e6f4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e6f4-124">接受</span><span class="sxs-lookup"><span data-stu-id="5e6f4-124">Accept</span></span>|<span data-ttu-id="5e6f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e6f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e6f4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e6f4-126">Request body</span></span>
<span data-ttu-id="5e6f4-127">在请求正文中，提供 groupPolicyUploadedDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-127">In the request body, supply a JSON representation for the groupPolicyUploadedDefinition object.</span></span>

<span data-ttu-id="5e6f4-128">下表显示创建 groupPolicyUploadedDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-128">The following table shows the properties that are required when you create the groupPolicyUploadedDefinition.</span></span>

|<span data-ttu-id="5e6f4-129">属性</span><span class="sxs-lookup"><span data-stu-id="5e6f4-129">Property</span></span>|<span data-ttu-id="5e6f4-130">类型</span><span class="sxs-lookup"><span data-stu-id="5e6f4-130">Type</span></span>|<span data-ttu-id="5e6f4-131">说明</span><span class="sxs-lookup"><span data-stu-id="5e6f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e6f4-132">classType</span><span class="sxs-lookup"><span data-stu-id="5e6f4-132">classType</span></span>|[<span data-ttu-id="5e6f4-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="5e6f4-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="5e6f4-134">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="5e6f4-135">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-135">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="5e6f4-136">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="5e6f4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5e6f4-137">displayName</span></span>|<span data-ttu-id="5e6f4-138">String</span><span class="sxs-lookup"><span data-stu-id="5e6f4-138">String</span></span>|<span data-ttu-id="5e6f4-139">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-139">The localized policy name.</span></span> <span data-ttu-id="5e6f4-140">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e6f4-140">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="5e6f4-141">explainText</span><span class="sxs-lookup"><span data-stu-id="5e6f4-141">explainText</span></span>|<span data-ttu-id="5e6f4-142">String</span><span class="sxs-lookup"><span data-stu-id="5e6f4-142">String</span></span>|<span data-ttu-id="5e6f4-143">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-143">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="5e6f4-144">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-144">The default value is empty.</span></span> <span data-ttu-id="5e6f4-145">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e6f4-145">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="5e6f4-146">categoryPath</span><span class="sxs-lookup"><span data-stu-id="5e6f4-146">categoryPath</span></span>|<span data-ttu-id="5e6f4-147">String</span><span class="sxs-lookup"><span data-stu-id="5e6f4-147">String</span></span>|<span data-ttu-id="5e6f4-148">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-148">The localized full category path for the policy.</span></span> <span data-ttu-id="5e6f4-149">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e6f4-149">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="5e6f4-150">supportedOn</span><span class="sxs-lookup"><span data-stu-id="5e6f4-150">supportedOn</span></span>|<span data-ttu-id="5e6f4-151">String</span><span class="sxs-lookup"><span data-stu-id="5e6f4-151">String</span></span>|<span data-ttu-id="5e6f4-152">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-152">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="5e6f4-153">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e6f4-153">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="5e6f4-154">policyType</span><span class="sxs-lookup"><span data-stu-id="5e6f4-154">policyType</span></span>|[<span data-ttu-id="5e6f4-155">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="5e6f4-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="5e6f4-156">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-156">Specifies the type of group policy.</span></span> <span data-ttu-id="5e6f4-157">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-157">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="5e6f4-158">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="5e6f4-159">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="5e6f4-159">groupPolicyCategoryId</span></span>|<span data-ttu-id="5e6f4-160">Guid</span><span class="sxs-lookup"><span data-stu-id="5e6f4-160">Guid</span></span>|<span data-ttu-id="5e6f4-161">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)的父类别的类别 id</span><span class="sxs-lookup"><span data-stu-id="5e6f4-161">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="5e6f4-162">id</span><span class="sxs-lookup"><span data-stu-id="5e6f4-162">id</span></span>|<span data-ttu-id="5e6f4-163">String</span><span class="sxs-lookup"><span data-stu-id="5e6f4-163">String</span></span>|<span data-ttu-id="5e6f4-164">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-164">Key of the entity.</span></span> <span data-ttu-id="5e6f4-165">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e6f4-165">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="5e6f4-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e6f4-166">lastModifiedDateTime</span></span>|<span data-ttu-id="5e6f4-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e6f4-167">DateTimeOffset</span></span>|<span data-ttu-id="5e6f4-168">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-168">The date and time the entity was last modified.</span></span> <span data-ttu-id="5e6f4-169">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e6f4-169">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5e6f4-170">响应</span><span class="sxs-lookup"><span data-stu-id="5e6f4-170">Response</span></span>
<span data-ttu-id="5e6f4-171">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-171">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e6f4-172">示例</span><span class="sxs-lookup"><span data-stu-id="5e6f4-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e6f4-173">请求</span><span class="sxs-lookup"><span data-stu-id="5e6f4-173">Request</span></span>
<span data-ttu-id="5e6f4-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
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

### <a name="response"></a><span data-ttu-id="5e6f4-175">响应</span><span class="sxs-lookup"><span data-stu-id="5e6f4-175">Response</span></span>
<span data-ttu-id="5e6f4-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e6f4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




