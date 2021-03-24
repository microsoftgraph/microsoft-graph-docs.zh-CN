---
title: 创建 groupPolicyUploadedDefinitionFile
description: 创建新的 groupPolicyUploadedDefinitionFile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b414eeb1211af6ff9f6683d021f74c3be0d48d79
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145724"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a><span data-ttu-id="9b700-103">创建 groupPolicyUploadedDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="9b700-103">Create groupPolicyUploadedDefinitionFile</span></span>

<span data-ttu-id="9b700-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b700-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b700-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b700-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b700-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b700-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b700-107">创建新的 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b700-107">Create a new [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b700-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9b700-108">Prerequisites</span></span>
<span data-ttu-id="9b700-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b700-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b700-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b700-111">Permission type</span></span>|<span data-ttu-id="9b700-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b700-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b700-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b700-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b700-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b700-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b700-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b700-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b700-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b700-116">Not supported.</span></span>|
|<span data-ttu-id="9b700-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b700-117">Application</span></span>|<span data-ttu-id="9b700-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b700-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b700-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b700-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a><span data-ttu-id="9b700-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b700-120">Request headers</span></span>
|<span data-ttu-id="9b700-121">标头</span><span class="sxs-lookup"><span data-stu-id="9b700-121">Header</span></span>|<span data-ttu-id="9b700-122">值</span><span class="sxs-lookup"><span data-stu-id="9b700-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b700-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b700-123">Authorization</span></span>|<span data-ttu-id="9b700-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9b700-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b700-125">接受</span><span class="sxs-lookup"><span data-stu-id="9b700-125">Accept</span></span>|<span data-ttu-id="9b700-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b700-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b700-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b700-127">Request body</span></span>
<span data-ttu-id="9b700-128">在请求正文中，提供 groupPolicyUploadedDefinitionFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b700-128">In the request body, supply a JSON representation for the groupPolicyUploadedDefinitionFile object.</span></span>

<span data-ttu-id="9b700-129">下表显示创建 groupPolicyUploadedDefinitionFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9b700-129">The following table shows the properties that are required when you create the groupPolicyUploadedDefinitionFile.</span></span>

|<span data-ttu-id="9b700-130">属性</span><span class="sxs-lookup"><span data-stu-id="9b700-130">Property</span></span>|<span data-ttu-id="9b700-131">类型</span><span class="sxs-lookup"><span data-stu-id="9b700-131">Type</span></span>|<span data-ttu-id="9b700-132">说明</span><span class="sxs-lookup"><span data-stu-id="9b700-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b700-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9b700-133">displayName</span></span>|<span data-ttu-id="9b700-134">String</span><span class="sxs-lookup"><span data-stu-id="9b700-134">String</span></span>|<span data-ttu-id="9b700-135">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="9b700-135">The localized friendly name of the ADMX file.</span></span> <span data-ttu-id="9b700-136">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-136">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-137">说明</span><span class="sxs-lookup"><span data-stu-id="9b700-137">description</span></span>|<span data-ttu-id="9b700-138">String</span><span class="sxs-lookup"><span data-stu-id="9b700-138">String</span></span>|<span data-ttu-id="9b700-139">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="9b700-139">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="9b700-140">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="9b700-140">The default value is empty.</span></span> <span data-ttu-id="9b700-141">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-141">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-142">languageCodes</span><span class="sxs-lookup"><span data-stu-id="9b700-142">languageCodes</span></span>|<span data-ttu-id="9b700-143">String collection</span><span class="sxs-lookup"><span data-stu-id="9b700-143">String collection</span></span>|<span data-ttu-id="9b700-144">ADMX 文件支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="9b700-144">The supported language codes for the ADMX file.</span></span> <span data-ttu-id="9b700-145">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-145">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-146">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="9b700-146">targetPrefix</span></span>|<span data-ttu-id="9b700-147">String</span><span class="sxs-lookup"><span data-stu-id="9b700-147">String</span></span>|<span data-ttu-id="9b700-148">指定引用 ADMX 文件内的命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="9b700-148">Specifies the logical name that refers to the namespace within the ADMX file.</span></span> <span data-ttu-id="9b700-149">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-149">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-150">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="9b700-150">targetNamespace</span></span>|<span data-ttu-id="9b700-151">String</span><span class="sxs-lookup"><span data-stu-id="9b700-151">String</span></span>|<span data-ttu-id="9b700-152">指定用于标识 ADMX 文件内的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="9b700-152">Specifies the URI used to identify the namespace within the ADMX file.</span></span> <span data-ttu-id="9b700-153">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-153">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-154">policyType</span><span class="sxs-lookup"><span data-stu-id="9b700-154">policyType</span></span>|[<span data-ttu-id="9b700-155">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="9b700-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9b700-156">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="9b700-156">Specifies the type of group policy.</span></span> <span data-ttu-id="9b700-157">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)。</span><span class="sxs-lookup"><span data-stu-id="9b700-157">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span> <span data-ttu-id="9b700-158">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="9b700-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9b700-159">revision</span><span class="sxs-lookup"><span data-stu-id="9b700-159">revision</span></span>|<span data-ttu-id="9b700-160">String</span><span class="sxs-lookup"><span data-stu-id="9b700-160">String</span></span>|<span data-ttu-id="9b700-161">与文件关联的修订版本。</span><span class="sxs-lookup"><span data-stu-id="9b700-161">The revision version associated with the file.</span></span> <span data-ttu-id="9b700-162">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-162">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-163">id</span><span class="sxs-lookup"><span data-stu-id="9b700-163">id</span></span>|<span data-ttu-id="9b700-164">String</span><span class="sxs-lookup"><span data-stu-id="9b700-164">String</span></span>|<span data-ttu-id="9b700-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b700-165">Key of the entity.</span></span> <span data-ttu-id="9b700-166">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-166">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b700-167">lastModifiedDateTime</span></span>|<span data-ttu-id="9b700-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b700-168">DateTimeOffset</span></span>|<span data-ttu-id="9b700-169">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9b700-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="9b700-170">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="9b700-170">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="9b700-171">fileName</span><span class="sxs-lookup"><span data-stu-id="9b700-171">fileName</span></span>|<span data-ttu-id="9b700-172">String</span><span class="sxs-lookup"><span data-stu-id="9b700-172">String</span></span>|<span data-ttu-id="9b700-173">已上载的 ADML 文件的文件名。</span><span class="sxs-lookup"><span data-stu-id="9b700-173">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="9b700-174">状态</span><span class="sxs-lookup"><span data-stu-id="9b700-174">status</span></span>|[<span data-ttu-id="9b700-175">groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="9b700-175">groupPolicyUploadedDefinitionFileStatus</span></span>](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|<span data-ttu-id="9b700-176">已上载的 ADMX 文件的上载状态。</span><span class="sxs-lookup"><span data-stu-id="9b700-176">The upload status of the uploaded ADMX file.</span></span> <span data-ttu-id="9b700-177">可取值为：`none`、`uploadInProgress`、`available`、`assigned`、`removalInProgress`、`uploadFailed` 或 `removalFailed`。</span><span class="sxs-lookup"><span data-stu-id="9b700-177">Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span></span>|
|<span data-ttu-id="9b700-178">content</span><span class="sxs-lookup"><span data-stu-id="9b700-178">content</span></span>|<span data-ttu-id="9b700-179">Binary</span><span class="sxs-lookup"><span data-stu-id="9b700-179">Binary</span></span>|<span data-ttu-id="9b700-180">上载的 ADMX 文件的内容。</span><span class="sxs-lookup"><span data-stu-id="9b700-180">The contents of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="9b700-181">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="9b700-181">uploadDateTime</span></span>|<span data-ttu-id="9b700-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b700-182">DateTimeOffset</span></span>|<span data-ttu-id="9b700-183">上传的 ADMX 文件的上传时间。</span><span class="sxs-lookup"><span data-stu-id="9b700-183">The uploaded time of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="9b700-184">defaultLanguageCode</span><span class="sxs-lookup"><span data-stu-id="9b700-184">defaultLanguageCode</span></span>|<span data-ttu-id="9b700-185">String</span><span class="sxs-lookup"><span data-stu-id="9b700-185">String</span></span>|<span data-ttu-id="9b700-186">上载的 ADMX 文件的默认语言。</span><span class="sxs-lookup"><span data-stu-id="9b700-186">The default language of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="9b700-187">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="9b700-187">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="9b700-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9b700-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="9b700-189">与上载的 ADMX 文件关联的 ADML 文件列表。</span><span class="sxs-lookup"><span data-stu-id="9b700-189">The list of ADML files associated with the uploaded ADMX file.</span></span>|



## <a name="response"></a><span data-ttu-id="9b700-190">响应</span><span class="sxs-lookup"><span data-stu-id="9b700-190">Response</span></span>
<span data-ttu-id="9b700-191">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b700-191">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b700-192">示例</span><span class="sxs-lookup"><span data-stu-id="9b700-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b700-193">请求</span><span class="sxs-lookup"><span data-stu-id="9b700-193">Request</span></span>
<span data-ttu-id="9b700-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b700-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
Content-type: application/json
Content-length: 922

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9b700-195">响应</span><span class="sxs-lookup"><span data-stu-id="9b700-195">Response</span></span>
<span data-ttu-id="9b700-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b700-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1035

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "0ce1a8cf-a8cf-0ce1-cfa8-e10ccfa8e10c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




