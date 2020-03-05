---
title: 创建 groupPolicyPresentationDecimalTextBox
description: 创建新的 groupPolicyPresentationDecimalTextBox 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93581dd5a12be1b6a8cec8944f97cefe8ed93dfa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464860"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="8d0e7-103">创建 groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="8d0e7-103">Create groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="8d0e7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8d0e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d0e7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d0e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d0e7-107">创建新的[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-107">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d0e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d0e7-108">Prerequisites</span></span>
<span data-ttu-id="8d0e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d0e7-111">Permission type</span></span>|<span data-ttu-id="8d0e7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8d0e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d0e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d0e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d0e7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0e7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d0e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d0e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d0e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-116">Not supported.</span></span>|
|<span data-ttu-id="8d0e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d0e7-117">Application</span></span>|<span data-ttu-id="8d0e7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0e7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d0e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d0e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="8d0e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d0e7-120">Request headers</span></span>
|<span data-ttu-id="8d0e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="8d0e7-121">Header</span></span>|<span data-ttu-id="8d0e7-122">值</span><span class="sxs-lookup"><span data-stu-id="8d0e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d0e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d0e7-123">Authorization</span></span>|<span data-ttu-id="8d0e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d0e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="8d0e7-125">Accept</span></span>|<span data-ttu-id="8d0e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d0e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d0e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d0e7-127">Request body</span></span>
<span data-ttu-id="8d0e7-128">在请求正文中，提供 groupPolicyPresentationDecimalTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-128">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="8d0e7-129">下表显示创建 groupPolicyPresentationDecimalTextBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-129">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="8d0e7-130">属性</span><span class="sxs-lookup"><span data-stu-id="8d0e7-130">Property</span></span>|<span data-ttu-id="8d0e7-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d0e7-131">Type</span></span>|<span data-ttu-id="8d0e7-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d0e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d0e7-133">label</span><span class="sxs-lookup"><span data-stu-id="8d0e7-133">label</span></span>|<span data-ttu-id="8d0e7-134">String</span><span class="sxs-lookup"><span data-stu-id="8d0e7-134">String</span></span>|<span data-ttu-id="8d0e7-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="8d0e7-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-136">The default value is empty.</span></span> <span data-ttu-id="8d0e7-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e7-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8d0e7-138">id</span><span class="sxs-lookup"><span data-stu-id="8d0e7-138">id</span></span>|<span data-ttu-id="8d0e7-139">String</span><span class="sxs-lookup"><span data-stu-id="8d0e7-139">String</span></span>|<span data-ttu-id="8d0e7-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-140">Key of the entity.</span></span> <span data-ttu-id="8d0e7-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e7-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8d0e7-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d0e7-142">lastModifiedDateTime</span></span>|<span data-ttu-id="8d0e7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d0e7-143">DateTimeOffset</span></span>|<span data-ttu-id="8d0e7-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="8d0e7-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e7-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8d0e7-146">默认</span><span class="sxs-lookup"><span data-stu-id="8d0e7-146">defaultValue</span></span>|<span data-ttu-id="8d0e7-147">Int64</span><span class="sxs-lookup"><span data-stu-id="8d0e7-147">Int64</span></span>|<span data-ttu-id="8d0e7-148">一个无符号整数，指定十进制文本框的初始值。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="8d0e7-149">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-149">The default value is 1.</span></span>|
|<span data-ttu-id="8d0e7-150">派生</span><span class="sxs-lookup"><span data-stu-id="8d0e7-150">spin</span></span>|<span data-ttu-id="8d0e7-151">布尔</span><span class="sxs-lookup"><span data-stu-id="8d0e7-151">Boolean</span></span>|<span data-ttu-id="8d0e7-152">如果为 true，则创建数值调节钮控件;否则，请为数字输入创建文本框。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="8d0e7-153">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-153">The default value is true.</span></span>|
|<span data-ttu-id="8d0e7-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="8d0e7-154">spinStep</span></span>|<span data-ttu-id="8d0e7-155">Int64</span><span class="sxs-lookup"><span data-stu-id="8d0e7-155">Int64</span></span>|<span data-ttu-id="8d0e7-156">一个无符号整数，指定数值调节钮控件的变化增量。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="8d0e7-157">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-157">The default value is 1.</span></span>|
|<span data-ttu-id="8d0e7-158">必需</span><span class="sxs-lookup"><span data-stu-id="8d0e7-158">required</span></span>|<span data-ttu-id="8d0e7-159">布尔</span><span class="sxs-lookup"><span data-stu-id="8d0e7-159">Boolean</span></span>|<span data-ttu-id="8d0e7-160">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="8d0e7-161">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-161">The default value is false.</span></span>|
|<span data-ttu-id="8d0e7-162">minValue</span><span class="sxs-lookup"><span data-stu-id="8d0e7-162">minValue</span></span>|<span data-ttu-id="8d0e7-163">Int64</span><span class="sxs-lookup"><span data-stu-id="8d0e7-163">Int64</span></span>|<span data-ttu-id="8d0e7-164">一个无符号整数，指定允许的最小值。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="8d0e7-165">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-165">The default value is 0.</span></span>|
|<span data-ttu-id="8d0e7-166">Timespan.maxvalue</span><span class="sxs-lookup"><span data-stu-id="8d0e7-166">maxValue</span></span>|<span data-ttu-id="8d0e7-167">Int64</span><span class="sxs-lookup"><span data-stu-id="8d0e7-167">Int64</span></span>|<span data-ttu-id="8d0e7-168">一个无符号整数，指定允许的最大值。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="8d0e7-169">默认值为9999。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="8d0e7-170">响应</span><span class="sxs-lookup"><span data-stu-id="8d0e7-170">Response</span></span>
<span data-ttu-id="8d0e7-171">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d0e7-172">示例</span><span class="sxs-lookup"><span data-stu-id="8d0e7-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d0e7-173">请求</span><span class="sxs-lookup"><span data-stu-id="8d0e7-173">Request</span></span>
<span data-ttu-id="8d0e7-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="8d0e7-175">响应</span><span class="sxs-lookup"><span data-stu-id="8d0e7-175">Response</span></span>
<span data-ttu-id="8d0e7-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d0e7-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```





