---
title: 更新 groupPolicyPresentationDecimalTextBox
description: 更新 groupPolicyPresentationDecimalTextBox 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fc51623a43c84b9926c32c604e29c49e8795d54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464783"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="59f8f-103">更新 groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="59f8f-103">Update groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="59f8f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="59f8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59f8f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59f8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59f8f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59f8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59f8f-107">更新[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="59f8f-107">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59f8f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="59f8f-108">Prerequisites</span></span>
<span data-ttu-id="59f8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59f8f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="59f8f-111">Permission type</span></span>|<span data-ttu-id="59f8f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59f8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59f8f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59f8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59f8f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f8f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="59f8f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59f8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59f8f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59f8f-116">Not supported.</span></span>|
|<span data-ttu-id="59f8f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="59f8f-117">Application</span></span>|<span data-ttu-id="59f8f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f8f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59f8f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59f8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="59f8f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="59f8f-120">Request headers</span></span>
|<span data-ttu-id="59f8f-121">标头</span><span class="sxs-lookup"><span data-stu-id="59f8f-121">Header</span></span>|<span data-ttu-id="59f8f-122">值</span><span class="sxs-lookup"><span data-stu-id="59f8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59f8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59f8f-123">Authorization</span></span>|<span data-ttu-id="59f8f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="59f8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59f8f-125">接受</span><span class="sxs-lookup"><span data-stu-id="59f8f-125">Accept</span></span>|<span data-ttu-id="59f8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59f8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59f8f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59f8f-127">Request body</span></span>
<span data-ttu-id="59f8f-128">在请求正文中，提供[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59f8f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="59f8f-129">下表显示创建[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="59f8f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="59f8f-130">属性</span><span class="sxs-lookup"><span data-stu-id="59f8f-130">Property</span></span>|<span data-ttu-id="59f8f-131">类型</span><span class="sxs-lookup"><span data-stu-id="59f8f-131">Type</span></span>|<span data-ttu-id="59f8f-132">说明</span><span class="sxs-lookup"><span data-stu-id="59f8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59f8f-133">label</span><span class="sxs-lookup"><span data-stu-id="59f8f-133">label</span></span>|<span data-ttu-id="59f8f-134">String</span><span class="sxs-lookup"><span data-stu-id="59f8f-134">String</span></span>|<span data-ttu-id="59f8f-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="59f8f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="59f8f-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="59f8f-136">The default value is empty.</span></span> <span data-ttu-id="59f8f-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="59f8f-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="59f8f-138">id</span><span class="sxs-lookup"><span data-stu-id="59f8f-138">id</span></span>|<span data-ttu-id="59f8f-139">String</span><span class="sxs-lookup"><span data-stu-id="59f8f-139">String</span></span>|<span data-ttu-id="59f8f-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="59f8f-140">Key of the entity.</span></span> <span data-ttu-id="59f8f-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="59f8f-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="59f8f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59f8f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="59f8f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59f8f-143">DateTimeOffset</span></span>|<span data-ttu-id="59f8f-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="59f8f-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="59f8f-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="59f8f-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="59f8f-146">默认</span><span class="sxs-lookup"><span data-stu-id="59f8f-146">defaultValue</span></span>|<span data-ttu-id="59f8f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="59f8f-147">Int64</span></span>|<span data-ttu-id="59f8f-148">一个无符号整数，指定十进制文本框的初始值。</span><span class="sxs-lookup"><span data-stu-id="59f8f-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="59f8f-149">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="59f8f-149">The default value is 1.</span></span>|
|<span data-ttu-id="59f8f-150">派生</span><span class="sxs-lookup"><span data-stu-id="59f8f-150">spin</span></span>|<span data-ttu-id="59f8f-151">布尔</span><span class="sxs-lookup"><span data-stu-id="59f8f-151">Boolean</span></span>|<span data-ttu-id="59f8f-152">如果为 true，则创建数值调节钮控件;否则，请为数字输入创建文本框。</span><span class="sxs-lookup"><span data-stu-id="59f8f-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="59f8f-153">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="59f8f-153">The default value is true.</span></span>|
|<span data-ttu-id="59f8f-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="59f8f-154">spinStep</span></span>|<span data-ttu-id="59f8f-155">Int64</span><span class="sxs-lookup"><span data-stu-id="59f8f-155">Int64</span></span>|<span data-ttu-id="59f8f-156">一个无符号整数，指定数值调节钮控件的变化增量。</span><span class="sxs-lookup"><span data-stu-id="59f8f-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="59f8f-157">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="59f8f-157">The default value is 1.</span></span>|
|<span data-ttu-id="59f8f-158">必需</span><span class="sxs-lookup"><span data-stu-id="59f8f-158">required</span></span>|<span data-ttu-id="59f8f-159">布尔</span><span class="sxs-lookup"><span data-stu-id="59f8f-159">Boolean</span></span>|<span data-ttu-id="59f8f-160">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="59f8f-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="59f8f-161">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="59f8f-161">The default value is false.</span></span>|
|<span data-ttu-id="59f8f-162">minValue</span><span class="sxs-lookup"><span data-stu-id="59f8f-162">minValue</span></span>|<span data-ttu-id="59f8f-163">Int64</span><span class="sxs-lookup"><span data-stu-id="59f8f-163">Int64</span></span>|<span data-ttu-id="59f8f-164">一个无符号整数，指定允许的最小值。</span><span class="sxs-lookup"><span data-stu-id="59f8f-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="59f8f-165">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="59f8f-165">The default value is 0.</span></span>|
|<span data-ttu-id="59f8f-166">Timespan.maxvalue</span><span class="sxs-lookup"><span data-stu-id="59f8f-166">maxValue</span></span>|<span data-ttu-id="59f8f-167">Int64</span><span class="sxs-lookup"><span data-stu-id="59f8f-167">Int64</span></span>|<span data-ttu-id="59f8f-168">一个无符号整数，指定允许的最大值。</span><span class="sxs-lookup"><span data-stu-id="59f8f-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="59f8f-169">默认值为9999。</span><span class="sxs-lookup"><span data-stu-id="59f8f-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="59f8f-170">响应</span><span class="sxs-lookup"><span data-stu-id="59f8f-170">Response</span></span>
<span data-ttu-id="59f8f-171">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59f8f-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59f8f-172">示例</span><span class="sxs-lookup"><span data-stu-id="59f8f-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="59f8f-173">请求</span><span class="sxs-lookup"><span data-stu-id="59f8f-173">Request</span></span>
<span data-ttu-id="59f8f-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59f8f-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59f8f-175">响应</span><span class="sxs-lookup"><span data-stu-id="59f8f-175">Response</span></span>
<span data-ttu-id="59f8f-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59f8f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





