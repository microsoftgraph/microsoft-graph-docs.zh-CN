---
title: 更新 groupPolicyUploadedDefinition
description: 更新 groupPolicyUploadedDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4103b13e8dc7c34c0fb7b9fe90c1e7d01c0f3c06
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224975"
---
# <a name="update-grouppolicyuploadeddefinition"></a><span data-ttu-id="b6224-103">更新 groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="b6224-103">Update groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="b6224-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6224-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6224-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6224-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6224-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6224-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6224-107">更新 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6224-107">Update the properties of a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6224-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6224-108">Prerequisites</span></span>
<span data-ttu-id="b6224-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6224-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6224-111">Permission type</span></span>|<span data-ttu-id="b6224-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6224-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6224-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6224-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6224-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6224-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6224-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6224-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6224-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6224-116">Not supported.</span></span>|
|<span data-ttu-id="b6224-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6224-117">Application</span></span>|<span data-ttu-id="b6224-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6224-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6224-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6224-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b6224-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6224-120">Request headers</span></span>
|<span data-ttu-id="b6224-121">标头</span><span class="sxs-lookup"><span data-stu-id="b6224-121">Header</span></span>|<span data-ttu-id="b6224-122">值</span><span class="sxs-lookup"><span data-stu-id="b6224-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6224-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6224-123">Authorization</span></span>|<span data-ttu-id="b6224-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6224-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6224-125">接受</span><span class="sxs-lookup"><span data-stu-id="b6224-125">Accept</span></span>|<span data-ttu-id="b6224-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6224-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6224-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6224-127">Request body</span></span>
<span data-ttu-id="b6224-128">在请求正文中，提供 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6224-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

<span data-ttu-id="b6224-129">下表显示创建 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6224-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span></span>

|<span data-ttu-id="b6224-130">属性</span><span class="sxs-lookup"><span data-stu-id="b6224-130">Property</span></span>|<span data-ttu-id="b6224-131">类型</span><span class="sxs-lookup"><span data-stu-id="b6224-131">Type</span></span>|<span data-ttu-id="b6224-132">说明</span><span class="sxs-lookup"><span data-stu-id="b6224-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6224-133">classType</span><span class="sxs-lookup"><span data-stu-id="b6224-133">classType</span></span>|[<span data-ttu-id="b6224-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="b6224-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="b6224-135">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="b6224-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="b6224-136">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b6224-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="b6224-137">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="b6224-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="b6224-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b6224-138">displayName</span></span>|<span data-ttu-id="b6224-139">String</span><span class="sxs-lookup"><span data-stu-id="b6224-139">String</span></span>|<span data-ttu-id="b6224-140">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="b6224-140">The localized policy name.</span></span> <span data-ttu-id="b6224-141">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b6224-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="b6224-142">explainText</span><span class="sxs-lookup"><span data-stu-id="b6224-142">explainText</span></span>|<span data-ttu-id="b6224-143">String</span><span class="sxs-lookup"><span data-stu-id="b6224-143">String</span></span>|<span data-ttu-id="b6224-144">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="b6224-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="b6224-145">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="b6224-145">The default value is empty.</span></span> <span data-ttu-id="b6224-146">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b6224-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="b6224-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="b6224-147">categoryPath</span></span>|<span data-ttu-id="b6224-148">String</span><span class="sxs-lookup"><span data-stu-id="b6224-148">String</span></span>|<span data-ttu-id="b6224-149">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="b6224-149">The localized full category path for the policy.</span></span> <span data-ttu-id="b6224-150">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b6224-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="b6224-151">supportedOn</span><span class="sxs-lookup"><span data-stu-id="b6224-151">supportedOn</span></span>|<span data-ttu-id="b6224-152">String</span><span class="sxs-lookup"><span data-stu-id="b6224-152">String</span></span>|<span data-ttu-id="b6224-153">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="b6224-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="b6224-154">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b6224-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="b6224-155">policyType</span><span class="sxs-lookup"><span data-stu-id="b6224-155">policyType</span></span>|[<span data-ttu-id="b6224-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="b6224-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="b6224-157">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="b6224-157">Specifies the type of group policy.</span></span> <span data-ttu-id="b6224-158">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b6224-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="b6224-159">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="b6224-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="b6224-160">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="b6224-160">groupPolicyCategoryId</span></span>|<span data-ttu-id="b6224-161">Guid</span><span class="sxs-lookup"><span data-stu-id="b6224-161">Guid</span></span>|<span data-ttu-id="b6224-162">继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)的父类别的类别 id</span><span class="sxs-lookup"><span data-stu-id="b6224-162">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="b6224-163">id</span><span class="sxs-lookup"><span data-stu-id="b6224-163">id</span></span>|<span data-ttu-id="b6224-164">String</span><span class="sxs-lookup"><span data-stu-id="b6224-164">String</span></span>|<span data-ttu-id="b6224-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6224-165">Key of the entity.</span></span> <span data-ttu-id="b6224-166">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b6224-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="b6224-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6224-167">lastModifiedDateTime</span></span>|<span data-ttu-id="b6224-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6224-168">DateTimeOffset</span></span>|<span data-ttu-id="b6224-169">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b6224-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="b6224-170">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b6224-170">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b6224-171">响应</span><span class="sxs-lookup"><span data-stu-id="b6224-171">Response</span></span>
<span data-ttu-id="b6224-172">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6224-172">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6224-173">示例</span><span class="sxs-lookup"><span data-stu-id="b6224-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6224-174">请求</span><span class="sxs-lookup"><span data-stu-id="b6224-174">Request</span></span>
<span data-ttu-id="b6224-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6224-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6224-176">响应</span><span class="sxs-lookup"><span data-stu-id="b6224-176">Response</span></span>
<span data-ttu-id="b6224-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6224-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




