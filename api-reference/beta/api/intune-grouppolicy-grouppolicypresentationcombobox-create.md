---
title: 创建 groupPolicyPresentationComboBox
description: 创建新的 groupPolicyPresentationComboBox 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 328550ed5c07259672ae4debee9a8b28681a4b8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431326"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="cc1f8-103">创建 groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="cc1f8-103">Create groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="cc1f8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc1f8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc1f8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc1f8-107">创建新的[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-107">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc1f8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cc1f8-108">Prerequisites</span></span>
<span data-ttu-id="cc1f8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc1f8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc1f8-111">Permission type</span></span>|<span data-ttu-id="cc1f8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cc1f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc1f8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc1f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc1f8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc1f8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc1f8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc1f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc1f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-116">Not supported.</span></span>|
|<span data-ttu-id="cc1f8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc1f8-117">Application</span></span>|<span data-ttu-id="cc1f8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc1f8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc1f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="cc1f8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc1f8-120">Request headers</span></span>
|<span data-ttu-id="cc1f8-121">标头</span><span class="sxs-lookup"><span data-stu-id="cc1f8-121">Header</span></span>|<span data-ttu-id="cc1f8-122">值</span><span class="sxs-lookup"><span data-stu-id="cc1f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc1f8-123">授权</span><span class="sxs-lookup"><span data-stu-id="cc1f8-123">Authorization</span></span>|<span data-ttu-id="cc1f8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc1f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc1f8-125">Accept</span></span>|<span data-ttu-id="cc1f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc1f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc1f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc1f8-127">Request body</span></span>
<span data-ttu-id="cc1f8-128">在请求正文中，提供 groupPolicyPresentationComboBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-128">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="cc1f8-129">下表显示时创建 groupPolicyPresentationComboBox 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-129">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="cc1f8-130">属性</span><span class="sxs-lookup"><span data-stu-id="cc1f8-130">Property</span></span>|<span data-ttu-id="cc1f8-131">类型</span><span class="sxs-lookup"><span data-stu-id="cc1f8-131">Type</span></span>|<span data-ttu-id="cc1f8-132">说明</span><span class="sxs-lookup"><span data-stu-id="cc1f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc1f8-133">标签</span><span class="sxs-lookup"><span data-stu-id="cc1f8-133">label</span></span>|<span data-ttu-id="cc1f8-134">String</span><span class="sxs-lookup"><span data-stu-id="cc1f8-134">String</span></span>|<span data-ttu-id="cc1f8-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cc1f8-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-136">The default value is empty.</span></span> <span data-ttu-id="cc1f8-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cc1f8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cc1f8-138">id</span><span class="sxs-lookup"><span data-stu-id="cc1f8-138">id</span></span>|<span data-ttu-id="cc1f8-139">String</span><span class="sxs-lookup"><span data-stu-id="cc1f8-139">String</span></span>|<span data-ttu-id="cc1f8-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-140">Key of the entity.</span></span> <span data-ttu-id="cc1f8-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cc1f8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cc1f8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc1f8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="cc1f8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc1f8-143">DateTimeOffset</span></span>|<span data-ttu-id="cc1f8-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="cc1f8-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cc1f8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cc1f8-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="cc1f8-146">defaultValue</span></span>|<span data-ttu-id="cc1f8-147">字符串</span><span class="sxs-lookup"><span data-stu-id="cc1f8-147">String</span></span>|<span data-ttu-id="cc1f8-148">本地化的组合框中显示的默认字符串。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="cc1f8-149">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-149">The default value is empty.</span></span>|
|<span data-ttu-id="cc1f8-150">建议</span><span class="sxs-lookup"><span data-stu-id="cc1f8-150">suggestions</span></span>|<span data-ttu-id="cc1f8-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="cc1f8-151">String collection</span></span>|<span data-ttu-id="cc1f8-152">组合框下拉列表中列出的本地化的字符串。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="cc1f8-153">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-153">The default value is empty.</span></span>|
|<span data-ttu-id="cc1f8-154">必需</span><span class="sxs-lookup"><span data-stu-id="cc1f8-154">required</span></span>|<span data-ttu-id="cc1f8-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc1f8-155">Boolean</span></span>|<span data-ttu-id="cc1f8-156">指定是否必须参数指定一个值。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="cc1f8-157">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-157">The default value is false.</span></span>|
|<span data-ttu-id="cc1f8-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="cc1f8-158">maxLength</span></span>|<span data-ttu-id="cc1f8-159">Int64</span><span class="sxs-lookup"><span data-stu-id="cc1f8-159">Int64</span></span>|<span data-ttu-id="cc1f8-160">指定的参数的文本字符的最大数量无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="cc1f8-161">默认值是 1023年。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="cc1f8-162">响应</span><span class="sxs-lookup"><span data-stu-id="cc1f8-162">Response</span></span>
<span data-ttu-id="cc1f8-163">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-163">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc1f8-164">示例</span><span class="sxs-lookup"><span data-stu-id="cc1f8-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc1f8-165">请求</span><span class="sxs-lookup"><span data-stu-id="cc1f8-165">Request</span></span>
<span data-ttu-id="cc1f8-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="cc1f8-167">响应</span><span class="sxs-lookup"><span data-stu-id="cc1f8-167">Response</span></span>
<span data-ttu-id="cc1f8-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc1f8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```




