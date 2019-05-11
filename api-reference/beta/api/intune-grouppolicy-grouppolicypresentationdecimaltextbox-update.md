---
title: 更新 groupPolicyPresentationDecimalTextBox
description: 更新 groupPolicyPresentationDecimalTextBox 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83ef5a7acfb16607719a5bc1a064d3f841c139a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904900"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="684ce-103">更新 groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="684ce-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="684ce-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="684ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="684ce-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="684ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="684ce-106">更新[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="684ce-106">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="684ce-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="684ce-107">Prerequisites</span></span>
<span data-ttu-id="684ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="684ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="684ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="684ce-110">Permission type</span></span>|<span data-ttu-id="684ce-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="684ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="684ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="684ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="684ce-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="684ce-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="684ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="684ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="684ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="684ce-115">Not supported.</span></span>|
|<span data-ttu-id="684ce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="684ce-116">Application</span></span>|<span data-ttu-id="684ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="684ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="684ce-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="684ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="684ce-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="684ce-119">Request headers</span></span>
|<span data-ttu-id="684ce-120">标头</span><span class="sxs-lookup"><span data-stu-id="684ce-120">Header</span></span>|<span data-ttu-id="684ce-121">值</span><span class="sxs-lookup"><span data-stu-id="684ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="684ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="684ce-122">Authorization</span></span>|<span data-ttu-id="684ce-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="684ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="684ce-124">接受</span><span class="sxs-lookup"><span data-stu-id="684ce-124">Accept</span></span>|<span data-ttu-id="684ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="684ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="684ce-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="684ce-126">Request body</span></span>
<span data-ttu-id="684ce-127">在请求正文中, 提供[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="684ce-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="684ce-128">下表显示创建[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="684ce-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="684ce-129">属性</span><span class="sxs-lookup"><span data-stu-id="684ce-129">Property</span></span>|<span data-ttu-id="684ce-130">类型</span><span class="sxs-lookup"><span data-stu-id="684ce-130">Type</span></span>|<span data-ttu-id="684ce-131">说明</span><span class="sxs-lookup"><span data-stu-id="684ce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="684ce-132">label</span><span class="sxs-lookup"><span data-stu-id="684ce-132">label</span></span>|<span data-ttu-id="684ce-133">String</span><span class="sxs-lookup"><span data-stu-id="684ce-133">String</span></span>|<span data-ttu-id="684ce-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="684ce-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="684ce-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="684ce-135">The default value is empty.</span></span> <span data-ttu-id="684ce-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="684ce-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="684ce-137">id</span><span class="sxs-lookup"><span data-stu-id="684ce-137">id</span></span>|<span data-ttu-id="684ce-138">String</span><span class="sxs-lookup"><span data-stu-id="684ce-138">String</span></span>|<span data-ttu-id="684ce-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="684ce-139">Key of the entity.</span></span> <span data-ttu-id="684ce-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="684ce-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="684ce-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="684ce-141">lastModifiedDateTime</span></span>|<span data-ttu-id="684ce-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="684ce-142">DateTimeOffset</span></span>|<span data-ttu-id="684ce-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="684ce-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="684ce-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="684ce-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="684ce-145">默认</span><span class="sxs-lookup"><span data-stu-id="684ce-145">defaultValue</span></span>|<span data-ttu-id="684ce-146">Int64</span><span class="sxs-lookup"><span data-stu-id="684ce-146">Int64</span></span>|<span data-ttu-id="684ce-147">一个无符号整数, 指定十进制文本框的初始值。</span><span class="sxs-lookup"><span data-stu-id="684ce-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="684ce-148">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="684ce-148">The default value is 1.</span></span>|
|<span data-ttu-id="684ce-149">派生</span><span class="sxs-lookup"><span data-stu-id="684ce-149">spin</span></span>|<span data-ttu-id="684ce-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="684ce-150">Boolean</span></span>|<span data-ttu-id="684ce-151">如果为 true, 则创建数值调节钮控件;否则, 请为数字输入创建文本框。</span><span class="sxs-lookup"><span data-stu-id="684ce-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="684ce-152">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="684ce-152">The default value is true.</span></span>|
|<span data-ttu-id="684ce-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="684ce-153">spinStep</span></span>|<span data-ttu-id="684ce-154">Int64</span><span class="sxs-lookup"><span data-stu-id="684ce-154">Int64</span></span>|<span data-ttu-id="684ce-155">一个无符号整数, 指定数值调节钮控件的变化增量。</span><span class="sxs-lookup"><span data-stu-id="684ce-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="684ce-156">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="684ce-156">The default value is 1.</span></span>|
|<span data-ttu-id="684ce-157">必需</span><span class="sxs-lookup"><span data-stu-id="684ce-157">required</span></span>|<span data-ttu-id="684ce-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="684ce-158">Boolean</span></span>|<span data-ttu-id="684ce-159">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="684ce-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="684ce-160">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="684ce-160">The default value is false.</span></span>|
|<span data-ttu-id="684ce-161">minValue</span><span class="sxs-lookup"><span data-stu-id="684ce-161">minValue</span></span>|<span data-ttu-id="684ce-162">Int64</span><span class="sxs-lookup"><span data-stu-id="684ce-162">Int64</span></span>|<span data-ttu-id="684ce-163">一个无符号整数, 指定允许的最小值。</span><span class="sxs-lookup"><span data-stu-id="684ce-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="684ce-164">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="684ce-164">The default value is 0.</span></span>|
|<span data-ttu-id="684ce-165">Timespan.maxvalue</span><span class="sxs-lookup"><span data-stu-id="684ce-165">maxValue</span></span>|<span data-ttu-id="684ce-166">Int64</span><span class="sxs-lookup"><span data-stu-id="684ce-166">Int64</span></span>|<span data-ttu-id="684ce-167">一个无符号整数, 指定允许的最大值。</span><span class="sxs-lookup"><span data-stu-id="684ce-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="684ce-168">默认值为9999。</span><span class="sxs-lookup"><span data-stu-id="684ce-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="684ce-169">响应</span><span class="sxs-lookup"><span data-stu-id="684ce-169">Response</span></span>
<span data-ttu-id="684ce-170">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="684ce-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="684ce-171">示例</span><span class="sxs-lookup"><span data-stu-id="684ce-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="684ce-172">请求</span><span class="sxs-lookup"><span data-stu-id="684ce-172">Request</span></span>
<span data-ttu-id="684ce-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="684ce-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="684ce-174">响应</span><span class="sxs-lookup"><span data-stu-id="684ce-174">Response</span></span>
<span data-ttu-id="684ce-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="684ce-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




