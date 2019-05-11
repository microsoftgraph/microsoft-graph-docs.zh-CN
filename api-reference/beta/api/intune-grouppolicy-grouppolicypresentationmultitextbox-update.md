---
title: 更新 groupPolicyPresentationMultiTextBox
description: 更新 groupPolicyPresentationMultiTextBox 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10c92f40413790c8049563123975f31d2ce3eeba
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904718"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="6a309-103">更新 groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="6a309-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="6a309-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a309-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a309-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a309-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a309-106">更新[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a309-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a309-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a309-107">Prerequisites</span></span>
<span data-ttu-id="6a309-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a309-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a309-110">Permission type</span></span>|<span data-ttu-id="6a309-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a309-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a309-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a309-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a309-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a309-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a309-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a309-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a309-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a309-115">Not supported.</span></span>|
|<span data-ttu-id="6a309-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a309-116">Application</span></span>|<span data-ttu-id="6a309-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a309-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a309-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a309-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="6a309-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a309-119">Request headers</span></span>
|<span data-ttu-id="6a309-120">标头</span><span class="sxs-lookup"><span data-stu-id="6a309-120">Header</span></span>|<span data-ttu-id="6a309-121">值</span><span class="sxs-lookup"><span data-stu-id="6a309-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a309-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a309-122">Authorization</span></span>|<span data-ttu-id="6a309-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a309-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a309-124">接受</span><span class="sxs-lookup"><span data-stu-id="6a309-124">Accept</span></span>|<span data-ttu-id="6a309-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a309-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a309-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a309-126">Request body</span></span>
<span data-ttu-id="6a309-127">在请求正文中, 提供[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a309-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="6a309-128">下表显示创建[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a309-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="6a309-129">属性</span><span class="sxs-lookup"><span data-stu-id="6a309-129">Property</span></span>|<span data-ttu-id="6a309-130">类型</span><span class="sxs-lookup"><span data-stu-id="6a309-130">Type</span></span>|<span data-ttu-id="6a309-131">说明</span><span class="sxs-lookup"><span data-stu-id="6a309-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a309-132">label</span><span class="sxs-lookup"><span data-stu-id="6a309-132">label</span></span>|<span data-ttu-id="6a309-133">String</span><span class="sxs-lookup"><span data-stu-id="6a309-133">String</span></span>|<span data-ttu-id="6a309-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="6a309-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6a309-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="6a309-135">The default value is empty.</span></span> <span data-ttu-id="6a309-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6a309-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6a309-137">id</span><span class="sxs-lookup"><span data-stu-id="6a309-137">id</span></span>|<span data-ttu-id="6a309-138">String</span><span class="sxs-lookup"><span data-stu-id="6a309-138">String</span></span>|<span data-ttu-id="6a309-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6a309-139">Key of the entity.</span></span> <span data-ttu-id="6a309-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6a309-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6a309-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a309-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6a309-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a309-142">DateTimeOffset</span></span>|<span data-ttu-id="6a309-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6a309-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="6a309-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6a309-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6a309-145">必需</span><span class="sxs-lookup"><span data-stu-id="6a309-145">required</span></span>|<span data-ttu-id="6a309-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a309-146">Boolean</span></span>|<span data-ttu-id="6a309-147">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="6a309-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="6a309-148">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="6a309-148">Default value is false.</span></span>|
|<span data-ttu-id="6a309-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="6a309-149">maxLength</span></span>|<span data-ttu-id="6a309-150">Int64</span><span class="sxs-lookup"><span data-stu-id="6a309-150">Int64</span></span>|<span data-ttu-id="6a309-151">一个无符号整数, 指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="6a309-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="6a309-152">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="6a309-152">Default value is 1023.</span></span>|
|<span data-ttu-id="6a309-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="6a309-153">maxStrings</span></span>|<span data-ttu-id="6a309-154">Int64</span><span class="sxs-lookup"><span data-stu-id="6a309-154">Int64</span></span>|<span data-ttu-id="6a309-155">一个无符号整数, 指定最大字符串数。</span><span class="sxs-lookup"><span data-stu-id="6a309-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="6a309-156">默认值为 0 。</span><span class="sxs-lookup"><span data-stu-id="6a309-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="6a309-157">响应</span><span class="sxs-lookup"><span data-stu-id="6a309-157">Response</span></span>
<span data-ttu-id="6a309-158">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a309-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a309-159">示例</span><span class="sxs-lookup"><span data-stu-id="6a309-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a309-160">请求</span><span class="sxs-lookup"><span data-stu-id="6a309-160">Request</span></span>
<span data-ttu-id="6a309-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a309-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="6a309-162">响应</span><span class="sxs-lookup"><span data-stu-id="6a309-162">Response</span></span>
<span data-ttu-id="6a309-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a309-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




