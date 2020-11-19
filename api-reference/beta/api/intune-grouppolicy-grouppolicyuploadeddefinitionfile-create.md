---
title: 创建 groupPolicyUploadedDefinitionFile
description: 创建新的 groupPolicyUploadedDefinitionFile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4b390008b94ca56f24b7c0d5c2891dbf8b881bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224905"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a><span data-ttu-id="d2821-103">创建 groupPolicyUploadedDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="d2821-103">Create groupPolicyUploadedDefinitionFile</span></span>

<span data-ttu-id="d2821-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2821-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2821-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2821-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2821-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2821-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2821-107">创建新的 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2821-107">Create a new [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2821-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2821-108">Prerequisites</span></span>
<span data-ttu-id="d2821-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2821-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2821-111">Permission type</span></span>|<span data-ttu-id="d2821-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2821-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2821-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2821-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2821-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2821-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2821-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2821-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2821-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2821-116">Not supported.</span></span>|
|<span data-ttu-id="d2821-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2821-117">Application</span></span>|<span data-ttu-id="d2821-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2821-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2821-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2821-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a><span data-ttu-id="d2821-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2821-120">Request headers</span></span>
|<span data-ttu-id="d2821-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2821-121">Header</span></span>|<span data-ttu-id="d2821-122">值</span><span class="sxs-lookup"><span data-stu-id="d2821-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2821-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2821-123">Authorization</span></span>|<span data-ttu-id="d2821-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2821-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2821-125">接受</span><span class="sxs-lookup"><span data-stu-id="d2821-125">Accept</span></span>|<span data-ttu-id="d2821-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2821-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2821-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2821-127">Request body</span></span>
<span data-ttu-id="d2821-128">在请求正文中，提供 groupPolicyUploadedDefinitionFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2821-128">In the request body, supply a JSON representation for the groupPolicyUploadedDefinitionFile object.</span></span>

<span data-ttu-id="d2821-129">下表显示创建 groupPolicyUploadedDefinitionFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2821-129">The following table shows the properties that are required when you create the groupPolicyUploadedDefinitionFile.</span></span>

|<span data-ttu-id="d2821-130">属性</span><span class="sxs-lookup"><span data-stu-id="d2821-130">Property</span></span>|<span data-ttu-id="d2821-131">类型</span><span class="sxs-lookup"><span data-stu-id="d2821-131">Type</span></span>|<span data-ttu-id="d2821-132">说明</span><span class="sxs-lookup"><span data-stu-id="d2821-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2821-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d2821-133">displayName</span></span>|<span data-ttu-id="d2821-134">String</span><span class="sxs-lookup"><span data-stu-id="d2821-134">String</span></span>|<span data-ttu-id="d2821-135">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="d2821-135">The localized friendly name of the ADMX file.</span></span> <span data-ttu-id="d2821-136">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-136">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-137">description</span><span class="sxs-lookup"><span data-stu-id="d2821-137">description</span></span>|<span data-ttu-id="d2821-138">String</span><span class="sxs-lookup"><span data-stu-id="d2821-138">String</span></span>|<span data-ttu-id="d2821-139">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="d2821-139">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="d2821-140">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="d2821-140">The default value is empty.</span></span> <span data-ttu-id="d2821-141">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-141">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-142">languageCodes</span><span class="sxs-lookup"><span data-stu-id="d2821-142">languageCodes</span></span>|<span data-ttu-id="d2821-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="d2821-143">String collection</span></span>|<span data-ttu-id="d2821-144">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="d2821-144">The supported language codes for the ADMX file.</span></span> <span data-ttu-id="d2821-145">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-145">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-146">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="d2821-146">targetPrefix</span></span>|<span data-ttu-id="d2821-147">String</span><span class="sxs-lookup"><span data-stu-id="d2821-147">String</span></span>|<span data-ttu-id="d2821-148">指定在 ADMX 文件中引用命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="d2821-148">Specifies the logical name that refers to the namespace within the ADMX file.</span></span> <span data-ttu-id="d2821-149">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-149">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-150">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="d2821-150">targetNamespace</span></span>|<span data-ttu-id="d2821-151">String</span><span class="sxs-lookup"><span data-stu-id="d2821-151">String</span></span>|<span data-ttu-id="d2821-152">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="d2821-152">Specifies the URI used to identify the namespace within the ADMX file.</span></span> <span data-ttu-id="d2821-153">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-153">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-154">policyType</span><span class="sxs-lookup"><span data-stu-id="d2821-154">policyType</span></span>|[<span data-ttu-id="d2821-155">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="d2821-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="d2821-156">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="d2821-156">Specifies the type of group policy.</span></span> <span data-ttu-id="d2821-157">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)。</span><span class="sxs-lookup"><span data-stu-id="d2821-157">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span> <span data-ttu-id="d2821-158">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="d2821-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="d2821-159">a01</span><span class="sxs-lookup"><span data-stu-id="d2821-159">revision</span></span>|<span data-ttu-id="d2821-160">String</span><span class="sxs-lookup"><span data-stu-id="d2821-160">String</span></span>|<span data-ttu-id="d2821-161">与文件关联的修订版本。</span><span class="sxs-lookup"><span data-stu-id="d2821-161">The revision version associated with the file.</span></span> <span data-ttu-id="d2821-162">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-162">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-163">id</span><span class="sxs-lookup"><span data-stu-id="d2821-163">id</span></span>|<span data-ttu-id="d2821-164">String</span><span class="sxs-lookup"><span data-stu-id="d2821-164">String</span></span>|<span data-ttu-id="d2821-165">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2821-165">Key of the entity.</span></span> <span data-ttu-id="d2821-166">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-166">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2821-167">lastModifiedDateTime</span></span>|<span data-ttu-id="d2821-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2821-168">DateTimeOffset</span></span>|<span data-ttu-id="d2821-169">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d2821-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="d2821-170">继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="d2821-170">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="d2821-171">fileName</span><span class="sxs-lookup"><span data-stu-id="d2821-171">fileName</span></span>|<span data-ttu-id="d2821-172">String</span><span class="sxs-lookup"><span data-stu-id="d2821-172">String</span></span>|<span data-ttu-id="d2821-173">上传的 ADML 文件的文件名。</span><span class="sxs-lookup"><span data-stu-id="d2821-173">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="d2821-174">status</span><span class="sxs-lookup"><span data-stu-id="d2821-174">status</span></span>|[<span data-ttu-id="d2821-175">groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="d2821-175">groupPolicyUploadedDefinitionFileStatus</span></span>](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|<span data-ttu-id="d2821-176">已上载的 ADMX 文件的上载状态。</span><span class="sxs-lookup"><span data-stu-id="d2821-176">The upload status of the uploaded ADMX file.</span></span> <span data-ttu-id="d2821-177">可取值为：`none`、`uploadInProgress`、`available`、`assigned`、`removalInProgress`、`uploadFailed` 或 `removalFailed`。</span><span class="sxs-lookup"><span data-stu-id="d2821-177">Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span></span>|
|<span data-ttu-id="d2821-178">content</span><span class="sxs-lookup"><span data-stu-id="d2821-178">content</span></span>|<span data-ttu-id="d2821-179">Binary</span><span class="sxs-lookup"><span data-stu-id="d2821-179">Binary</span></span>|<span data-ttu-id="d2821-180">已上载的 ADMX 文件的内容。</span><span class="sxs-lookup"><span data-stu-id="d2821-180">The contents of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="d2821-181">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="d2821-181">uploadDateTime</span></span>|<span data-ttu-id="d2821-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2821-182">DateTimeOffset</span></span>|<span data-ttu-id="d2821-183">上载的 ADMX 文件的上载时间。</span><span class="sxs-lookup"><span data-stu-id="d2821-183">The uploaded time of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="d2821-184">defaultLanguageCode</span><span class="sxs-lookup"><span data-stu-id="d2821-184">defaultLanguageCode</span></span>|<span data-ttu-id="d2821-185">String</span><span class="sxs-lookup"><span data-stu-id="d2821-185">String</span></span>|<span data-ttu-id="d2821-186">上载的 ADMX 文件的默认语言。</span><span class="sxs-lookup"><span data-stu-id="d2821-186">The default language of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="d2821-187">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="d2821-187">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="d2821-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2821-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="d2821-189">与上载的 ADMX 文件关联的 ADML 文件的列表。</span><span class="sxs-lookup"><span data-stu-id="d2821-189">The list of ADML files associated with the uploaded ADMX file.</span></span>|



## <a name="response"></a><span data-ttu-id="d2821-190">响应</span><span class="sxs-lookup"><span data-stu-id="d2821-190">Response</span></span>
<span data-ttu-id="d2821-191">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2821-191">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2821-192">示例</span><span class="sxs-lookup"><span data-stu-id="d2821-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2821-193">请求</span><span class="sxs-lookup"><span data-stu-id="d2821-193">Request</span></span>
<span data-ttu-id="d2821-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2821-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d2821-195">响应</span><span class="sxs-lookup"><span data-stu-id="d2821-195">Response</span></span>
<span data-ttu-id="d2821-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2821-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




