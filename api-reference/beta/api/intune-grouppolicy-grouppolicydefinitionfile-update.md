---
title: 更新 groupPolicyDefinitionFile
description: 更新 groupPolicyDefinitionFile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 130e66b47459958cbc32c2e9b64e2968018825cd
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576387"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="34d7e-103">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="34d7e-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="34d7e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34d7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34d7e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34d7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34d7e-106">更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="34d7e-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34d7e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="34d7e-107">Prerequisites</span></span>
<span data-ttu-id="34d7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34d7e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34d7e-110">Permission type</span></span>|<span data-ttu-id="34d7e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34d7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34d7e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34d7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34d7e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34d7e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="34d7e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34d7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34d7e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="34d7e-115">Not supported.</span></span>|
|<span data-ttu-id="34d7e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="34d7e-116">Application</span></span>|<span data-ttu-id="34d7e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="34d7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34d7e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34d7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="34d7e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="34d7e-119">Request headers</span></span>
|<span data-ttu-id="34d7e-120">标头</span><span class="sxs-lookup"><span data-stu-id="34d7e-120">Header</span></span>|<span data-ttu-id="34d7e-121">值</span><span class="sxs-lookup"><span data-stu-id="34d7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34d7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34d7e-122">Authorization</span></span>|<span data-ttu-id="34d7e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34d7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34d7e-124">接受</span><span class="sxs-lookup"><span data-stu-id="34d7e-124">Accept</span></span>|<span data-ttu-id="34d7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34d7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34d7e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="34d7e-126">Request body</span></span>
<span data-ttu-id="34d7e-127">在请求正文中, 提供[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34d7e-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="34d7e-128">下表显示创建[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="34d7e-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="34d7e-129">属性</span><span class="sxs-lookup"><span data-stu-id="34d7e-129">Property</span></span>|<span data-ttu-id="34d7e-130">类型</span><span class="sxs-lookup"><span data-stu-id="34d7e-130">Type</span></span>|<span data-ttu-id="34d7e-131">说明</span><span class="sxs-lookup"><span data-stu-id="34d7e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34d7e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="34d7e-132">displayName</span></span>|<span data-ttu-id="34d7e-133">String</span><span class="sxs-lookup"><span data-stu-id="34d7e-133">String</span></span>|<span data-ttu-id="34d7e-134">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="34d7e-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="34d7e-135">说明</span><span class="sxs-lookup"><span data-stu-id="34d7e-135">description</span></span>|<span data-ttu-id="34d7e-136">String</span><span class="sxs-lookup"><span data-stu-id="34d7e-136">String</span></span>|<span data-ttu-id="34d7e-137">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="34d7e-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="34d7e-138">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="34d7e-138">The default value is empty.</span></span>|
|<span data-ttu-id="34d7e-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="34d7e-139">languageCodes</span></span>|<span data-ttu-id="34d7e-140">String collection</span><span class="sxs-lookup"><span data-stu-id="34d7e-140">String collection</span></span>|<span data-ttu-id="34d7e-141">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="34d7e-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="34d7e-142">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="34d7e-142">targetPrefix</span></span>|<span data-ttu-id="34d7e-143">String</span><span class="sxs-lookup"><span data-stu-id="34d7e-143">String</span></span>|<span data-ttu-id="34d7e-144">指定在 ADMX 文件中引用命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="34d7e-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="34d7e-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="34d7e-145">targetNamespace</span></span>|<span data-ttu-id="34d7e-146">String</span><span class="sxs-lookup"><span data-stu-id="34d7e-146">String</span></span>|<span data-ttu-id="34d7e-147">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="34d7e-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="34d7e-148">policyType</span><span class="sxs-lookup"><span data-stu-id="34d7e-148">policyType</span></span>|[<span data-ttu-id="34d7e-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="34d7e-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="34d7e-150">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="34d7e-150">Specifies the type of group policy.</span></span> <span data-ttu-id="34d7e-151">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="34d7e-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="34d7e-152">a01</span><span class="sxs-lookup"><span data-stu-id="34d7e-152">revision</span></span>|<span data-ttu-id="34d7e-153">String</span><span class="sxs-lookup"><span data-stu-id="34d7e-153">String</span></span>|<span data-ttu-id="34d7e-154">与文件关联的修订版本。</span><span class="sxs-lookup"><span data-stu-id="34d7e-154">The revision version associated with the file.</span></span>|
|<span data-ttu-id="34d7e-155">id</span><span class="sxs-lookup"><span data-stu-id="34d7e-155">id</span></span>|<span data-ttu-id="34d7e-156">字符串</span><span class="sxs-lookup"><span data-stu-id="34d7e-156">String</span></span>|<span data-ttu-id="34d7e-157">实体的键。</span><span class="sxs-lookup"><span data-stu-id="34d7e-157">Key of the entity.</span></span>|
|<span data-ttu-id="34d7e-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34d7e-158">lastModifiedDateTime</span></span>|<span data-ttu-id="34d7e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34d7e-159">DateTimeOffset</span></span>|<span data-ttu-id="34d7e-160">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="34d7e-160">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="34d7e-161">响应</span><span class="sxs-lookup"><span data-stu-id="34d7e-161">Response</span></span>
<span data-ttu-id="34d7e-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34d7e-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34d7e-163">示例</span><span class="sxs-lookup"><span data-stu-id="34d7e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="34d7e-164">请求</span><span class="sxs-lookup"><span data-stu-id="34d7e-164">Request</span></span>
<span data-ttu-id="34d7e-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34d7e-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34d7e-166">响应</span><span class="sxs-lookup"><span data-stu-id="34d7e-166">Response</span></span>
<span data-ttu-id="34d7e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34d7e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



