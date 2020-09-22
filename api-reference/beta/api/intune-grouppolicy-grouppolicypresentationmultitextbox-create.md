---
title: 创建 groupPolicyPresentationMultiTextBox
description: 创建新的 groupPolicyPresentationMultiTextBox 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dae2e6560fcfb7b5a95df31171437e1b388da6c5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065128"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="8f24c-103">创建 groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="8f24c-103">Create groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="8f24c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f24c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f24c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8f24c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f24c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f24c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f24c-107">创建新的 [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f24c-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f24c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f24c-108">Prerequisites</span></span>
<span data-ttu-id="8f24c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f24c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f24c-111">Permission type</span></span>|<span data-ttu-id="8f24c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f24c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f24c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f24c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f24c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f24c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f24c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f24c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f24c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f24c-116">Not supported.</span></span>|
|<span data-ttu-id="8f24c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f24c-117">Application</span></span>|<span data-ttu-id="8f24c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f24c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f24c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f24c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="8f24c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f24c-120">Request headers</span></span>
|<span data-ttu-id="8f24c-121">标头</span><span class="sxs-lookup"><span data-stu-id="8f24c-121">Header</span></span>|<span data-ttu-id="8f24c-122">值</span><span class="sxs-lookup"><span data-stu-id="8f24c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f24c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f24c-123">Authorization</span></span>|<span data-ttu-id="8f24c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f24c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f24c-125">接受</span><span class="sxs-lookup"><span data-stu-id="8f24c-125">Accept</span></span>|<span data-ttu-id="8f24c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f24c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f24c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f24c-127">Request body</span></span>
<span data-ttu-id="8f24c-128">在请求正文中，提供 groupPolicyPresentationMultiTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f24c-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="8f24c-129">下表显示创建 groupPolicyPresentationMultiTextBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8f24c-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="8f24c-130">属性</span><span class="sxs-lookup"><span data-stu-id="8f24c-130">Property</span></span>|<span data-ttu-id="8f24c-131">类型</span><span class="sxs-lookup"><span data-stu-id="8f24c-131">Type</span></span>|<span data-ttu-id="8f24c-132">说明</span><span class="sxs-lookup"><span data-stu-id="8f24c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f24c-133">label</span><span class="sxs-lookup"><span data-stu-id="8f24c-133">label</span></span>|<span data-ttu-id="8f24c-134">String</span><span class="sxs-lookup"><span data-stu-id="8f24c-134">String</span></span>|<span data-ttu-id="8f24c-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="8f24c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="8f24c-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="8f24c-136">The default value is empty.</span></span> <span data-ttu-id="8f24c-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8f24c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8f24c-138">id</span><span class="sxs-lookup"><span data-stu-id="8f24c-138">id</span></span>|<span data-ttu-id="8f24c-139">String</span><span class="sxs-lookup"><span data-stu-id="8f24c-139">String</span></span>|<span data-ttu-id="8f24c-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8f24c-140">Key of the entity.</span></span> <span data-ttu-id="8f24c-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8f24c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8f24c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f24c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="8f24c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f24c-143">DateTimeOffset</span></span>|<span data-ttu-id="8f24c-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8f24c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="8f24c-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8f24c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8f24c-146">必需</span><span class="sxs-lookup"><span data-stu-id="8f24c-146">required</span></span>|<span data-ttu-id="8f24c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f24c-147">Boolean</span></span>|<span data-ttu-id="8f24c-148">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="8f24c-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="8f24c-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="8f24c-149">Default value is false.</span></span>|
|<span data-ttu-id="8f24c-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="8f24c-150">maxLength</span></span>|<span data-ttu-id="8f24c-151">Int64</span><span class="sxs-lookup"><span data-stu-id="8f24c-151">Int64</span></span>|<span data-ttu-id="8f24c-152">一个无符号整数，指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="8f24c-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="8f24c-153">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="8f24c-153">Default value is 1023.</span></span>|
|<span data-ttu-id="8f24c-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="8f24c-154">maxStrings</span></span>|<span data-ttu-id="8f24c-155">Int64</span><span class="sxs-lookup"><span data-stu-id="8f24c-155">Int64</span></span>|<span data-ttu-id="8f24c-156">一个无符号整数，指定最大字符串数。</span><span class="sxs-lookup"><span data-stu-id="8f24c-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="8f24c-157">默认值为 0 。</span><span class="sxs-lookup"><span data-stu-id="8f24c-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="8f24c-158">响应</span><span class="sxs-lookup"><span data-stu-id="8f24c-158">Response</span></span>
<span data-ttu-id="8f24c-159">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f24c-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f24c-160">示例</span><span class="sxs-lookup"><span data-stu-id="8f24c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f24c-161">请求</span><span class="sxs-lookup"><span data-stu-id="8f24c-161">Request</span></span>
<span data-ttu-id="8f24c-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f24c-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f24c-163">响应</span><span class="sxs-lookup"><span data-stu-id="8f24c-163">Response</span></span>
<span data-ttu-id="8f24c-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f24c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






