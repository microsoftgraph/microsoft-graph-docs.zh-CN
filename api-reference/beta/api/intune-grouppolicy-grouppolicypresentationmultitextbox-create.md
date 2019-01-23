---
title: 创建 groupPolicyPresentationMultiTextBox
description: 创建新的 groupPolicyPresentationMultiTextBox 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41042c5ad62cb56573e924c69b62cef72ee6835c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429279"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="23e84-103">创建 groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="23e84-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="23e84-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="23e84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23e84-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23e84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23e84-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23e84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23e84-107">创建新的[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23e84-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23e84-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="23e84-108">Prerequisites</span></span>
<span data-ttu-id="23e84-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="23e84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23e84-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="23e84-111">Permission type</span></span>|<span data-ttu-id="23e84-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="23e84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23e84-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23e84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23e84-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e84-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23e84-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23e84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23e84-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="23e84-116">Not supported.</span></span>|
|<span data-ttu-id="23e84-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="23e84-117">Application</span></span>|<span data-ttu-id="23e84-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="23e84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23e84-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23e84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="23e84-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="23e84-120">Request headers</span></span>
|<span data-ttu-id="23e84-121">标头</span><span class="sxs-lookup"><span data-stu-id="23e84-121">Header</span></span>|<span data-ttu-id="23e84-122">值</span><span class="sxs-lookup"><span data-stu-id="23e84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23e84-123">授权</span><span class="sxs-lookup"><span data-stu-id="23e84-123">Authorization</span></span>|<span data-ttu-id="23e84-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="23e84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23e84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23e84-125">Accept</span></span>|<span data-ttu-id="23e84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23e84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23e84-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="23e84-127">Request body</span></span>
<span data-ttu-id="23e84-128">在请求正文中，提供 groupPolicyPresentationMultiTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23e84-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="23e84-129">下表显示时创建 groupPolicyPresentationMultiTextBox 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="23e84-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="23e84-130">属性</span><span class="sxs-lookup"><span data-stu-id="23e84-130">Property</span></span>|<span data-ttu-id="23e84-131">类型</span><span class="sxs-lookup"><span data-stu-id="23e84-131">Type</span></span>|<span data-ttu-id="23e84-132">说明</span><span class="sxs-lookup"><span data-stu-id="23e84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23e84-133">标签</span><span class="sxs-lookup"><span data-stu-id="23e84-133">label</span></span>|<span data-ttu-id="23e84-134">String</span><span class="sxs-lookup"><span data-stu-id="23e84-134">String</span></span>|<span data-ttu-id="23e84-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="23e84-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="23e84-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="23e84-136">The default value is empty.</span></span> <span data-ttu-id="23e84-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="23e84-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="23e84-138">id</span><span class="sxs-lookup"><span data-stu-id="23e84-138">id</span></span>|<span data-ttu-id="23e84-139">String</span><span class="sxs-lookup"><span data-stu-id="23e84-139">String</span></span>|<span data-ttu-id="23e84-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="23e84-140">Key of the entity.</span></span> <span data-ttu-id="23e84-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="23e84-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="23e84-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23e84-142">lastModifiedDateTime</span></span>|<span data-ttu-id="23e84-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23e84-143">DateTimeOffset</span></span>|<span data-ttu-id="23e84-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="23e84-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="23e84-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="23e84-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="23e84-146">必需</span><span class="sxs-lookup"><span data-stu-id="23e84-146">required</span></span>|<span data-ttu-id="23e84-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="23e84-147">Boolean</span></span>|<span data-ttu-id="23e84-148">在文本框中输入值的要求。</span><span class="sxs-lookup"><span data-stu-id="23e84-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="23e84-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="23e84-149">Default value is false.</span></span>|
|<span data-ttu-id="23e84-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="23e84-150">maxLength</span></span>|<span data-ttu-id="23e84-151">Int64</span><span class="sxs-lookup"><span data-stu-id="23e84-151">Int64</span></span>|<span data-ttu-id="23e84-152">指定的文本字符的最大数量无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="23e84-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="23e84-153">默认值为 1023年。</span><span class="sxs-lookup"><span data-stu-id="23e84-153">Default value is 1023.</span></span>|
|<span data-ttu-id="23e84-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="23e84-154">maxStrings</span></span>|<span data-ttu-id="23e84-155">Int64</span><span class="sxs-lookup"><span data-stu-id="23e84-155">Int64</span></span>|<span data-ttu-id="23e84-156">无符号的整数，指定字符串的最大数量。</span><span class="sxs-lookup"><span data-stu-id="23e84-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="23e84-157">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="23e84-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="23e84-158">响应</span><span class="sxs-lookup"><span data-stu-id="23e84-158">Response</span></span>
<span data-ttu-id="23e84-159">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23e84-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23e84-160">示例</span><span class="sxs-lookup"><span data-stu-id="23e84-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="23e84-161">请求</span><span class="sxs-lookup"><span data-stu-id="23e84-161">Request</span></span>
<span data-ttu-id="23e84-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23e84-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="23e84-163">响应</span><span class="sxs-lookup"><span data-stu-id="23e84-163">Response</span></span>
<span data-ttu-id="23e84-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23e84-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




