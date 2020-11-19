---
title: 创建 groupPolicyPresentationMultiTextBox
description: 创建新的 groupPolicyPresentationMultiTextBox 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eec21e6d9f12004ea858869edd2e1cdc15f2a9bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49262831"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="11ba4-103">创建 groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="11ba4-103">Create groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="11ba4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11ba4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11ba4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11ba4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11ba4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11ba4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11ba4-107">创建新的 [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="11ba4-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11ba4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="11ba4-108">Prerequisites</span></span>
<span data-ttu-id="11ba4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11ba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11ba4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="11ba4-111">Permission type</span></span>|<span data-ttu-id="11ba4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="11ba4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11ba4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11ba4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11ba4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11ba4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11ba4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11ba4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11ba4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11ba4-116">Not supported.</span></span>|
|<span data-ttu-id="11ba4-117">Application</span><span class="sxs-lookup"><span data-stu-id="11ba4-117">Application</span></span>|<span data-ttu-id="11ba4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11ba4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11ba4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11ba4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="11ba4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="11ba4-120">Request headers</span></span>
|<span data-ttu-id="11ba4-121">标头</span><span class="sxs-lookup"><span data-stu-id="11ba4-121">Header</span></span>|<span data-ttu-id="11ba4-122">值</span><span class="sxs-lookup"><span data-stu-id="11ba4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11ba4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11ba4-123">Authorization</span></span>|<span data-ttu-id="11ba4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="11ba4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11ba4-125">接受</span><span class="sxs-lookup"><span data-stu-id="11ba4-125">Accept</span></span>|<span data-ttu-id="11ba4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11ba4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11ba4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="11ba4-127">Request body</span></span>
<span data-ttu-id="11ba4-128">在请求正文中，提供 groupPolicyPresentationMultiTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11ba4-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="11ba4-129">下表显示创建 groupPolicyPresentationMultiTextBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="11ba4-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="11ba4-130">属性</span><span class="sxs-lookup"><span data-stu-id="11ba4-130">Property</span></span>|<span data-ttu-id="11ba4-131">类型</span><span class="sxs-lookup"><span data-stu-id="11ba4-131">Type</span></span>|<span data-ttu-id="11ba4-132">说明</span><span class="sxs-lookup"><span data-stu-id="11ba4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11ba4-133">label</span><span class="sxs-lookup"><span data-stu-id="11ba4-133">label</span></span>|<span data-ttu-id="11ba4-134">字符串</span><span class="sxs-lookup"><span data-stu-id="11ba4-134">String</span></span>|<span data-ttu-id="11ba4-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="11ba4-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="11ba4-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="11ba4-136">The default value is empty.</span></span> <span data-ttu-id="11ba4-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="11ba4-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="11ba4-138">id</span><span class="sxs-lookup"><span data-stu-id="11ba4-138">id</span></span>|<span data-ttu-id="11ba4-139">字符串</span><span class="sxs-lookup"><span data-stu-id="11ba4-139">String</span></span>|<span data-ttu-id="11ba4-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="11ba4-140">Key of the entity.</span></span> <span data-ttu-id="11ba4-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="11ba4-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="11ba4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11ba4-142">lastModifiedDateTime</span></span>|<span data-ttu-id="11ba4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11ba4-143">DateTimeOffset</span></span>|<span data-ttu-id="11ba4-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="11ba4-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="11ba4-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="11ba4-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="11ba4-146">必需</span><span class="sxs-lookup"><span data-stu-id="11ba4-146">required</span></span>|<span data-ttu-id="11ba4-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="11ba4-147">Boolean</span></span>|<span data-ttu-id="11ba4-148">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="11ba4-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="11ba4-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="11ba4-149">Default value is false.</span></span>|
|<span data-ttu-id="11ba4-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="11ba4-150">maxLength</span></span>|<span data-ttu-id="11ba4-151">Int64</span><span class="sxs-lookup"><span data-stu-id="11ba4-151">Int64</span></span>|<span data-ttu-id="11ba4-152">一个无符号整数，指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="11ba4-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="11ba4-153">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="11ba4-153">Default value is 1023.</span></span>|
|<span data-ttu-id="11ba4-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="11ba4-154">maxStrings</span></span>|<span data-ttu-id="11ba4-155">Int64</span><span class="sxs-lookup"><span data-stu-id="11ba4-155">Int64</span></span>|<span data-ttu-id="11ba4-156">一个无符号整数，指定最大字符串数。</span><span class="sxs-lookup"><span data-stu-id="11ba4-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="11ba4-157">默认值为 0 。</span><span class="sxs-lookup"><span data-stu-id="11ba4-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="11ba4-158">响应</span><span class="sxs-lookup"><span data-stu-id="11ba4-158">Response</span></span>
<span data-ttu-id="11ba4-159">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="11ba4-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11ba4-160">示例</span><span class="sxs-lookup"><span data-stu-id="11ba4-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="11ba4-161">请求</span><span class="sxs-lookup"><span data-stu-id="11ba4-161">Request</span></span>
<span data-ttu-id="11ba4-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11ba4-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11ba4-163">响应</span><span class="sxs-lookup"><span data-stu-id="11ba4-163">Response</span></span>
<span data-ttu-id="11ba4-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="11ba4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




