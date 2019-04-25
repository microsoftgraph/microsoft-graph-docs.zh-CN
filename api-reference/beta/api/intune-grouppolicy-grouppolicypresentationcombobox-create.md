---
title: 创建 groupPolicyPresentationComboBox
description: 创建新的 groupPolicyPresentationComboBox 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ca375a771856f314563e2780128fc7d8aab3c88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531171"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="ffabe-103">创建 groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="ffabe-103">Create groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="ffabe-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffabe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffabe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffabe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffabe-106">创建新的[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffabe-106">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffabe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffabe-107">Prerequisites</span></span>
<span data-ttu-id="ffabe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffabe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffabe-110">Permission type</span></span>|<span data-ttu-id="ffabe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffabe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffabe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffabe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffabe-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffabe-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ffabe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffabe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffabe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffabe-115">Not supported.</span></span>|
|<span data-ttu-id="ffabe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffabe-116">Application</span></span>|<span data-ttu-id="ffabe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffabe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffabe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffabe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="ffabe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffabe-119">Request headers</span></span>
|<span data-ttu-id="ffabe-120">标头</span><span class="sxs-lookup"><span data-stu-id="ffabe-120">Header</span></span>|<span data-ttu-id="ffabe-121">值</span><span class="sxs-lookup"><span data-stu-id="ffabe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffabe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffabe-122">Authorization</span></span>|<span data-ttu-id="ffabe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffabe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffabe-124">接受</span><span class="sxs-lookup"><span data-stu-id="ffabe-124">Accept</span></span>|<span data-ttu-id="ffabe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffabe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffabe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffabe-126">Request body</span></span>
<span data-ttu-id="ffabe-127">在请求正文中, 提供 groupPolicyPresentationComboBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffabe-127">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="ffabe-128">下表显示创建 groupPolicyPresentationComboBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ffabe-128">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="ffabe-129">属性</span><span class="sxs-lookup"><span data-stu-id="ffabe-129">Property</span></span>|<span data-ttu-id="ffabe-130">类型</span><span class="sxs-lookup"><span data-stu-id="ffabe-130">Type</span></span>|<span data-ttu-id="ffabe-131">说明</span><span class="sxs-lookup"><span data-stu-id="ffabe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffabe-132">label</span><span class="sxs-lookup"><span data-stu-id="ffabe-132">label</span></span>|<span data-ttu-id="ffabe-133">String</span><span class="sxs-lookup"><span data-stu-id="ffabe-133">String</span></span>|<span data-ttu-id="ffabe-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="ffabe-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ffabe-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="ffabe-135">The default value is empty.</span></span> <span data-ttu-id="ffabe-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ffabe-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ffabe-137">id</span><span class="sxs-lookup"><span data-stu-id="ffabe-137">id</span></span>|<span data-ttu-id="ffabe-138">String</span><span class="sxs-lookup"><span data-stu-id="ffabe-138">String</span></span>|<span data-ttu-id="ffabe-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ffabe-139">Key of the entity.</span></span> <span data-ttu-id="ffabe-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ffabe-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ffabe-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffabe-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ffabe-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffabe-142">DateTimeOffset</span></span>|<span data-ttu-id="ffabe-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ffabe-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="ffabe-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ffabe-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ffabe-145">默认</span><span class="sxs-lookup"><span data-stu-id="ffabe-145">defaultValue</span></span>|<span data-ttu-id="ffabe-146">String</span><span class="sxs-lookup"><span data-stu-id="ffabe-146">String</span></span>|<span data-ttu-id="ffabe-147">组合框中显示的本地化默认字符串。</span><span class="sxs-lookup"><span data-stu-id="ffabe-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="ffabe-148">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="ffabe-148">The default value is empty.</span></span>|
|<span data-ttu-id="ffabe-149">推荐</span><span class="sxs-lookup"><span data-stu-id="ffabe-149">suggestions</span></span>|<span data-ttu-id="ffabe-150">String collection</span><span class="sxs-lookup"><span data-stu-id="ffabe-150">String collection</span></span>|<span data-ttu-id="ffabe-151">组合框下拉列表中列出的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="ffabe-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="ffabe-152">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="ffabe-152">The default value is empty.</span></span>|
|<span data-ttu-id="ffabe-153">必需</span><span class="sxs-lookup"><span data-stu-id="ffabe-153">required</span></span>|<span data-ttu-id="ffabe-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="ffabe-154">Boolean</span></span>|<span data-ttu-id="ffabe-155">指定是否必须为参数指定值。</span><span class="sxs-lookup"><span data-stu-id="ffabe-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="ffabe-156">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="ffabe-156">The default value is false.</span></span>|
|<span data-ttu-id="ffabe-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="ffabe-157">maxLength</span></span>|<span data-ttu-id="ffabe-158">Int64</span><span class="sxs-lookup"><span data-stu-id="ffabe-158">Int64</span></span>|<span data-ttu-id="ffabe-159">一个无符号整数, 指定参数的最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="ffabe-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="ffabe-160">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="ffabe-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="ffabe-161">响应</span><span class="sxs-lookup"><span data-stu-id="ffabe-161">Response</span></span>
<span data-ttu-id="ffabe-162">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffabe-162">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffabe-163">示例</span><span class="sxs-lookup"><span data-stu-id="ffabe-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffabe-164">请求</span><span class="sxs-lookup"><span data-stu-id="ffabe-164">Request</span></span>
<span data-ttu-id="ffabe-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffabe-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ffabe-166">响应</span><span class="sxs-lookup"><span data-stu-id="ffabe-166">Response</span></span>
<span data-ttu-id="ffabe-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffabe-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





