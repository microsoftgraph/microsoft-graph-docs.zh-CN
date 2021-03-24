---
title: 创建 groupPolicyPresentationMultiTextBox
description: 创建新的 groupPolicyPresentationMultiTextBox 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b633e6b08a06a46be5db297b92a52abe8663422a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149553"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="770f0-103">创建 groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="770f0-103">Create groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="770f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="770f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="770f0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="770f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="770f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="770f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="770f0-107">创建新的 [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="770f0-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="770f0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="770f0-108">Prerequisites</span></span>
<span data-ttu-id="770f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="770f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="770f0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="770f0-111">Permission type</span></span>|<span data-ttu-id="770f0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="770f0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="770f0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="770f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="770f0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="770f0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="770f0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="770f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="770f0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="770f0-116">Not supported.</span></span>|
|<span data-ttu-id="770f0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="770f0-117">Application</span></span>|<span data-ttu-id="770f0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="770f0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="770f0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="770f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="770f0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="770f0-120">Request headers</span></span>
|<span data-ttu-id="770f0-121">标头</span><span class="sxs-lookup"><span data-stu-id="770f0-121">Header</span></span>|<span data-ttu-id="770f0-122">值</span><span class="sxs-lookup"><span data-stu-id="770f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="770f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="770f0-123">Authorization</span></span>|<span data-ttu-id="770f0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="770f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="770f0-125">接受</span><span class="sxs-lookup"><span data-stu-id="770f0-125">Accept</span></span>|<span data-ttu-id="770f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="770f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="770f0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="770f0-127">Request body</span></span>
<span data-ttu-id="770f0-128">在请求正文中，提供 groupPolicyPresentationMultiTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="770f0-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="770f0-129">下表显示创建 groupPolicyPresentationMultiTextBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="770f0-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="770f0-130">属性</span><span class="sxs-lookup"><span data-stu-id="770f0-130">Property</span></span>|<span data-ttu-id="770f0-131">类型</span><span class="sxs-lookup"><span data-stu-id="770f0-131">Type</span></span>|<span data-ttu-id="770f0-132">说明</span><span class="sxs-lookup"><span data-stu-id="770f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="770f0-133">label</span><span class="sxs-lookup"><span data-stu-id="770f0-133">label</span></span>|<span data-ttu-id="770f0-134">String</span><span class="sxs-lookup"><span data-stu-id="770f0-134">String</span></span>|<span data-ttu-id="770f0-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="770f0-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="770f0-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="770f0-136">The default value is empty.</span></span> <span data-ttu-id="770f0-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="770f0-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="770f0-138">id</span><span class="sxs-lookup"><span data-stu-id="770f0-138">id</span></span>|<span data-ttu-id="770f0-139">String</span><span class="sxs-lookup"><span data-stu-id="770f0-139">String</span></span>|<span data-ttu-id="770f0-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="770f0-140">Key of the entity.</span></span> <span data-ttu-id="770f0-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="770f0-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="770f0-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="770f0-142">lastModifiedDateTime</span></span>|<span data-ttu-id="770f0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="770f0-143">DateTimeOffset</span></span>|<span data-ttu-id="770f0-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="770f0-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="770f0-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="770f0-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="770f0-146">必需</span><span class="sxs-lookup"><span data-stu-id="770f0-146">required</span></span>|<span data-ttu-id="770f0-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="770f0-147">Boolean</span></span>|<span data-ttu-id="770f0-148">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="770f0-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="770f0-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="770f0-149">Default value is false.</span></span>|
|<span data-ttu-id="770f0-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="770f0-150">maxLength</span></span>|<span data-ttu-id="770f0-151">Int64</span><span class="sxs-lookup"><span data-stu-id="770f0-151">Int64</span></span>|<span data-ttu-id="770f0-152">一个无符号整数，指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="770f0-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="770f0-153">默认值为 1023。</span><span class="sxs-lookup"><span data-stu-id="770f0-153">Default value is 1023.</span></span>|
|<span data-ttu-id="770f0-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="770f0-154">maxStrings</span></span>|<span data-ttu-id="770f0-155">Int64</span><span class="sxs-lookup"><span data-stu-id="770f0-155">Int64</span></span>|<span data-ttu-id="770f0-156">一个无符号整数，指定字符串的最大数目。</span><span class="sxs-lookup"><span data-stu-id="770f0-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="770f0-157">默认值为 0 。</span><span class="sxs-lookup"><span data-stu-id="770f0-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="770f0-158">响应</span><span class="sxs-lookup"><span data-stu-id="770f0-158">Response</span></span>
<span data-ttu-id="770f0-159">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="770f0-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="770f0-160">示例</span><span class="sxs-lookup"><span data-stu-id="770f0-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="770f0-161">请求</span><span class="sxs-lookup"><span data-stu-id="770f0-161">Request</span></span>
<span data-ttu-id="770f0-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="770f0-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="770f0-163">响应</span><span class="sxs-lookup"><span data-stu-id="770f0-163">Response</span></span>
<span data-ttu-id="770f0-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="770f0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




