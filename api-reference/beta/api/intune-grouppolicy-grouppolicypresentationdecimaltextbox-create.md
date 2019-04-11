---
title: 创建 groupPolicyPresentationDecimalTextBox
description: 创建新的 groupPolicyPresentationDecimalTextBox 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45a930e1973c00f7ec3ad67fe8d0ed863ab2a7f7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802287"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="1bd31-103">创建 groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="1bd31-103">Create groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="1bd31-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1bd31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bd31-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1bd31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd31-106">创建新的[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1bd31-106">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bd31-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bd31-107">Prerequisites</span></span>
<span data-ttu-id="1bd31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bd31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd31-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bd31-110">Permission type</span></span>|<span data-ttu-id="1bd31-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bd31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bd31-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bd31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bd31-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd31-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1bd31-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bd31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bd31-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bd31-115">Not supported.</span></span>|
|<span data-ttu-id="1bd31-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bd31-116">Application</span></span>|<span data-ttu-id="1bd31-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bd31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bd31-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bd31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="1bd31-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bd31-119">Request headers</span></span>
|<span data-ttu-id="1bd31-120">标头</span><span class="sxs-lookup"><span data-stu-id="1bd31-120">Header</span></span>|<span data-ttu-id="1bd31-121">值</span><span class="sxs-lookup"><span data-stu-id="1bd31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bd31-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bd31-122">Authorization</span></span>|<span data-ttu-id="1bd31-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bd31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bd31-124">接受</span><span class="sxs-lookup"><span data-stu-id="1bd31-124">Accept</span></span>|<span data-ttu-id="1bd31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1bd31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bd31-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bd31-126">Request body</span></span>
<span data-ttu-id="1bd31-127">在请求正文中, 提供 groupPolicyPresentationDecimalTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bd31-127">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="1bd31-128">下表显示创建 groupPolicyPresentationDecimalTextBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1bd31-128">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="1bd31-129">属性</span><span class="sxs-lookup"><span data-stu-id="1bd31-129">Property</span></span>|<span data-ttu-id="1bd31-130">类型</span><span class="sxs-lookup"><span data-stu-id="1bd31-130">Type</span></span>|<span data-ttu-id="1bd31-131">说明</span><span class="sxs-lookup"><span data-stu-id="1bd31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd31-132">label</span><span class="sxs-lookup"><span data-stu-id="1bd31-132">label</span></span>|<span data-ttu-id="1bd31-133">String</span><span class="sxs-lookup"><span data-stu-id="1bd31-133">String</span></span>|<span data-ttu-id="1bd31-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="1bd31-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="1bd31-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="1bd31-135">The default value is empty.</span></span> <span data-ttu-id="1bd31-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1bd31-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1bd31-137">id</span><span class="sxs-lookup"><span data-stu-id="1bd31-137">id</span></span>|<span data-ttu-id="1bd31-138">String</span><span class="sxs-lookup"><span data-stu-id="1bd31-138">String</span></span>|<span data-ttu-id="1bd31-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1bd31-139">Key of the entity.</span></span> <span data-ttu-id="1bd31-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1bd31-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1bd31-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1bd31-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1bd31-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bd31-142">DateTimeOffset</span></span>|<span data-ttu-id="1bd31-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1bd31-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="1bd31-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1bd31-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1bd31-145">默认</span><span class="sxs-lookup"><span data-stu-id="1bd31-145">defaultValue</span></span>|<span data-ttu-id="1bd31-146">Int64</span><span class="sxs-lookup"><span data-stu-id="1bd31-146">Int64</span></span>|<span data-ttu-id="1bd31-147">一个无符号整数, 指定十进制文本框的初始值。</span><span class="sxs-lookup"><span data-stu-id="1bd31-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="1bd31-148">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="1bd31-148">The default value is 1.</span></span>|
|<span data-ttu-id="1bd31-149">派生</span><span class="sxs-lookup"><span data-stu-id="1bd31-149">spin</span></span>|<span data-ttu-id="1bd31-150">布尔值</span><span class="sxs-lookup"><span data-stu-id="1bd31-150">Boolean</span></span>|<span data-ttu-id="1bd31-151">如果为 true, 则创建数值调节钮控件;否则, 请为数字输入创建文本框。</span><span class="sxs-lookup"><span data-stu-id="1bd31-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="1bd31-152">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="1bd31-152">The default value is true.</span></span>|
|<span data-ttu-id="1bd31-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="1bd31-153">spinStep</span></span>|<span data-ttu-id="1bd31-154">Int64</span><span class="sxs-lookup"><span data-stu-id="1bd31-154">Int64</span></span>|<span data-ttu-id="1bd31-155">一个无符号整数, 指定数值调节钮控件的变化增量。</span><span class="sxs-lookup"><span data-stu-id="1bd31-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="1bd31-156">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="1bd31-156">The default value is 1.</span></span>|
|<span data-ttu-id="1bd31-157">必需</span><span class="sxs-lookup"><span data-stu-id="1bd31-157">required</span></span>|<span data-ttu-id="1bd31-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="1bd31-158">Boolean</span></span>|<span data-ttu-id="1bd31-159">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="1bd31-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="1bd31-160">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="1bd31-160">The default value is false.</span></span>|
|<span data-ttu-id="1bd31-161">minValue</span><span class="sxs-lookup"><span data-stu-id="1bd31-161">minValue</span></span>|<span data-ttu-id="1bd31-162">Int64</span><span class="sxs-lookup"><span data-stu-id="1bd31-162">Int64</span></span>|<span data-ttu-id="1bd31-163">一个无符号整数, 指定允许的最小值。</span><span class="sxs-lookup"><span data-stu-id="1bd31-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="1bd31-164">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="1bd31-164">The default value is 0.</span></span>|
|<span data-ttu-id="1bd31-165">timespan.maxvalue</span><span class="sxs-lookup"><span data-stu-id="1bd31-165">maxValue</span></span>|<span data-ttu-id="1bd31-166">Int64</span><span class="sxs-lookup"><span data-stu-id="1bd31-166">Int64</span></span>|<span data-ttu-id="1bd31-167">一个无符号整数, 指定允许的最大值。</span><span class="sxs-lookup"><span data-stu-id="1bd31-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="1bd31-168">默认值为9999。</span><span class="sxs-lookup"><span data-stu-id="1bd31-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="1bd31-169">响应</span><span class="sxs-lookup"><span data-stu-id="1bd31-169">Response</span></span>
<span data-ttu-id="1bd31-170">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1bd31-170">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bd31-171">示例</span><span class="sxs-lookup"><span data-stu-id="1bd31-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bd31-172">请求</span><span class="sxs-lookup"><span data-stu-id="1bd31-172">Request</span></span>
<span data-ttu-id="1bd31-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bd31-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1bd31-174">响应</span><span class="sxs-lookup"><span data-stu-id="1bd31-174">Response</span></span>
<span data-ttu-id="1bd31-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bd31-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





