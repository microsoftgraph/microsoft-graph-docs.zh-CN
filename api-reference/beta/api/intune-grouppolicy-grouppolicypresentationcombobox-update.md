---
title: 更新 groupPolicyPresentationComboBox
description: 更新 groupPolicyPresentationComboBox 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07b286b58a478e2b91446dfba9fd849b5621940f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464853"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="03bd6-103">更新 groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="03bd6-103">Update groupPolicyPresentationComboBox</span></span>

<span data-ttu-id="03bd6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="03bd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03bd6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03bd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03bd6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03bd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03bd6-107">更新[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03bd6-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03bd6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03bd6-108">Prerequisites</span></span>
<span data-ttu-id="03bd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03bd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03bd6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03bd6-111">Permission type</span></span>|<span data-ttu-id="03bd6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03bd6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03bd6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03bd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03bd6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bd6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="03bd6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03bd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03bd6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03bd6-116">Not supported.</span></span>|
|<span data-ttu-id="03bd6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03bd6-117">Application</span></span>|<span data-ttu-id="03bd6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bd6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03bd6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03bd6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="03bd6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03bd6-120">Request headers</span></span>
|<span data-ttu-id="03bd6-121">标头</span><span class="sxs-lookup"><span data-stu-id="03bd6-121">Header</span></span>|<span data-ttu-id="03bd6-122">值</span><span class="sxs-lookup"><span data-stu-id="03bd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03bd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03bd6-123">Authorization</span></span>|<span data-ttu-id="03bd6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03bd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03bd6-125">接受</span><span class="sxs-lookup"><span data-stu-id="03bd6-125">Accept</span></span>|<span data-ttu-id="03bd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03bd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03bd6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03bd6-127">Request body</span></span>
<span data-ttu-id="03bd6-128">在请求正文中，提供[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03bd6-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="03bd6-129">下表显示创建[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03bd6-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="03bd6-130">属性</span><span class="sxs-lookup"><span data-stu-id="03bd6-130">Property</span></span>|<span data-ttu-id="03bd6-131">类型</span><span class="sxs-lookup"><span data-stu-id="03bd6-131">Type</span></span>|<span data-ttu-id="03bd6-132">说明</span><span class="sxs-lookup"><span data-stu-id="03bd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03bd6-133">label</span><span class="sxs-lookup"><span data-stu-id="03bd6-133">label</span></span>|<span data-ttu-id="03bd6-134">String</span><span class="sxs-lookup"><span data-stu-id="03bd6-134">String</span></span>|<span data-ttu-id="03bd6-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="03bd6-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="03bd6-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="03bd6-136">The default value is empty.</span></span> <span data-ttu-id="03bd6-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="03bd6-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="03bd6-138">id</span><span class="sxs-lookup"><span data-stu-id="03bd6-138">id</span></span>|<span data-ttu-id="03bd6-139">String</span><span class="sxs-lookup"><span data-stu-id="03bd6-139">String</span></span>|<span data-ttu-id="03bd6-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="03bd6-140">Key of the entity.</span></span> <span data-ttu-id="03bd6-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="03bd6-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="03bd6-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03bd6-142">lastModifiedDateTime</span></span>|<span data-ttu-id="03bd6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03bd6-143">DateTimeOffset</span></span>|<span data-ttu-id="03bd6-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="03bd6-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="03bd6-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="03bd6-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="03bd6-146">默认</span><span class="sxs-lookup"><span data-stu-id="03bd6-146">defaultValue</span></span>|<span data-ttu-id="03bd6-147">String</span><span class="sxs-lookup"><span data-stu-id="03bd6-147">String</span></span>|<span data-ttu-id="03bd6-148">组合框中显示的本地化默认字符串。</span><span class="sxs-lookup"><span data-stu-id="03bd6-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="03bd6-149">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="03bd6-149">The default value is empty.</span></span>|
|<span data-ttu-id="03bd6-150">推荐</span><span class="sxs-lookup"><span data-stu-id="03bd6-150">suggestions</span></span>|<span data-ttu-id="03bd6-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="03bd6-151">String collection</span></span>|<span data-ttu-id="03bd6-152">组合框下拉列表中列出的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="03bd6-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="03bd6-153">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="03bd6-153">The default value is empty.</span></span>|
|<span data-ttu-id="03bd6-154">必需</span><span class="sxs-lookup"><span data-stu-id="03bd6-154">required</span></span>|<span data-ttu-id="03bd6-155">布尔</span><span class="sxs-lookup"><span data-stu-id="03bd6-155">Boolean</span></span>|<span data-ttu-id="03bd6-156">指定是否必须为参数指定值。</span><span class="sxs-lookup"><span data-stu-id="03bd6-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="03bd6-157">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="03bd6-157">The default value is false.</span></span>|
|<span data-ttu-id="03bd6-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="03bd6-158">maxLength</span></span>|<span data-ttu-id="03bd6-159">Int64</span><span class="sxs-lookup"><span data-stu-id="03bd6-159">Int64</span></span>|<span data-ttu-id="03bd6-160">一个无符号整数，指定参数的最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="03bd6-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="03bd6-161">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="03bd6-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="03bd6-162">响应</span><span class="sxs-lookup"><span data-stu-id="03bd6-162">Response</span></span>
<span data-ttu-id="03bd6-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="03bd6-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03bd6-164">示例</span><span class="sxs-lookup"><span data-stu-id="03bd6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="03bd6-165">请求</span><span class="sxs-lookup"><span data-stu-id="03bd6-165">Request</span></span>
<span data-ttu-id="03bd6-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03bd6-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03bd6-167">响应</span><span class="sxs-lookup"><span data-stu-id="03bd6-167">Response</span></span>
<span data-ttu-id="03bd6-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03bd6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





