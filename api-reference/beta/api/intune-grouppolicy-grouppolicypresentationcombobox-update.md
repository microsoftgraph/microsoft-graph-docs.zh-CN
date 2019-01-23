---
title: 更新 groupPolicyPresentationComboBox
description: 更新 groupPolicyPresentationComboBox 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6302d52e91e5fe1cf8a21e525d0eccef608b3b24
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429493"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="15072-103">更新 groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="15072-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="15072-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="15072-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15072-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="15072-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15072-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="15072-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15072-107">更新[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="15072-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15072-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="15072-108">Prerequisites</span></span>
<span data-ttu-id="15072-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="15072-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15072-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="15072-111">Permission type</span></span>|<span data-ttu-id="15072-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="15072-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15072-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15072-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15072-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15072-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15072-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15072-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15072-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="15072-116">Not supported.</span></span>|
|<span data-ttu-id="15072-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="15072-117">Application</span></span>|<span data-ttu-id="15072-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="15072-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15072-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15072-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="15072-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="15072-120">Request headers</span></span>
|<span data-ttu-id="15072-121">标头</span><span class="sxs-lookup"><span data-stu-id="15072-121">Header</span></span>|<span data-ttu-id="15072-122">值</span><span class="sxs-lookup"><span data-stu-id="15072-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15072-123">授权</span><span class="sxs-lookup"><span data-stu-id="15072-123">Authorization</span></span>|<span data-ttu-id="15072-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="15072-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15072-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15072-125">Accept</span></span>|<span data-ttu-id="15072-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15072-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15072-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="15072-127">Request body</span></span>
<span data-ttu-id="15072-128">在请求正文中，提供[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15072-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="15072-129">下表显示时创建[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="15072-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="15072-130">属性</span><span class="sxs-lookup"><span data-stu-id="15072-130">Property</span></span>|<span data-ttu-id="15072-131">类型</span><span class="sxs-lookup"><span data-stu-id="15072-131">Type</span></span>|<span data-ttu-id="15072-132">说明</span><span class="sxs-lookup"><span data-stu-id="15072-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15072-133">标签</span><span class="sxs-lookup"><span data-stu-id="15072-133">label</span></span>|<span data-ttu-id="15072-134">String</span><span class="sxs-lookup"><span data-stu-id="15072-134">String</span></span>|<span data-ttu-id="15072-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="15072-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="15072-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="15072-136">The default value is empty.</span></span> <span data-ttu-id="15072-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="15072-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="15072-138">id</span><span class="sxs-lookup"><span data-stu-id="15072-138">id</span></span>|<span data-ttu-id="15072-139">String</span><span class="sxs-lookup"><span data-stu-id="15072-139">String</span></span>|<span data-ttu-id="15072-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="15072-140">Key of the entity.</span></span> <span data-ttu-id="15072-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="15072-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="15072-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15072-142">lastModifiedDateTime</span></span>|<span data-ttu-id="15072-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15072-143">DateTimeOffset</span></span>|<span data-ttu-id="15072-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="15072-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="15072-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="15072-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="15072-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="15072-146">defaultValue</span></span>|<span data-ttu-id="15072-147">字符串</span><span class="sxs-lookup"><span data-stu-id="15072-147">String</span></span>|<span data-ttu-id="15072-148">本地化的组合框中显示的默认字符串。</span><span class="sxs-lookup"><span data-stu-id="15072-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="15072-149">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="15072-149">The default value is empty.</span></span>|
|<span data-ttu-id="15072-150">建议</span><span class="sxs-lookup"><span data-stu-id="15072-150">suggestions</span></span>|<span data-ttu-id="15072-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="15072-151">String collection</span></span>|<span data-ttu-id="15072-152">组合框下拉列表中列出的本地化的字符串。</span><span class="sxs-lookup"><span data-stu-id="15072-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="15072-153">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="15072-153">The default value is empty.</span></span>|
|<span data-ttu-id="15072-154">必需</span><span class="sxs-lookup"><span data-stu-id="15072-154">required</span></span>|<span data-ttu-id="15072-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="15072-155">Boolean</span></span>|<span data-ttu-id="15072-156">指定是否必须参数指定一个值。</span><span class="sxs-lookup"><span data-stu-id="15072-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="15072-157">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="15072-157">The default value is false.</span></span>|
|<span data-ttu-id="15072-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="15072-158">maxLength</span></span>|<span data-ttu-id="15072-159">Int64</span><span class="sxs-lookup"><span data-stu-id="15072-159">Int64</span></span>|<span data-ttu-id="15072-160">指定的参数的文本字符的最大数量无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="15072-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="15072-161">默认值是 1023年。</span><span class="sxs-lookup"><span data-stu-id="15072-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="15072-162">响应</span><span class="sxs-lookup"><span data-stu-id="15072-162">Response</span></span>
<span data-ttu-id="15072-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="15072-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15072-164">示例</span><span class="sxs-lookup"><span data-stu-id="15072-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="15072-165">请求</span><span class="sxs-lookup"><span data-stu-id="15072-165">Request</span></span>
<span data-ttu-id="15072-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="15072-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="15072-167">响应</span><span class="sxs-lookup"><span data-stu-id="15072-167">Response</span></span>
<span data-ttu-id="15072-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="15072-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




