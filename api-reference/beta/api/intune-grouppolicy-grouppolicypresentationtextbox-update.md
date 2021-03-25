---
title: 更新 groupPolicyPresentationTextBox
description: 更新 groupPolicyPresentationTextBox 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ff83558c1d66505e0623d4cd9b48ef83f033f37
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157389"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="f92eb-103">更新 groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="f92eb-103">Update groupPolicyPresentationTextBox</span></span>

<span data-ttu-id="f92eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f92eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f92eb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f92eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f92eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f92eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f92eb-107">更新 [groupPolicyPresentationTextBox 对象](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f92eb-107">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f92eb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f92eb-108">Prerequisites</span></span>
<span data-ttu-id="f92eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f92eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f92eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f92eb-111">Permission type</span></span>|<span data-ttu-id="f92eb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f92eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f92eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f92eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f92eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f92eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f92eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f92eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f92eb-116">Not supported.</span></span>|
|<span data-ttu-id="f92eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f92eb-117">Application</span></span>|<span data-ttu-id="f92eb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92eb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f92eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f92eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="f92eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f92eb-120">Request headers</span></span>
|<span data-ttu-id="f92eb-121">标头</span><span class="sxs-lookup"><span data-stu-id="f92eb-121">Header</span></span>|<span data-ttu-id="f92eb-122">值</span><span class="sxs-lookup"><span data-stu-id="f92eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f92eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f92eb-123">Authorization</span></span>|<span data-ttu-id="f92eb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f92eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f92eb-125">接受</span><span class="sxs-lookup"><span data-stu-id="f92eb-125">Accept</span></span>|<span data-ttu-id="f92eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f92eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f92eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f92eb-127">Request body</span></span>
<span data-ttu-id="f92eb-128">在请求正文中，提供 [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f92eb-128">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="f92eb-129">下表显示创建 [groupPolicyPresentationTextBox 时所需的属性](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)。</span><span class="sxs-lookup"><span data-stu-id="f92eb-129">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="f92eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="f92eb-130">Property</span></span>|<span data-ttu-id="f92eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="f92eb-131">Type</span></span>|<span data-ttu-id="f92eb-132">说明</span><span class="sxs-lookup"><span data-stu-id="f92eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f92eb-133">label</span><span class="sxs-lookup"><span data-stu-id="f92eb-133">label</span></span>|<span data-ttu-id="f92eb-134">String</span><span class="sxs-lookup"><span data-stu-id="f92eb-134">String</span></span>|<span data-ttu-id="f92eb-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="f92eb-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f92eb-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="f92eb-136">The default value is empty.</span></span> <span data-ttu-id="f92eb-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f92eb-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f92eb-138">id</span><span class="sxs-lookup"><span data-stu-id="f92eb-138">id</span></span>|<span data-ttu-id="f92eb-139">String</span><span class="sxs-lookup"><span data-stu-id="f92eb-139">String</span></span>|<span data-ttu-id="f92eb-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f92eb-140">Key of the entity.</span></span> <span data-ttu-id="f92eb-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f92eb-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f92eb-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f92eb-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f92eb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f92eb-143">DateTimeOffset</span></span>|<span data-ttu-id="f92eb-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f92eb-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="f92eb-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f92eb-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f92eb-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="f92eb-146">defaultValue</span></span>|<span data-ttu-id="f92eb-147">String</span><span class="sxs-lookup"><span data-stu-id="f92eb-147">String</span></span>|<span data-ttu-id="f92eb-148">文本框中显示的本地化默认字符串。</span><span class="sxs-lookup"><span data-stu-id="f92eb-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="f92eb-149">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="f92eb-149">The default value is empty.</span></span>|
|<span data-ttu-id="f92eb-150">必需</span><span class="sxs-lookup"><span data-stu-id="f92eb-150">required</span></span>|<span data-ttu-id="f92eb-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f92eb-151">Boolean</span></span>|<span data-ttu-id="f92eb-152">要求在文本框中输入值。</span><span class="sxs-lookup"><span data-stu-id="f92eb-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="f92eb-153">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="f92eb-153">Default value is false.</span></span>|
|<span data-ttu-id="f92eb-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="f92eb-154">maxLength</span></span>|<span data-ttu-id="f92eb-155">Int64</span><span class="sxs-lookup"><span data-stu-id="f92eb-155">Int64</span></span>|<span data-ttu-id="f92eb-156">一个无符号整数，指定最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="f92eb-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="f92eb-157">默认值为 1023。</span><span class="sxs-lookup"><span data-stu-id="f92eb-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="f92eb-158">响应</span><span class="sxs-lookup"><span data-stu-id="f92eb-158">Response</span></span>
<span data-ttu-id="f92eb-159">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f92eb-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f92eb-160">示例</span><span class="sxs-lookup"><span data-stu-id="f92eb-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="f92eb-161">请求</span><span class="sxs-lookup"><span data-stu-id="f92eb-161">Request</span></span>
<span data-ttu-id="f92eb-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f92eb-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f92eb-163">响应</span><span class="sxs-lookup"><span data-stu-id="f92eb-163">Response</span></span>
<span data-ttu-id="f92eb-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f92eb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




