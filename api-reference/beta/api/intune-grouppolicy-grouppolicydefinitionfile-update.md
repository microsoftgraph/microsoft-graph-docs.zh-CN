---
title: 更新 groupPolicyDefinitionFile
description: 更新 groupPolicyDefinitionFile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0910406f564f86decf211285ed472f57792267c5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158890"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="c88dc-103">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c88dc-103">Update groupPolicyDefinitionFile</span></span>

<span data-ttu-id="c88dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c88dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c88dc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c88dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c88dc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c88dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c88dc-107">更新 [groupPolicyDefinitionFile 对象](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c88dc-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c88dc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c88dc-108">Prerequisites</span></span>
<span data-ttu-id="c88dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c88dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c88dc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c88dc-111">Permission type</span></span>|<span data-ttu-id="c88dc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c88dc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c88dc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c88dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c88dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c88dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c88dc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c88dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c88dc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c88dc-116">Not supported.</span></span>|
|<span data-ttu-id="c88dc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c88dc-117">Application</span></span>|<span data-ttu-id="c88dc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c88dc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c88dc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c88dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="c88dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c88dc-120">Request headers</span></span>
|<span data-ttu-id="c88dc-121">标头</span><span class="sxs-lookup"><span data-stu-id="c88dc-121">Header</span></span>|<span data-ttu-id="c88dc-122">值</span><span class="sxs-lookup"><span data-stu-id="c88dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c88dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c88dc-123">Authorization</span></span>|<span data-ttu-id="c88dc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c88dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c88dc-125">接受</span><span class="sxs-lookup"><span data-stu-id="c88dc-125">Accept</span></span>|<span data-ttu-id="c88dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c88dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c88dc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c88dc-127">Request body</span></span>
<span data-ttu-id="c88dc-128">在请求正文中，提供 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c88dc-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="c88dc-129">下表显示创建 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c88dc-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="c88dc-130">属性</span><span class="sxs-lookup"><span data-stu-id="c88dc-130">Property</span></span>|<span data-ttu-id="c88dc-131">类型</span><span class="sxs-lookup"><span data-stu-id="c88dc-131">Type</span></span>|<span data-ttu-id="c88dc-132">说明</span><span class="sxs-lookup"><span data-stu-id="c88dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c88dc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c88dc-133">displayName</span></span>|<span data-ttu-id="c88dc-134">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-134">String</span></span>|<span data-ttu-id="c88dc-135">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="c88dc-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="c88dc-136">说明</span><span class="sxs-lookup"><span data-stu-id="c88dc-136">description</span></span>|<span data-ttu-id="c88dc-137">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-137">String</span></span>|<span data-ttu-id="c88dc-138">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="c88dc-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="c88dc-139">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="c88dc-139">The default value is empty.</span></span>|
|<span data-ttu-id="c88dc-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="c88dc-140">languageCodes</span></span>|<span data-ttu-id="c88dc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c88dc-141">String collection</span></span>|<span data-ttu-id="c88dc-142">ADMX 文件支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="c88dc-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="c88dc-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="c88dc-143">targetPrefix</span></span>|<span data-ttu-id="c88dc-144">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-144">String</span></span>|<span data-ttu-id="c88dc-145">指定引用 ADMX 文件内的命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="c88dc-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c88dc-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="c88dc-146">targetNamespace</span></span>|<span data-ttu-id="c88dc-147">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-147">String</span></span>|<span data-ttu-id="c88dc-148">指定用于标识 ADMX 文件内的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="c88dc-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c88dc-149">policyType</span><span class="sxs-lookup"><span data-stu-id="c88dc-149">policyType</span></span>|[<span data-ttu-id="c88dc-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="c88dc-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c88dc-151">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="c88dc-151">Specifies the type of group policy.</span></span> <span data-ttu-id="c88dc-152">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="c88dc-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c88dc-153">revision</span><span class="sxs-lookup"><span data-stu-id="c88dc-153">revision</span></span>|<span data-ttu-id="c88dc-154">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-154">String</span></span>|<span data-ttu-id="c88dc-155">与文件关联的修订版本。</span><span class="sxs-lookup"><span data-stu-id="c88dc-155">The revision version associated with the file.</span></span>|
|<span data-ttu-id="c88dc-156">id</span><span class="sxs-lookup"><span data-stu-id="c88dc-156">id</span></span>|<span data-ttu-id="c88dc-157">String</span><span class="sxs-lookup"><span data-stu-id="c88dc-157">String</span></span>|<span data-ttu-id="c88dc-158">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c88dc-158">Key of the entity.</span></span>|
|<span data-ttu-id="c88dc-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c88dc-159">lastModifiedDateTime</span></span>|<span data-ttu-id="c88dc-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c88dc-160">DateTimeOffset</span></span>|<span data-ttu-id="c88dc-161">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c88dc-161">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c88dc-162">响应</span><span class="sxs-lookup"><span data-stu-id="c88dc-162">Response</span></span>
<span data-ttu-id="c88dc-163">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c88dc-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c88dc-164">示例</span><span class="sxs-lookup"><span data-stu-id="c88dc-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c88dc-165">请求</span><span class="sxs-lookup"><span data-stu-id="c88dc-165">Request</span></span>
<span data-ttu-id="c88dc-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c88dc-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value"
}
```

### <a name="response"></a><span data-ttu-id="c88dc-167">响应</span><span class="sxs-lookup"><span data-stu-id="c88dc-167">Response</span></span>
<span data-ttu-id="c88dc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c88dc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




