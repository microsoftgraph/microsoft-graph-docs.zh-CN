---
title: 更新 groupPolicyDefinition
description: 更新 groupPolicyDefinition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f750e7f6a3bd631973fdeabc59011d0d07301cb4
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644291"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="596fe-103">更新 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="596fe-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="596fe-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="596fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="596fe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="596fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="596fe-106">更新[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="596fe-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="596fe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="596fe-107">Prerequisites</span></span>
<span data-ttu-id="596fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="596fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="596fe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="596fe-110">Permission type</span></span>|<span data-ttu-id="596fe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="596fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="596fe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="596fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="596fe-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="596fe-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="596fe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="596fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="596fe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="596fe-115">Not supported.</span></span>|
|<span data-ttu-id="596fe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="596fe-116">Application</span></span>|<span data-ttu-id="596fe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="596fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="596fe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="596fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="596fe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="596fe-119">Request headers</span></span>
|<span data-ttu-id="596fe-120">标头</span><span class="sxs-lookup"><span data-stu-id="596fe-120">Header</span></span>|<span data-ttu-id="596fe-121">值</span><span class="sxs-lookup"><span data-stu-id="596fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="596fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="596fe-122">Authorization</span></span>|<span data-ttu-id="596fe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="596fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="596fe-124">接受</span><span class="sxs-lookup"><span data-stu-id="596fe-124">Accept</span></span>|<span data-ttu-id="596fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="596fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="596fe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="596fe-126">Request body</span></span>
<span data-ttu-id="596fe-127">在请求正文中, 提供[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="596fe-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="596fe-128">下表显示创建[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="596fe-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="596fe-129">属性</span><span class="sxs-lookup"><span data-stu-id="596fe-129">Property</span></span>|<span data-ttu-id="596fe-130">类型</span><span class="sxs-lookup"><span data-stu-id="596fe-130">Type</span></span>|<span data-ttu-id="596fe-131">说明</span><span class="sxs-lookup"><span data-stu-id="596fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="596fe-132">classType</span><span class="sxs-lookup"><span data-stu-id="596fe-132">classType</span></span>|[<span data-ttu-id="596fe-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="596fe-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="596fe-134">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="596fe-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="596fe-135">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="596fe-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="596fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="596fe-136">displayName</span></span>|<span data-ttu-id="596fe-137">String</span><span class="sxs-lookup"><span data-stu-id="596fe-137">String</span></span>|<span data-ttu-id="596fe-138">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="596fe-138">The localized policy name.</span></span>|
|<span data-ttu-id="596fe-139">explainText</span><span class="sxs-lookup"><span data-stu-id="596fe-139">explainText</span></span>|<span data-ttu-id="596fe-140">字符串</span><span class="sxs-lookup"><span data-stu-id="596fe-140">String</span></span>|<span data-ttu-id="596fe-141">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="596fe-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="596fe-142">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="596fe-142">The default value is empty.</span></span>|
|<span data-ttu-id="596fe-143">categoryPath</span><span class="sxs-lookup"><span data-stu-id="596fe-143">categoryPath</span></span>|<span data-ttu-id="596fe-144">字符串</span><span class="sxs-lookup"><span data-stu-id="596fe-144">String</span></span>|<span data-ttu-id="596fe-145">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="596fe-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="596fe-146">supportedOn</span><span class="sxs-lookup"><span data-stu-id="596fe-146">supportedOn</span></span>|<span data-ttu-id="596fe-147">字符串</span><span class="sxs-lookup"><span data-stu-id="596fe-147">String</span></span>|<span data-ttu-id="596fe-148">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="596fe-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="596fe-149">policyType</span><span class="sxs-lookup"><span data-stu-id="596fe-149">policyType</span></span>|[<span data-ttu-id="596fe-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="596fe-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="596fe-151">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="596fe-151">Specifies the type of group policy.</span></span> <span data-ttu-id="596fe-152">可能的值是：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="596fe-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="596fe-153">id</span><span class="sxs-lookup"><span data-stu-id="596fe-153">id</span></span>|<span data-ttu-id="596fe-154">String</span><span class="sxs-lookup"><span data-stu-id="596fe-154">String</span></span>|<span data-ttu-id="596fe-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="596fe-155">Key of the entity.</span></span>|
|<span data-ttu-id="596fe-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="596fe-156">lastModifiedDateTime</span></span>|<span data-ttu-id="596fe-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="596fe-157">DateTimeOffset</span></span>|<span data-ttu-id="596fe-158">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="596fe-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="596fe-159">响应</span><span class="sxs-lookup"><span data-stu-id="596fe-159">Response</span></span>
<span data-ttu-id="596fe-160">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="596fe-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="596fe-161">示例</span><span class="sxs-lookup"><span data-stu-id="596fe-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="596fe-162">请求</span><span class="sxs-lookup"><span data-stu-id="596fe-162">Request</span></span>
<span data-ttu-id="596fe-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="596fe-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="596fe-164">响应</span><span class="sxs-lookup"><span data-stu-id="596fe-164">Response</span></span>
<span data-ttu-id="596fe-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="596fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




