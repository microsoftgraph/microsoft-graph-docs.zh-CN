---
title: 更新 groupPolicyPresentationComboBox
description: 更新 groupPolicyPresentationComboBox 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0059464113753cd9c504abe03947342a5855a11
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49308821"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="012d8-103">更新 groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="012d8-103">Update groupPolicyPresentationComboBox</span></span>

<span data-ttu-id="012d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="012d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="012d8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="012d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="012d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="012d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="012d8-107">更新 [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="012d8-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="012d8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="012d8-108">Prerequisites</span></span>
<span data-ttu-id="012d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="012d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="012d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="012d8-111">Permission type</span></span>|<span data-ttu-id="012d8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="012d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="012d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="012d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="012d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="012d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="012d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="012d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="012d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="012d8-116">Not supported.</span></span>|
|<span data-ttu-id="012d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="012d8-117">Application</span></span>|<span data-ttu-id="012d8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="012d8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="012d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="012d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="012d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="012d8-120">Request headers</span></span>
|<span data-ttu-id="012d8-121">标头</span><span class="sxs-lookup"><span data-stu-id="012d8-121">Header</span></span>|<span data-ttu-id="012d8-122">值</span><span class="sxs-lookup"><span data-stu-id="012d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="012d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="012d8-123">Authorization</span></span>|<span data-ttu-id="012d8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="012d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="012d8-125">接受</span><span class="sxs-lookup"><span data-stu-id="012d8-125">Accept</span></span>|<span data-ttu-id="012d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="012d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="012d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="012d8-127">Request body</span></span>
<span data-ttu-id="012d8-128">在请求正文中，提供 [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="012d8-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="012d8-129">下表显示创建 [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="012d8-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="012d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="012d8-130">Property</span></span>|<span data-ttu-id="012d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="012d8-131">Type</span></span>|<span data-ttu-id="012d8-132">Description</span><span class="sxs-lookup"><span data-stu-id="012d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="012d8-133">label</span><span class="sxs-lookup"><span data-stu-id="012d8-133">label</span></span>|<span data-ttu-id="012d8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="012d8-134">String</span></span>|<span data-ttu-id="012d8-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="012d8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="012d8-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="012d8-136">The default value is empty.</span></span> <span data-ttu-id="012d8-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="012d8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="012d8-138">id</span><span class="sxs-lookup"><span data-stu-id="012d8-138">id</span></span>|<span data-ttu-id="012d8-139">字符串</span><span class="sxs-lookup"><span data-stu-id="012d8-139">String</span></span>|<span data-ttu-id="012d8-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="012d8-140">Key of the entity.</span></span> <span data-ttu-id="012d8-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="012d8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="012d8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="012d8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="012d8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="012d8-143">DateTimeOffset</span></span>|<span data-ttu-id="012d8-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="012d8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="012d8-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="012d8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="012d8-146">默认</span><span class="sxs-lookup"><span data-stu-id="012d8-146">defaultValue</span></span>|<span data-ttu-id="012d8-147">字符串</span><span class="sxs-lookup"><span data-stu-id="012d8-147">String</span></span>|<span data-ttu-id="012d8-148">组合框中显示的本地化默认字符串。</span><span class="sxs-lookup"><span data-stu-id="012d8-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="012d8-149">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="012d8-149">The default value is empty.</span></span>|
|<span data-ttu-id="012d8-150">推荐</span><span class="sxs-lookup"><span data-stu-id="012d8-150">suggestions</span></span>|<span data-ttu-id="012d8-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="012d8-151">String collection</span></span>|<span data-ttu-id="012d8-152">组合框下拉列表中列出的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="012d8-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="012d8-153">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="012d8-153">The default value is empty.</span></span>|
|<span data-ttu-id="012d8-154">必需</span><span class="sxs-lookup"><span data-stu-id="012d8-154">required</span></span>|<span data-ttu-id="012d8-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="012d8-155">Boolean</span></span>|<span data-ttu-id="012d8-156">指定是否必须为参数指定值。</span><span class="sxs-lookup"><span data-stu-id="012d8-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="012d8-157">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="012d8-157">The default value is false.</span></span>|
|<span data-ttu-id="012d8-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="012d8-158">maxLength</span></span>|<span data-ttu-id="012d8-159">Int64</span><span class="sxs-lookup"><span data-stu-id="012d8-159">Int64</span></span>|<span data-ttu-id="012d8-160">一个无符号整数，指定参数的最大文本字符数。</span><span class="sxs-lookup"><span data-stu-id="012d8-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="012d8-161">默认值为1023。</span><span class="sxs-lookup"><span data-stu-id="012d8-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="012d8-162">响应</span><span class="sxs-lookup"><span data-stu-id="012d8-162">Response</span></span>
<span data-ttu-id="012d8-163">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="012d8-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="012d8-164">示例</span><span class="sxs-lookup"><span data-stu-id="012d8-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="012d8-165">请求</span><span class="sxs-lookup"><span data-stu-id="012d8-165">Request</span></span>
<span data-ttu-id="012d8-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="012d8-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="012d8-167">响应</span><span class="sxs-lookup"><span data-stu-id="012d8-167">Response</span></span>
<span data-ttu-id="012d8-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="012d8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




