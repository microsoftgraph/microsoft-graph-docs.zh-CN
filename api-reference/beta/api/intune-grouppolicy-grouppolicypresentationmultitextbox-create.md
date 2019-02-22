---
title: 创建 groupPolicyPresentationMultiTextBox
description: 创建新的 groupPolicyPresentationMultiTextBox 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdde2677c4852c70f1693e7a16e2b9e3fb048388
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152099"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="be6ac-103">创建 groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="be6ac-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="be6ac-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be6ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be6ac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be6ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be6ac-106">创建新的[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="be6ac-106">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be6ac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="be6ac-107">Prerequisites</span></span>
<span data-ttu-id="be6ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="be6ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="be6ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="be6ac-110">Permission type</span></span>|<span data-ttu-id="be6ac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be6ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be6ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be6ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be6ac-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be6ac-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be6ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be6ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be6ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be6ac-115">Not supported.</span></span>|
|<span data-ttu-id="be6ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="be6ac-116">Application</span></span>|<span data-ttu-id="be6ac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="be6ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be6ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be6ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="be6ac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="be6ac-119">Request headers</span></span>
|<span data-ttu-id="be6ac-120">标头</span><span class="sxs-lookup"><span data-stu-id="be6ac-120">Header</span></span>|<span data-ttu-id="be6ac-121">值</span><span class="sxs-lookup"><span data-stu-id="be6ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be6ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be6ac-122">Authorization</span></span>|<span data-ttu-id="be6ac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be6ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be6ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be6ac-124">Accept</span></span>|<span data-ttu-id="be6ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be6ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be6ac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="be6ac-126">Request body</span></span>
<span data-ttu-id="be6ac-127">在请求正文中, 提供 groupPolicyPresentationMultiTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be6ac-127">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="be6ac-128">下表显示创建 groupPolicyPresentationMultiTextBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be6ac-128">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="be6ac-129">属性</span><span class="sxs-lookup"><span data-stu-id="be6ac-129">Property</span></span>|<span data-ttu-id="be6ac-130">类型</span><span class="sxs-lookup"><span data-stu-id="be6ac-130">Type</span></span>|<span data-ttu-id="be6ac-131">说明</span><span class="sxs-lookup"><span data-stu-id="be6ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be6ac-132">标签</span><span class="sxs-lookup"><span data-stu-id="be6ac-132">label</span></span>|<span data-ttu-id="be6ac-133">字符串</span><span class="sxs-lookup"><span data-stu-id="be6ac-133">String</span></span>|<span data-ttu-id="be6ac-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="be6ac-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="be6ac-135">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="be6ac-135">The default value is empty.</span></span> <span data-ttu-id="be6ac-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="be6ac-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="be6ac-137">id</span><span class="sxs-lookup"><span data-stu-id="be6ac-137">id</span></span>|<span data-ttu-id="be6ac-138">String</span><span class="sxs-lookup"><span data-stu-id="be6ac-138">String</span></span>|<span data-ttu-id="be6ac-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be6ac-139">Key of the entity.</span></span> <span data-ttu-id="be6ac-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="be6ac-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="be6ac-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be6ac-141">lastModifiedDateTime</span></span>|<span data-ttu-id="be6ac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be6ac-142">DateTimeOffset</span></span>|<span data-ttu-id="be6ac-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="be6ac-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="be6ac-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="be6ac-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="be6ac-145">必需</span><span class="sxs-lookup"><span data-stu-id="be6ac-145">required</span></span>|<span data-ttu-id="be6ac-146">布尔</span><span class="sxs-lookup"><span data-stu-id="be6ac-146">Boolean</span></span>|<span data-ttu-id="be6ac-147">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="be6ac-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="be6ac-148">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="be6ac-148">Default value is false.</span></span>|
|<span data-ttu-id="be6ac-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="be6ac-149">maxLength</span></span>|<span data-ttu-id="be6ac-150">Int64</span><span class="sxs-lookup"><span data-stu-id="be6ac-150">Int64</span></span>|<span data-ttu-id="be6ac-151">一个无符号整数, 指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="be6ac-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="be6ac-152">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="be6ac-152">Default value is 1023.</span></span>|
|<span data-ttu-id="be6ac-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="be6ac-153">maxStrings</span></span>|<span data-ttu-id="be6ac-154">Int64</span><span class="sxs-lookup"><span data-stu-id="be6ac-154">Int64</span></span>|<span data-ttu-id="be6ac-155">一个无符号整数, 指定最大字符串数。</span><span class="sxs-lookup"><span data-stu-id="be6ac-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="be6ac-156">默认值为0。</span><span class="sxs-lookup"><span data-stu-id="be6ac-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="be6ac-157">响应</span><span class="sxs-lookup"><span data-stu-id="be6ac-157">Response</span></span>
<span data-ttu-id="be6ac-158">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="be6ac-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be6ac-159">示例</span><span class="sxs-lookup"><span data-stu-id="be6ac-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="be6ac-160">请求</span><span class="sxs-lookup"><span data-stu-id="be6ac-160">Request</span></span>
<span data-ttu-id="be6ac-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be6ac-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be6ac-162">响应</span><span class="sxs-lookup"><span data-stu-id="be6ac-162">Response</span></span>
<span data-ttu-id="be6ac-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be6ac-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




