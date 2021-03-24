---
title: 更新 groupPolicyUploadedDefinition
description: 更新 groupPolicyUploadedDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f643d8f957590f2a619174ccc50545bdd5b53520
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135276"
---
# <a name="update-grouppolicyuploadeddefinition"></a><span data-ttu-id="e2504-103">更新 groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="e2504-103">Update groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="e2504-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2504-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2504-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2504-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2504-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2504-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2504-107">更新 [groupPolicyUploadedDefinition 对象](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e2504-107">Update the properties of a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2504-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2504-108">Prerequisites</span></span>
<span data-ttu-id="e2504-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2504-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2504-111">Permission type</span></span>|<span data-ttu-id="e2504-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2504-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2504-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2504-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2504-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2504-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2504-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2504-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2504-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2504-116">Not supported.</span></span>|
|<span data-ttu-id="e2504-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2504-117">Application</span></span>|<span data-ttu-id="e2504-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2504-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2504-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2504-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e2504-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2504-120">Request headers</span></span>
|<span data-ttu-id="e2504-121">标头</span><span class="sxs-lookup"><span data-stu-id="e2504-121">Header</span></span>|<span data-ttu-id="e2504-122">值</span><span class="sxs-lookup"><span data-stu-id="e2504-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2504-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2504-123">Authorization</span></span>|<span data-ttu-id="e2504-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2504-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2504-125">接受</span><span class="sxs-lookup"><span data-stu-id="e2504-125">Accept</span></span>|<span data-ttu-id="e2504-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2504-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2504-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2504-127">Request body</span></span>
<span data-ttu-id="e2504-128">在请求正文中，提供 [groupPolicyUploadedDefinition 对象的](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2504-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

<span data-ttu-id="e2504-129">下表显示创建 [groupPolicyUploadedDefinition 时所需的属性](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e2504-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span></span>

|<span data-ttu-id="e2504-130">属性</span><span class="sxs-lookup"><span data-stu-id="e2504-130">Property</span></span>|<span data-ttu-id="e2504-131">类型</span><span class="sxs-lookup"><span data-stu-id="e2504-131">Type</span></span>|<span data-ttu-id="e2504-132">说明</span><span class="sxs-lookup"><span data-stu-id="e2504-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2504-133">classType</span><span class="sxs-lookup"><span data-stu-id="e2504-133">classType</span></span>|[<span data-ttu-id="e2504-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="e2504-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="e2504-135">标识策略可应用于的组类型。</span><span class="sxs-lookup"><span data-stu-id="e2504-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="e2504-136">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e2504-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="e2504-137">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="e2504-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="e2504-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e2504-138">displayName</span></span>|<span data-ttu-id="e2504-139">String</span><span class="sxs-lookup"><span data-stu-id="e2504-139">String</span></span>|<span data-ttu-id="e2504-140">本地化的策略名称。</span><span class="sxs-lookup"><span data-stu-id="e2504-140">The localized policy name.</span></span> <span data-ttu-id="e2504-141">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2504-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e2504-142">explainText</span><span class="sxs-lookup"><span data-stu-id="e2504-142">explainText</span></span>|<span data-ttu-id="e2504-143">String</span><span class="sxs-lookup"><span data-stu-id="e2504-143">String</span></span>|<span data-ttu-id="e2504-144">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="e2504-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="e2504-145">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="e2504-145">The default value is empty.</span></span> <span data-ttu-id="e2504-146">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2504-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e2504-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="e2504-147">categoryPath</span></span>|<span data-ttu-id="e2504-148">String</span><span class="sxs-lookup"><span data-stu-id="e2504-148">String</span></span>|<span data-ttu-id="e2504-149">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="e2504-149">The localized full category path for the policy.</span></span> <span data-ttu-id="e2504-150">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2504-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e2504-151">supportedOn</span><span class="sxs-lookup"><span data-stu-id="e2504-151">supportedOn</span></span>|<span data-ttu-id="e2504-152">String</span><span class="sxs-lookup"><span data-stu-id="e2504-152">String</span></span>|<span data-ttu-id="e2504-153">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="e2504-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="e2504-154">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2504-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e2504-155">policyType</span><span class="sxs-lookup"><span data-stu-id="e2504-155">policyType</span></span>|[<span data-ttu-id="e2504-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="e2504-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="e2504-157">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="e2504-157">Specifies the type of group policy.</span></span> <span data-ttu-id="e2504-158">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e2504-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="e2504-159">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="e2504-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="e2504-160">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="e2504-160">groupPolicyCategoryId</span></span>|<span data-ttu-id="e2504-161">Guid</span><span class="sxs-lookup"><span data-stu-id="e2504-161">Guid</span></span>|<span data-ttu-id="e2504-162">父类别的类别 ID 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2504-162">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e2504-163">id</span><span class="sxs-lookup"><span data-stu-id="e2504-163">id</span></span>|<span data-ttu-id="e2504-164">String</span><span class="sxs-lookup"><span data-stu-id="e2504-164">String</span></span>|<span data-ttu-id="e2504-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e2504-165">Key of the entity.</span></span> <span data-ttu-id="e2504-166">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2504-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="e2504-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2504-167">lastModifiedDateTime</span></span>|<span data-ttu-id="e2504-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2504-168">DateTimeOffset</span></span>|<span data-ttu-id="e2504-169">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2504-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="e2504-170">继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2504-170">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e2504-171">响应</span><span class="sxs-lookup"><span data-stu-id="e2504-171">Response</span></span>
<span data-ttu-id="e2504-172">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2504-172">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2504-173">示例</span><span class="sxs-lookup"><span data-stu-id="e2504-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2504-174">请求</span><span class="sxs-lookup"><span data-stu-id="e2504-174">Request</span></span>
<span data-ttu-id="e2504-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2504-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2504-176">响应</span><span class="sxs-lookup"><span data-stu-id="e2504-176">Response</span></span>
<span data-ttu-id="e2504-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2504-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




