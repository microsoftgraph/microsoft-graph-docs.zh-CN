---
title: 更新 groupPolicyPresentationMultiTextBox
description: 更新 groupPolicyPresentationMultiTextBox 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2aa9e5005269d2385f807f3eac9d16388e70cae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530905"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="c3745-103">更新 groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="c3745-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="c3745-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3745-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3745-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3745-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3745-106">更新[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3745-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3745-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3745-107">Prerequisites</span></span>
<span data-ttu-id="c3745-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3745-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3745-110">Permission type</span></span>|<span data-ttu-id="c3745-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3745-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3745-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3745-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3745-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3745-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c3745-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3745-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3745-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3745-115">Not supported.</span></span>|
|<span data-ttu-id="c3745-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3745-116">Application</span></span>|<span data-ttu-id="c3745-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3745-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3745-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3745-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="c3745-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3745-119">Request headers</span></span>
|<span data-ttu-id="c3745-120">标头</span><span class="sxs-lookup"><span data-stu-id="c3745-120">Header</span></span>|<span data-ttu-id="c3745-121">值</span><span class="sxs-lookup"><span data-stu-id="c3745-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3745-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3745-122">Authorization</span></span>|<span data-ttu-id="c3745-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3745-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3745-124">接受</span><span class="sxs-lookup"><span data-stu-id="c3745-124">Accept</span></span>|<span data-ttu-id="c3745-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3745-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3745-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3745-126">Request body</span></span>
<span data-ttu-id="c3745-127">在请求正文中, 提供[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3745-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="c3745-128">下表显示创建[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3745-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="c3745-129">属性</span><span class="sxs-lookup"><span data-stu-id="c3745-129">Property</span></span>|<span data-ttu-id="c3745-130">类型</span><span class="sxs-lookup"><span data-stu-id="c3745-130">Type</span></span>|<span data-ttu-id="c3745-131">说明</span><span class="sxs-lookup"><span data-stu-id="c3745-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3745-132">label</span><span class="sxs-lookup"><span data-stu-id="c3745-132">label</span></span>|<span data-ttu-id="c3745-133">String</span><span class="sxs-lookup"><span data-stu-id="c3745-133">String</span></span>|<span data-ttu-id="c3745-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="c3745-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c3745-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="c3745-135">The default value is empty.</span></span> <span data-ttu-id="c3745-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c3745-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c3745-137">id</span><span class="sxs-lookup"><span data-stu-id="c3745-137">id</span></span>|<span data-ttu-id="c3745-138">String</span><span class="sxs-lookup"><span data-stu-id="c3745-138">String</span></span>|<span data-ttu-id="c3745-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3745-139">Key of the entity.</span></span> <span data-ttu-id="c3745-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c3745-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c3745-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3745-141">lastModifiedDateTime</span></span>|<span data-ttu-id="c3745-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3745-142">DateTimeOffset</span></span>|<span data-ttu-id="c3745-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c3745-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="c3745-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c3745-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c3745-145">必需</span><span class="sxs-lookup"><span data-stu-id="c3745-145">required</span></span>|<span data-ttu-id="c3745-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="c3745-146">Boolean</span></span>|<span data-ttu-id="c3745-147">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="c3745-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="c3745-148">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="c3745-148">Default value is false.</span></span>|
|<span data-ttu-id="c3745-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="c3745-149">maxLength</span></span>|<span data-ttu-id="c3745-150">Int64</span><span class="sxs-lookup"><span data-stu-id="c3745-150">Int64</span></span>|<span data-ttu-id="c3745-151">一个无符号整数, 指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="c3745-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="c3745-152">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="c3745-152">Default value is 1023.</span></span>|
|<span data-ttu-id="c3745-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="c3745-153">maxStrings</span></span>|<span data-ttu-id="c3745-154">Int64</span><span class="sxs-lookup"><span data-stu-id="c3745-154">Int64</span></span>|<span data-ttu-id="c3745-155">一个无符号整数, 指定最大字符串数。</span><span class="sxs-lookup"><span data-stu-id="c3745-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="c3745-156">默认值为 0 。</span><span class="sxs-lookup"><span data-stu-id="c3745-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="c3745-157">响应</span><span class="sxs-lookup"><span data-stu-id="c3745-157">Response</span></span>
<span data-ttu-id="c3745-158">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c3745-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3745-159">示例</span><span class="sxs-lookup"><span data-stu-id="c3745-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3745-160">请求</span><span class="sxs-lookup"><span data-stu-id="c3745-160">Request</span></span>
<span data-ttu-id="c3745-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3745-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3745-162">响应</span><span class="sxs-lookup"><span data-stu-id="c3745-162">Response</span></span>
<span data-ttu-id="c3745-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3745-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





