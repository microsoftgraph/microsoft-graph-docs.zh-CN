---
title: 更新 groupPolicyPresentationTextBox
description: 更新 groupPolicyPresentationTextBox 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b5b7ac370825c54c55ebdcfc0c219dd3916834a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789085"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="410b0-103">更新 groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="410b0-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="410b0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="410b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="410b0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="410b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="410b0-106">更新[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="410b0-106">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="410b0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="410b0-107">Prerequisites</span></span>
<span data-ttu-id="410b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="410b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="410b0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="410b0-110">Permission type</span></span>|<span data-ttu-id="410b0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="410b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="410b0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="410b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="410b0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="410b0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="410b0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="410b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="410b0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="410b0-115">Not supported.</span></span>|
|<span data-ttu-id="410b0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="410b0-116">Application</span></span>|<span data-ttu-id="410b0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="410b0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="410b0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="410b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="410b0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="410b0-119">Request headers</span></span>
|<span data-ttu-id="410b0-120">标头</span><span class="sxs-lookup"><span data-stu-id="410b0-120">Header</span></span>|<span data-ttu-id="410b0-121">值</span><span class="sxs-lookup"><span data-stu-id="410b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="410b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="410b0-122">Authorization</span></span>|<span data-ttu-id="410b0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="410b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="410b0-124">接受</span><span class="sxs-lookup"><span data-stu-id="410b0-124">Accept</span></span>|<span data-ttu-id="410b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="410b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="410b0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="410b0-126">Request body</span></span>
<span data-ttu-id="410b0-127">在请求正文中, 提供[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="410b0-127">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="410b0-128">下表显示创建[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="410b0-128">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="410b0-129">属性</span><span class="sxs-lookup"><span data-stu-id="410b0-129">Property</span></span>|<span data-ttu-id="410b0-130">类型</span><span class="sxs-lookup"><span data-stu-id="410b0-130">Type</span></span>|<span data-ttu-id="410b0-131">说明</span><span class="sxs-lookup"><span data-stu-id="410b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="410b0-132">label</span><span class="sxs-lookup"><span data-stu-id="410b0-132">label</span></span>|<span data-ttu-id="410b0-133">String</span><span class="sxs-lookup"><span data-stu-id="410b0-133">String</span></span>|<span data-ttu-id="410b0-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="410b0-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="410b0-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="410b0-135">The default value is empty.</span></span> <span data-ttu-id="410b0-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="410b0-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="410b0-137">id</span><span class="sxs-lookup"><span data-stu-id="410b0-137">id</span></span>|<span data-ttu-id="410b0-138">String</span><span class="sxs-lookup"><span data-stu-id="410b0-138">String</span></span>|<span data-ttu-id="410b0-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="410b0-139">Key of the entity.</span></span> <span data-ttu-id="410b0-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="410b0-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="410b0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="410b0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="410b0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="410b0-142">DateTimeOffset</span></span>|<span data-ttu-id="410b0-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="410b0-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="410b0-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="410b0-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="410b0-145">默认</span><span class="sxs-lookup"><span data-stu-id="410b0-145">defaultValue</span></span>|<span data-ttu-id="410b0-146">String</span><span class="sxs-lookup"><span data-stu-id="410b0-146">String</span></span>|<span data-ttu-id="410b0-147">显示在文本框中的本地化默认字符串。</span><span class="sxs-lookup"><span data-stu-id="410b0-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="410b0-148">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="410b0-148">The default value is empty.</span></span>|
|<span data-ttu-id="410b0-149">必需</span><span class="sxs-lookup"><span data-stu-id="410b0-149">required</span></span>|<span data-ttu-id="410b0-150">布尔值</span><span class="sxs-lookup"><span data-stu-id="410b0-150">Boolean</span></span>|<span data-ttu-id="410b0-151">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="410b0-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="410b0-152">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="410b0-152">Default value is false.</span></span>|
|<span data-ttu-id="410b0-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="410b0-153">maxLength</span></span>|<span data-ttu-id="410b0-154">Int64</span><span class="sxs-lookup"><span data-stu-id="410b0-154">Int64</span></span>|<span data-ttu-id="410b0-155">一个无符号整数, 指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="410b0-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="410b0-156">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="410b0-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="410b0-157">响应</span><span class="sxs-lookup"><span data-stu-id="410b0-157">Response</span></span>
<span data-ttu-id="410b0-158">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="410b0-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="410b0-159">示例</span><span class="sxs-lookup"><span data-stu-id="410b0-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="410b0-160">请求</span><span class="sxs-lookup"><span data-stu-id="410b0-160">Request</span></span>
<span data-ttu-id="410b0-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="410b0-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="410b0-162">响应</span><span class="sxs-lookup"><span data-stu-id="410b0-162">Response</span></span>
<span data-ttu-id="410b0-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="410b0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```





