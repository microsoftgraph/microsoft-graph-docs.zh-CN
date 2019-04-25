---
title: 更新 groupPolicyDefinitionFile
description: 更新 groupPolicyDefinitionFile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 040b484a5e4f959fd6e4bbd35f2f08e66910d30c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531458"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="c24c2-103">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c24c2-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="c24c2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c24c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c24c2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c24c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c24c2-106">更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c24c2-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c24c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c24c2-107">Prerequisites</span></span>
<span data-ttu-id="c24c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c24c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c24c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c24c2-110">Permission type</span></span>|<span data-ttu-id="c24c2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c24c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c24c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c24c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c24c2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c24c2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c24c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c24c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c24c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c24c2-115">Not supported.</span></span>|
|<span data-ttu-id="c24c2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c24c2-116">Application</span></span>|<span data-ttu-id="c24c2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c24c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c24c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c24c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="c24c2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c24c2-119">Request headers</span></span>
|<span data-ttu-id="c24c2-120">标头</span><span class="sxs-lookup"><span data-stu-id="c24c2-120">Header</span></span>|<span data-ttu-id="c24c2-121">值</span><span class="sxs-lookup"><span data-stu-id="c24c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c24c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c24c2-122">Authorization</span></span>|<span data-ttu-id="c24c2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c24c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c24c2-124">接受</span><span class="sxs-lookup"><span data-stu-id="c24c2-124">Accept</span></span>|<span data-ttu-id="c24c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c24c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c24c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c24c2-126">Request body</span></span>
<span data-ttu-id="c24c2-127">在请求正文中, 提供[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c24c2-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="c24c2-128">下表显示创建[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c24c2-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="c24c2-129">属性</span><span class="sxs-lookup"><span data-stu-id="c24c2-129">Property</span></span>|<span data-ttu-id="c24c2-130">类型</span><span class="sxs-lookup"><span data-stu-id="c24c2-130">Type</span></span>|<span data-ttu-id="c24c2-131">说明</span><span class="sxs-lookup"><span data-stu-id="c24c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c24c2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c24c2-132">displayName</span></span>|<span data-ttu-id="c24c2-133">String</span><span class="sxs-lookup"><span data-stu-id="c24c2-133">String</span></span>|<span data-ttu-id="c24c2-134">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="c24c2-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="c24c2-135">description</span><span class="sxs-lookup"><span data-stu-id="c24c2-135">description</span></span>|<span data-ttu-id="c24c2-136">String</span><span class="sxs-lookup"><span data-stu-id="c24c2-136">String</span></span>|<span data-ttu-id="c24c2-137">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="c24c2-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="c24c2-138">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="c24c2-138">The default value is empty.</span></span>|
|<span data-ttu-id="c24c2-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="c24c2-139">languageCodes</span></span>|<span data-ttu-id="c24c2-140">String collection</span><span class="sxs-lookup"><span data-stu-id="c24c2-140">String collection</span></span>|<span data-ttu-id="c24c2-141">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="c24c2-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="c24c2-142">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="c24c2-142">targetPrefix</span></span>|<span data-ttu-id="c24c2-143">String</span><span class="sxs-lookup"><span data-stu-id="c24c2-143">String</span></span>|<span data-ttu-id="c24c2-144">指定在 ADMX 文件中引用命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="c24c2-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c24c2-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="c24c2-145">targetNamespace</span></span>|<span data-ttu-id="c24c2-146">String</span><span class="sxs-lookup"><span data-stu-id="c24c2-146">String</span></span>|<span data-ttu-id="c24c2-147">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="c24c2-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c24c2-148">policyType</span><span class="sxs-lookup"><span data-stu-id="c24c2-148">policyType</span></span>|[<span data-ttu-id="c24c2-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="c24c2-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c24c2-150">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="c24c2-150">Specifies the type of group policy.</span></span> <span data-ttu-id="c24c2-151">可能的值是：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="c24c2-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c24c2-152">id</span><span class="sxs-lookup"><span data-stu-id="c24c2-152">id</span></span>|<span data-ttu-id="c24c2-153">字符串</span><span class="sxs-lookup"><span data-stu-id="c24c2-153">String</span></span>|<span data-ttu-id="c24c2-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c24c2-154">Key of the entity.</span></span>|
|<span data-ttu-id="c24c2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c24c2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c24c2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c24c2-156">DateTimeOffset</span></span>|<span data-ttu-id="c24c2-157">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c24c2-157">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c24c2-158">响应</span><span class="sxs-lookup"><span data-stu-id="c24c2-158">Response</span></span>
<span data-ttu-id="c24c2-159">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c24c2-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c24c2-160">示例</span><span class="sxs-lookup"><span data-stu-id="c24c2-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c24c2-161">请求</span><span class="sxs-lookup"><span data-stu-id="c24c2-161">Request</span></span>
<span data-ttu-id="c24c2-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c24c2-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="c24c2-163">响应</span><span class="sxs-lookup"><span data-stu-id="c24c2-163">Response</span></span>
<span data-ttu-id="c24c2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c24c2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

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
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





