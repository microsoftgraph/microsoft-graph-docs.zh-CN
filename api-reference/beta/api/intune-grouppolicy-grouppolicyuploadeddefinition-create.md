---
title: 创建 groupPolicyUploadedDefinition
description: 创建新的 groupPolicyUploadedDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab254aae6e5d319fa10515a10165feb9eafb8899
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444660"
---
# <a name="create-grouppolicyuploadeddefinition"></a><span data-ttu-id="e3995-103">创建 groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="e3995-103">Create groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="e3995-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3995-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3995-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3995-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3995-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3995-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3995-107">创建新的[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3995-107">Create a new [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3995-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e3995-108">Prerequisites</span></span>
<span data-ttu-id="e3995-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3995-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3995-111">Permission type</span></span>|<span data-ttu-id="e3995-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e3995-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3995-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3995-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3995-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3995-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3995-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3995-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3995-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3995-116">Not supported.</span></span>|
|<span data-ttu-id="e3995-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3995-117">Application</span></span>|<span data-ttu-id="e3995-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3995-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3995-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3995-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="e3995-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3995-120">Request headers</span></span>
|<span data-ttu-id="e3995-121">标头</span><span class="sxs-lookup"><span data-stu-id="e3995-121">Header</span></span>|<span data-ttu-id="e3995-122">值</span><span class="sxs-lookup"><span data-stu-id="e3995-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3995-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3995-123">Authorization</span></span>|<span data-ttu-id="e3995-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e3995-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3995-125">接受</span><span class="sxs-lookup"><span data-stu-id="e3995-125">Accept</span></span>|<span data-ttu-id="e3995-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3995-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3995-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3995-127">Request body</span></span>
<span data-ttu-id="e3995-128">在请求正文中，提供 groupPolicyUploadedDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3995-128">In the request body, supply a JSON representation for the groupPolicyUploadedDefinition object.</span></span>

<span data-ttu-id="e3995-129">下表显示创建 groupPolicyUploadedDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e3995-129">The following table shows the properties that are required when you create the groupPolicyUploadedDefinition.</span></span>

|<span data-ttu-id="e3995-130">属性</span><span class="sxs-lookup"><span data-stu-id="e3995-130">Property</span></span>|<span data-ttu-id="e3995-131">类型</span><span class="sxs-lookup"><span data-stu-id="e3995-131">Type</span></span>|<span data-ttu-id="e3995-132">说明</span><span class="sxs-lookup"><span data-stu-id="e3995-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3995-133">classType</span><span class="sxs-lookup"><span data-stu-id="e3995-133">classType</span></span>|[<span data-ttu-id="e3995-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="e3995-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="e3995-135">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="e3995-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="e3995-136">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e3995-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="e3995-137">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="e3995-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="e3995-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e3995-138">displayName</span></span>|<span data-ttu-id="e3995-139">String</span><span class="sxs-lookup"><span data-stu-id="e3995-139">String</span></span>|<span data-ttu-id="e3995-140">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="e3995-140">The localized policy name.</span></span> <span data-ttu-id="e3995-141">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e3995-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e3995-142">explainText</span><span class="sxs-lookup"><span data-stu-id="e3995-142">explainText</span></span>|<span data-ttu-id="e3995-143">String</span><span class="sxs-lookup"><span data-stu-id="e3995-143">String</span></span>|<span data-ttu-id="e3995-144">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="e3995-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="e3995-145">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="e3995-145">The default value is empty.</span></span> <span data-ttu-id="e3995-146">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e3995-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e3995-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="e3995-147">categoryPath</span></span>|<span data-ttu-id="e3995-148">String</span><span class="sxs-lookup"><span data-stu-id="e3995-148">String</span></span>|<span data-ttu-id="e3995-149">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="e3995-149">The localized full category path for the policy.</span></span> <span data-ttu-id="e3995-150">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e3995-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e3995-151">supportedOn</span><span class="sxs-lookup"><span data-stu-id="e3995-151">supportedOn</span></span>|<span data-ttu-id="e3995-152">String</span><span class="sxs-lookup"><span data-stu-id="e3995-152">String</span></span>|<span data-ttu-id="e3995-153">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="e3995-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="e3995-154">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e3995-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e3995-155">policyType</span><span class="sxs-lookup"><span data-stu-id="e3995-155">policyType</span></span>|[<span data-ttu-id="e3995-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="e3995-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="e3995-157">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="e3995-157">Specifies the type of group policy.</span></span> <span data-ttu-id="e3995-158">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e3995-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="e3995-159">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="e3995-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="e3995-160">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="e3995-160">groupPolicyCategoryId</span></span>|<span data-ttu-id="e3995-161">Guid</span><span class="sxs-lookup"><span data-stu-id="e3995-161">Guid</span></span>|<span data-ttu-id="e3995-162">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)的父类别的类别 id</span><span class="sxs-lookup"><span data-stu-id="e3995-162">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e3995-163">id</span><span class="sxs-lookup"><span data-stu-id="e3995-163">id</span></span>|<span data-ttu-id="e3995-164">String</span><span class="sxs-lookup"><span data-stu-id="e3995-164">String</span></span>|<span data-ttu-id="e3995-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e3995-165">Key of the entity.</span></span> <span data-ttu-id="e3995-166">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e3995-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e3995-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3995-167">lastModifiedDateTime</span></span>|<span data-ttu-id="e3995-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3995-168">DateTimeOffset</span></span>|<span data-ttu-id="e3995-169">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e3995-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="e3995-170">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e3995-170">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e3995-171">响应</span><span class="sxs-lookup"><span data-stu-id="e3995-171">Response</span></span>
<span data-ttu-id="e3995-172">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3995-172">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3995-173">示例</span><span class="sxs-lookup"><span data-stu-id="e3995-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3995-174">请求</span><span class="sxs-lookup"><span data-stu-id="e3995-174">Request</span></span>
<span data-ttu-id="e3995-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3995-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3995-176">响应</span><span class="sxs-lookup"><span data-stu-id="e3995-176">Response</span></span>
<span data-ttu-id="e3995-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3995-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



