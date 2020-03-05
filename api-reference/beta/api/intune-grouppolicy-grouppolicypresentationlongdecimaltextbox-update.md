---
title: 更新 groupPolicyPresentationLongDecimalTextBox
description: 更新 groupPolicyPresentationLongDecimalTextBox 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af2cb713497e291e2ca3f58ad0c627b15837f9a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464580"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="6926b-103">更新 groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="6926b-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

<span data-ttu-id="6926b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6926b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6926b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6926b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6926b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6926b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6926b-107">更新[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6926b-107">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6926b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6926b-108">Prerequisites</span></span>
<span data-ttu-id="6926b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6926b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6926b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6926b-111">Permission type</span></span>|<span data-ttu-id="6926b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6926b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6926b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6926b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6926b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6926b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6926b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6926b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6926b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6926b-116">Not supported.</span></span>|
|<span data-ttu-id="6926b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6926b-117">Application</span></span>|<span data-ttu-id="6926b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6926b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6926b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6926b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="6926b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6926b-120">Request headers</span></span>
|<span data-ttu-id="6926b-121">标头</span><span class="sxs-lookup"><span data-stu-id="6926b-121">Header</span></span>|<span data-ttu-id="6926b-122">值</span><span class="sxs-lookup"><span data-stu-id="6926b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6926b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6926b-123">Authorization</span></span>|<span data-ttu-id="6926b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6926b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6926b-125">接受</span><span class="sxs-lookup"><span data-stu-id="6926b-125">Accept</span></span>|<span data-ttu-id="6926b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6926b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6926b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6926b-127">Request body</span></span>
<span data-ttu-id="6926b-128">在请求正文中，提供[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6926b-128">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="6926b-129">下表显示创建[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6926b-129">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="6926b-130">属性</span><span class="sxs-lookup"><span data-stu-id="6926b-130">Property</span></span>|<span data-ttu-id="6926b-131">类型</span><span class="sxs-lookup"><span data-stu-id="6926b-131">Type</span></span>|<span data-ttu-id="6926b-132">说明</span><span class="sxs-lookup"><span data-stu-id="6926b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6926b-133">label</span><span class="sxs-lookup"><span data-stu-id="6926b-133">label</span></span>|<span data-ttu-id="6926b-134">String</span><span class="sxs-lookup"><span data-stu-id="6926b-134">String</span></span>|<span data-ttu-id="6926b-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="6926b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6926b-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="6926b-136">The default value is empty.</span></span> <span data-ttu-id="6926b-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6926b-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6926b-138">id</span><span class="sxs-lookup"><span data-stu-id="6926b-138">id</span></span>|<span data-ttu-id="6926b-139">String</span><span class="sxs-lookup"><span data-stu-id="6926b-139">String</span></span>|<span data-ttu-id="6926b-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6926b-140">Key of the entity.</span></span> <span data-ttu-id="6926b-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6926b-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6926b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6926b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="6926b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6926b-143">DateTimeOffset</span></span>|<span data-ttu-id="6926b-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6926b-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="6926b-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6926b-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6926b-146">默认</span><span class="sxs-lookup"><span data-stu-id="6926b-146">defaultValue</span></span>|<span data-ttu-id="6926b-147">Int64</span><span class="sxs-lookup"><span data-stu-id="6926b-147">Int64</span></span>|<span data-ttu-id="6926b-148">一个无符号整数，指定十进制文本框的初始值。</span><span class="sxs-lookup"><span data-stu-id="6926b-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="6926b-149">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="6926b-149">The default value is 1.</span></span>|
|<span data-ttu-id="6926b-150">派生</span><span class="sxs-lookup"><span data-stu-id="6926b-150">spin</span></span>|<span data-ttu-id="6926b-151">布尔</span><span class="sxs-lookup"><span data-stu-id="6926b-151">Boolean</span></span>|<span data-ttu-id="6926b-152">如果为 true，则创建数值调节钮控件;否则，请为数字输入创建文本框。</span><span class="sxs-lookup"><span data-stu-id="6926b-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="6926b-153">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="6926b-153">The default value is true.</span></span>|
|<span data-ttu-id="6926b-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="6926b-154">spinStep</span></span>|<span data-ttu-id="6926b-155">Int64</span><span class="sxs-lookup"><span data-stu-id="6926b-155">Int64</span></span>|<span data-ttu-id="6926b-156">一个无符号整数，指定数值调节钮控件的变化增量。</span><span class="sxs-lookup"><span data-stu-id="6926b-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="6926b-157">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="6926b-157">The default value is 1.</span></span>|
|<span data-ttu-id="6926b-158">必需</span><span class="sxs-lookup"><span data-stu-id="6926b-158">required</span></span>|<span data-ttu-id="6926b-159">布尔</span><span class="sxs-lookup"><span data-stu-id="6926b-159">Boolean</span></span>|<span data-ttu-id="6926b-160">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="6926b-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="6926b-161">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="6926b-161">The default value is false.</span></span>|
|<span data-ttu-id="6926b-162">minValue</span><span class="sxs-lookup"><span data-stu-id="6926b-162">minValue</span></span>|<span data-ttu-id="6926b-163">Int64</span><span class="sxs-lookup"><span data-stu-id="6926b-163">Int64</span></span>|<span data-ttu-id="6926b-164">一个无符号的 long，指定允许的最小值。</span><span class="sxs-lookup"><span data-stu-id="6926b-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="6926b-165">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="6926b-165">The default value is 0.</span></span>|
|<span data-ttu-id="6926b-166">Timespan.maxvalue</span><span class="sxs-lookup"><span data-stu-id="6926b-166">maxValue</span></span>|<span data-ttu-id="6926b-167">Int64</span><span class="sxs-lookup"><span data-stu-id="6926b-167">Int64</span></span>|<span data-ttu-id="6926b-168">一个无符号的 long，指定允许的最大值。</span><span class="sxs-lookup"><span data-stu-id="6926b-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="6926b-169">默认值为9999。</span><span class="sxs-lookup"><span data-stu-id="6926b-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="6926b-170">响应</span><span class="sxs-lookup"><span data-stu-id="6926b-170">Response</span></span>
<span data-ttu-id="6926b-171">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6926b-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6926b-172">示例</span><span class="sxs-lookup"><span data-stu-id="6926b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6926b-173">请求</span><span class="sxs-lookup"><span data-stu-id="6926b-173">Request</span></span>
<span data-ttu-id="6926b-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6926b-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="6926b-175">响应</span><span class="sxs-lookup"><span data-stu-id="6926b-175">Response</span></span>
<span data-ttu-id="6926b-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6926b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "id": "754d8495-8495-754d-9584-4d7595844d75",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```





