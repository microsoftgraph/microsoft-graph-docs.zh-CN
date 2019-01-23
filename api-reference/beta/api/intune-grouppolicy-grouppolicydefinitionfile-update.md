---
title: 更新 groupPolicyDefinitionFile
description: 更新 groupPolicyDefinitionFile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be713dba2d503f19cd565fe5e53d252ed20667e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429495"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="6df1c-103">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="6df1c-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="6df1c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6df1c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6df1c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6df1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6df1c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6df1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6df1c-107">更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6df1c-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6df1c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6df1c-108">Prerequisites</span></span>
<span data-ttu-id="6df1c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6df1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6df1c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6df1c-111">Permission type</span></span>|<span data-ttu-id="6df1c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6df1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6df1c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6df1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6df1c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6df1c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6df1c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6df1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6df1c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6df1c-116">Not supported.</span></span>|
|<span data-ttu-id="6df1c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6df1c-117">Application</span></span>|<span data-ttu-id="6df1c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6df1c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6df1c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6df1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="6df1c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6df1c-120">Request headers</span></span>
|<span data-ttu-id="6df1c-121">标头</span><span class="sxs-lookup"><span data-stu-id="6df1c-121">Header</span></span>|<span data-ttu-id="6df1c-122">值</span><span class="sxs-lookup"><span data-stu-id="6df1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6df1c-123">授权</span><span class="sxs-lookup"><span data-stu-id="6df1c-123">Authorization</span></span>|<span data-ttu-id="6df1c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6df1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6df1c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6df1c-125">Accept</span></span>|<span data-ttu-id="6df1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6df1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6df1c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6df1c-127">Request body</span></span>
<span data-ttu-id="6df1c-128">在请求正文中，提供[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6df1c-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="6df1c-129">下表显示时创建[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6df1c-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="6df1c-130">属性</span><span class="sxs-lookup"><span data-stu-id="6df1c-130">Property</span></span>|<span data-ttu-id="6df1c-131">类型</span><span class="sxs-lookup"><span data-stu-id="6df1c-131">Type</span></span>|<span data-ttu-id="6df1c-132">说明</span><span class="sxs-lookup"><span data-stu-id="6df1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6df1c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6df1c-133">displayName</span></span>|<span data-ttu-id="6df1c-134">String</span><span class="sxs-lookup"><span data-stu-id="6df1c-134">String</span></span>|<span data-ttu-id="6df1c-135">ADMX 文件的本地化的友好名称。</span><span class="sxs-lookup"><span data-stu-id="6df1c-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="6df1c-136">说明</span><span class="sxs-lookup"><span data-stu-id="6df1c-136">description</span></span>|<span data-ttu-id="6df1c-137">String</span><span class="sxs-lookup"><span data-stu-id="6df1c-137">String</span></span>|<span data-ttu-id="6df1c-138">ADMX 文件中的策略设置的本地化的描述。</span><span class="sxs-lookup"><span data-stu-id="6df1c-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="6df1c-139">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="6df1c-139">The default value is empty.</span></span>|
|<span data-ttu-id="6df1c-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="6df1c-140">languageCodes</span></span>|<span data-ttu-id="6df1c-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="6df1c-141">String collection</span></span>|<span data-ttu-id="6df1c-142">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="6df1c-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="6df1c-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="6df1c-143">targetPrefix</span></span>|<span data-ttu-id="6df1c-144">String</span><span class="sxs-lookup"><span data-stu-id="6df1c-144">String</span></span>|<span data-ttu-id="6df1c-145">指定引用 ADMX 文件中的命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="6df1c-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="6df1c-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="6df1c-146">targetNamespace</span></span>|<span data-ttu-id="6df1c-147">String</span><span class="sxs-lookup"><span data-stu-id="6df1c-147">String</span></span>|<span data-ttu-id="6df1c-148">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="6df1c-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="6df1c-149">policyType</span><span class="sxs-lookup"><span data-stu-id="6df1c-149">policyType</span></span>|[<span data-ttu-id="6df1c-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="6df1c-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="6df1c-151">指定的组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="6df1c-151">Specifies the type of group policy.</span></span> <span data-ttu-id="6df1c-152">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="6df1c-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="6df1c-153">id</span><span class="sxs-lookup"><span data-stu-id="6df1c-153">id</span></span>|<span data-ttu-id="6df1c-154">String</span><span class="sxs-lookup"><span data-stu-id="6df1c-154">String</span></span>|<span data-ttu-id="6df1c-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6df1c-155">Key of the entity.</span></span>|
|<span data-ttu-id="6df1c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6df1c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6df1c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6df1c-157">DateTimeOffset</span></span>|<span data-ttu-id="6df1c-158">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="6df1c-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6df1c-159">响应</span><span class="sxs-lookup"><span data-stu-id="6df1c-159">Response</span></span>
<span data-ttu-id="6df1c-160">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6df1c-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6df1c-161">示例</span><span class="sxs-lookup"><span data-stu-id="6df1c-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="6df1c-162">请求</span><span class="sxs-lookup"><span data-stu-id="6df1c-162">Request</span></span>
<span data-ttu-id="6df1c-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6df1c-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6df1c-164">响应</span><span class="sxs-lookup"><span data-stu-id="6df1c-164">Response</span></span>
<span data-ttu-id="6df1c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6df1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




