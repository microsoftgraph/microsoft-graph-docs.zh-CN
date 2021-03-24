---
title: 更新 groupPolicyDefinition
description: 更新 groupPolicyDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40012449a86324874251588dad27021e3e38fcec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145745"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="b4de8-103">更新 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="b4de8-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="b4de8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4de8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4de8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4de8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4de8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4de8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4de8-107">更新 [groupPolicyDefinition 对象](../resources/intune-grouppolicy-grouppolicydefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b4de8-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4de8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4de8-108">Prerequisites</span></span>
<span data-ttu-id="b4de8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4de8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4de8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4de8-111">Permission type</span></span>|<span data-ttu-id="b4de8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4de8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4de8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4de8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4de8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4de8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4de8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4de8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4de8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4de8-116">Not supported.</span></span>|
|<span data-ttu-id="b4de8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4de8-117">Application</span></span>|<span data-ttu-id="b4de8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4de8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4de8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4de8-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b4de8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4de8-120">Request headers</span></span>
|<span data-ttu-id="b4de8-121">标头</span><span class="sxs-lookup"><span data-stu-id="b4de8-121">Header</span></span>|<span data-ttu-id="b4de8-122">值</span><span class="sxs-lookup"><span data-stu-id="b4de8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4de8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4de8-123">Authorization</span></span>|<span data-ttu-id="b4de8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4de8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4de8-125">接受</span><span class="sxs-lookup"><span data-stu-id="b4de8-125">Accept</span></span>|<span data-ttu-id="b4de8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4de8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4de8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4de8-127">Request body</span></span>
<span data-ttu-id="b4de8-128">在请求正文中，提供 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4de8-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="b4de8-129">下表显示创建 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b4de8-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="b4de8-130">属性</span><span class="sxs-lookup"><span data-stu-id="b4de8-130">Property</span></span>|<span data-ttu-id="b4de8-131">类型</span><span class="sxs-lookup"><span data-stu-id="b4de8-131">Type</span></span>|<span data-ttu-id="b4de8-132">说明</span><span class="sxs-lookup"><span data-stu-id="b4de8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4de8-133">classType</span><span class="sxs-lookup"><span data-stu-id="b4de8-133">classType</span></span>|[<span data-ttu-id="b4de8-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="b4de8-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="b4de8-135">标识策略可应用于的组类型。</span><span class="sxs-lookup"><span data-stu-id="b4de8-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="b4de8-136">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="b4de8-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="b4de8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b4de8-137">displayName</span></span>|<span data-ttu-id="b4de8-138">String</span><span class="sxs-lookup"><span data-stu-id="b4de8-138">String</span></span>|<span data-ttu-id="b4de8-139">本地化的策略名称。</span><span class="sxs-lookup"><span data-stu-id="b4de8-139">The localized policy name.</span></span>|
|<span data-ttu-id="b4de8-140">explainText</span><span class="sxs-lookup"><span data-stu-id="b4de8-140">explainText</span></span>|<span data-ttu-id="b4de8-141">String</span><span class="sxs-lookup"><span data-stu-id="b4de8-141">String</span></span>|<span data-ttu-id="b4de8-142">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="b4de8-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="b4de8-143">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="b4de8-143">The default value is empty.</span></span>|
|<span data-ttu-id="b4de8-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="b4de8-144">categoryPath</span></span>|<span data-ttu-id="b4de8-145">String</span><span class="sxs-lookup"><span data-stu-id="b4de8-145">String</span></span>|<span data-ttu-id="b4de8-146">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="b4de8-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="b4de8-147">supportedOn</span><span class="sxs-lookup"><span data-stu-id="b4de8-147">supportedOn</span></span>|<span data-ttu-id="b4de8-148">String</span><span class="sxs-lookup"><span data-stu-id="b4de8-148">String</span></span>|<span data-ttu-id="b4de8-149">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="b4de8-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="b4de8-150">policyType</span><span class="sxs-lookup"><span data-stu-id="b4de8-150">policyType</span></span>|[<span data-ttu-id="b4de8-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="b4de8-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="b4de8-152">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="b4de8-152">Specifies the type of group policy.</span></span> <span data-ttu-id="b4de8-153">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="b4de8-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="b4de8-154">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="b4de8-154">groupPolicyCategoryId</span></span>|<span data-ttu-id="b4de8-155">Guid</span><span class="sxs-lookup"><span data-stu-id="b4de8-155">Guid</span></span>|<span data-ttu-id="b4de8-156">父类别的类别 ID</span><span class="sxs-lookup"><span data-stu-id="b4de8-156">The category id of the parent category</span></span>|
|<span data-ttu-id="b4de8-157">id</span><span class="sxs-lookup"><span data-stu-id="b4de8-157">id</span></span>|<span data-ttu-id="b4de8-158">String</span><span class="sxs-lookup"><span data-stu-id="b4de8-158">String</span></span>|<span data-ttu-id="b4de8-159">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b4de8-159">Key of the entity.</span></span>|
|<span data-ttu-id="b4de8-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4de8-160">lastModifiedDateTime</span></span>|<span data-ttu-id="b4de8-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4de8-161">DateTimeOffset</span></span>|<span data-ttu-id="b4de8-162">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4de8-162">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b4de8-163">响应</span><span class="sxs-lookup"><span data-stu-id="b4de8-163">Response</span></span>
<span data-ttu-id="b4de8-164">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4de8-164">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4de8-165">示例</span><span class="sxs-lookup"><span data-stu-id="b4de8-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4de8-166">请求</span><span class="sxs-lookup"><span data-stu-id="b4de8-166">Request</span></span>
<span data-ttu-id="b4de8-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4de8-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 353

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d"
}
```

### <a name="response"></a><span data-ttu-id="b4de8-168">响应</span><span class="sxs-lookup"><span data-stu-id="b4de8-168">Response</span></span>
<span data-ttu-id="b4de8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4de8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 466

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




