---
title: 更新 groupPolicyPresentationTextBox
description: 更新 groupPolicyPresentationTextBox 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 48417f8d3dcc057e535adcf429cc96922c24162a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431329"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="692fe-103">更新 groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="692fe-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="692fe-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="692fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="692fe-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="692fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="692fe-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="692fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="692fe-107">更新[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="692fe-107">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="692fe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="692fe-108">Prerequisites</span></span>
<span data-ttu-id="692fe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="692fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="692fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="692fe-111">Permission type</span></span>|<span data-ttu-id="692fe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="692fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="692fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="692fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="692fe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="692fe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="692fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="692fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="692fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="692fe-116">Not supported.</span></span>|
|<span data-ttu-id="692fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="692fe-117">Application</span></span>|<span data-ttu-id="692fe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="692fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="692fe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="692fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="692fe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="692fe-120">Request headers</span></span>
|<span data-ttu-id="692fe-121">标头</span><span class="sxs-lookup"><span data-stu-id="692fe-121">Header</span></span>|<span data-ttu-id="692fe-122">值</span><span class="sxs-lookup"><span data-stu-id="692fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="692fe-123">授权</span><span class="sxs-lookup"><span data-stu-id="692fe-123">Authorization</span></span>|<span data-ttu-id="692fe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="692fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="692fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="692fe-125">Accept</span></span>|<span data-ttu-id="692fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="692fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="692fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="692fe-127">Request body</span></span>
<span data-ttu-id="692fe-128">在请求正文中，提供[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="692fe-128">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="692fe-129">下表显示时创建[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="692fe-129">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="692fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="692fe-130">Property</span></span>|<span data-ttu-id="692fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="692fe-131">Type</span></span>|<span data-ttu-id="692fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="692fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="692fe-133">标签</span><span class="sxs-lookup"><span data-stu-id="692fe-133">label</span></span>|<span data-ttu-id="692fe-134">String</span><span class="sxs-lookup"><span data-stu-id="692fe-134">String</span></span>|<span data-ttu-id="692fe-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="692fe-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="692fe-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="692fe-136">The default value is empty.</span></span> <span data-ttu-id="692fe-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="692fe-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="692fe-138">id</span><span class="sxs-lookup"><span data-stu-id="692fe-138">id</span></span>|<span data-ttu-id="692fe-139">String</span><span class="sxs-lookup"><span data-stu-id="692fe-139">String</span></span>|<span data-ttu-id="692fe-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="692fe-140">Key of the entity.</span></span> <span data-ttu-id="692fe-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="692fe-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="692fe-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="692fe-142">lastModifiedDateTime</span></span>|<span data-ttu-id="692fe-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="692fe-143">DateTimeOffset</span></span>|<span data-ttu-id="692fe-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="692fe-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="692fe-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="692fe-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="692fe-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="692fe-146">defaultValue</span></span>|<span data-ttu-id="692fe-147">字符串</span><span class="sxs-lookup"><span data-stu-id="692fe-147">String</span></span>|<span data-ttu-id="692fe-148">本地化显示在文本框中的默认字符串。</span><span class="sxs-lookup"><span data-stu-id="692fe-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="692fe-149">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="692fe-149">The default value is empty.</span></span>|
|<span data-ttu-id="692fe-150">必需</span><span class="sxs-lookup"><span data-stu-id="692fe-150">required</span></span>|<span data-ttu-id="692fe-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="692fe-151">Boolean</span></span>|<span data-ttu-id="692fe-152">在文本框中输入值的要求。</span><span class="sxs-lookup"><span data-stu-id="692fe-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="692fe-153">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="692fe-153">Default value is false.</span></span>|
|<span data-ttu-id="692fe-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="692fe-154">maxLength</span></span>|<span data-ttu-id="692fe-155">Int64</span><span class="sxs-lookup"><span data-stu-id="692fe-155">Int64</span></span>|<span data-ttu-id="692fe-156">指定的文本字符的最大数量无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="692fe-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="692fe-157">默认值为 1023年。</span><span class="sxs-lookup"><span data-stu-id="692fe-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="692fe-158">响应</span><span class="sxs-lookup"><span data-stu-id="692fe-158">Response</span></span>
<span data-ttu-id="692fe-159">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="692fe-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="692fe-160">示例</span><span class="sxs-lookup"><span data-stu-id="692fe-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="692fe-161">请求</span><span class="sxs-lookup"><span data-stu-id="692fe-161">Request</span></span>
<span data-ttu-id="692fe-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="692fe-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="692fe-163">响应</span><span class="sxs-lookup"><span data-stu-id="692fe-163">Response</span></span>
<span data-ttu-id="692fe-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="692fe-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




