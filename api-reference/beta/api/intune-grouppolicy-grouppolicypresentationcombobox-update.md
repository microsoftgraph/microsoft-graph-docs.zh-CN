---
title: 更新 groupPolicyPresentationComboBox
description: 更新 groupPolicyPresentationComboBox 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9dbb758f82c31e271cba2d5e2182efe947f78f5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974130"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="a901e-103">更新 groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="a901e-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="a901e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a901e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a901e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a901e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a901e-106">更新[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a901e-106">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a901e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a901e-107">Prerequisites</span></span>
<span data-ttu-id="a901e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a901e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a901e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a901e-110">Permission type</span></span>|<span data-ttu-id="a901e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a901e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a901e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a901e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a901e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a901e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a901e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a901e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a901e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a901e-115">Not supported.</span></span>|
|<span data-ttu-id="a901e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a901e-116">Application</span></span>|<span data-ttu-id="a901e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a901e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a901e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a901e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="a901e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a901e-119">Request headers</span></span>
|<span data-ttu-id="a901e-120">标头</span><span class="sxs-lookup"><span data-stu-id="a901e-120">Header</span></span>|<span data-ttu-id="a901e-121">值</span><span class="sxs-lookup"><span data-stu-id="a901e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a901e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a901e-122">Authorization</span></span>|<span data-ttu-id="a901e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a901e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a901e-124">接受</span><span class="sxs-lookup"><span data-stu-id="a901e-124">Accept</span></span>|<span data-ttu-id="a901e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a901e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a901e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a901e-126">Request body</span></span>
<span data-ttu-id="a901e-127">在请求正文中, 提供[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a901e-127">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="a901e-128">下表显示创建[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a901e-128">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="a901e-129">属性</span><span class="sxs-lookup"><span data-stu-id="a901e-129">Property</span></span>|<span data-ttu-id="a901e-130">类型</span><span class="sxs-lookup"><span data-stu-id="a901e-130">Type</span></span>|<span data-ttu-id="a901e-131">说明</span><span class="sxs-lookup"><span data-stu-id="a901e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a901e-132">label</span><span class="sxs-lookup"><span data-stu-id="a901e-132">label</span></span>|<span data-ttu-id="a901e-133">String</span><span class="sxs-lookup"><span data-stu-id="a901e-133">String</span></span>|<span data-ttu-id="a901e-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="a901e-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a901e-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="a901e-135">The default value is empty.</span></span> <span data-ttu-id="a901e-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a901e-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a901e-137">id</span><span class="sxs-lookup"><span data-stu-id="a901e-137">id</span></span>|<span data-ttu-id="a901e-138">String</span><span class="sxs-lookup"><span data-stu-id="a901e-138">String</span></span>|<span data-ttu-id="a901e-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a901e-139">Key of the entity.</span></span> <span data-ttu-id="a901e-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a901e-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a901e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a901e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a901e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a901e-142">DateTimeOffset</span></span>|<span data-ttu-id="a901e-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a901e-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="a901e-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a901e-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a901e-145">默认</span><span class="sxs-lookup"><span data-stu-id="a901e-145">defaultValue</span></span>|<span data-ttu-id="a901e-146">String</span><span class="sxs-lookup"><span data-stu-id="a901e-146">String</span></span>|<span data-ttu-id="a901e-147">组合框中显示的本地化默认字符串。</span><span class="sxs-lookup"><span data-stu-id="a901e-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="a901e-148">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="a901e-148">The default value is empty.</span></span>|
|<span data-ttu-id="a901e-149">推荐</span><span class="sxs-lookup"><span data-stu-id="a901e-149">suggestions</span></span>|<span data-ttu-id="a901e-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="a901e-150">String collection</span></span>|<span data-ttu-id="a901e-151">组合框下拉列表中列出的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="a901e-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="a901e-152">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="a901e-152">The default value is empty.</span></span>|
|<span data-ttu-id="a901e-153">必需</span><span class="sxs-lookup"><span data-stu-id="a901e-153">required</span></span>|<span data-ttu-id="a901e-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a901e-154">Boolean</span></span>|<span data-ttu-id="a901e-155">指定是否必须为参数指定值。</span><span class="sxs-lookup"><span data-stu-id="a901e-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="a901e-156">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="a901e-156">The default value is false.</span></span>|
|<span data-ttu-id="a901e-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="a901e-157">maxLength</span></span>|<span data-ttu-id="a901e-158">Int64</span><span class="sxs-lookup"><span data-stu-id="a901e-158">Int64</span></span>|<span data-ttu-id="a901e-159">一个无符号整数, 指定参数的最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="a901e-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="a901e-160">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="a901e-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="a901e-161">响应</span><span class="sxs-lookup"><span data-stu-id="a901e-161">Response</span></span>
<span data-ttu-id="a901e-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a901e-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a901e-163">示例</span><span class="sxs-lookup"><span data-stu-id="a901e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a901e-164">请求</span><span class="sxs-lookup"><span data-stu-id="a901e-164">Request</span></span>
<span data-ttu-id="a901e-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a901e-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a901e-166">响应</span><span class="sxs-lookup"><span data-stu-id="a901e-166">Response</span></span>
<span data-ttu-id="a901e-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a901e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




