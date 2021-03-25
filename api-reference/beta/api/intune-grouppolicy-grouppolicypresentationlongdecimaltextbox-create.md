---
title: 创建 groupPolicyPresentationLongDecimalTextBox
description: 创建新的 groupPolicyPresentationLongDecimalTextBox 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5de88999c439ef4a7b6ec8d9316dd32cfd54e94d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153305"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="7d41a-103">创建 groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="7d41a-103">Create groupPolicyPresentationLongDecimalTextBox</span></span>

<span data-ttu-id="7d41a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d41a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d41a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d41a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d41a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d41a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d41a-107">创建新的 [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d41a-107">Create a new [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d41a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7d41a-108">Prerequisites</span></span>
<span data-ttu-id="7d41a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d41a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d41a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d41a-111">Permission type</span></span>|<span data-ttu-id="7d41a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d41a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d41a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d41a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d41a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d41a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d41a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d41a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d41a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d41a-116">Not supported.</span></span>|
|<span data-ttu-id="7d41a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d41a-117">Application</span></span>|<span data-ttu-id="7d41a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d41a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d41a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d41a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="7d41a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d41a-120">Request headers</span></span>
|<span data-ttu-id="7d41a-121">标头</span><span class="sxs-lookup"><span data-stu-id="7d41a-121">Header</span></span>|<span data-ttu-id="7d41a-122">值</span><span class="sxs-lookup"><span data-stu-id="7d41a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d41a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d41a-123">Authorization</span></span>|<span data-ttu-id="7d41a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7d41a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d41a-125">接受</span><span class="sxs-lookup"><span data-stu-id="7d41a-125">Accept</span></span>|<span data-ttu-id="7d41a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d41a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d41a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d41a-127">Request body</span></span>
<span data-ttu-id="7d41a-128">在请求正文中，提供 groupPolicyPresentationLongDecimalTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d41a-128">In the request body, supply a JSON representation for the groupPolicyPresentationLongDecimalTextBox object.</span></span>

<span data-ttu-id="7d41a-129">下表显示创建 groupPolicyPresentationLongDecimalTextBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7d41a-129">The following table shows the properties that are required when you create the groupPolicyPresentationLongDecimalTextBox.</span></span>

|<span data-ttu-id="7d41a-130">属性</span><span class="sxs-lookup"><span data-stu-id="7d41a-130">Property</span></span>|<span data-ttu-id="7d41a-131">类型</span><span class="sxs-lookup"><span data-stu-id="7d41a-131">Type</span></span>|<span data-ttu-id="7d41a-132">说明</span><span class="sxs-lookup"><span data-stu-id="7d41a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d41a-133">label</span><span class="sxs-lookup"><span data-stu-id="7d41a-133">label</span></span>|<span data-ttu-id="7d41a-134">String</span><span class="sxs-lookup"><span data-stu-id="7d41a-134">String</span></span>|<span data-ttu-id="7d41a-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="7d41a-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7d41a-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="7d41a-136">The default value is empty.</span></span> <span data-ttu-id="7d41a-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7d41a-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7d41a-138">id</span><span class="sxs-lookup"><span data-stu-id="7d41a-138">id</span></span>|<span data-ttu-id="7d41a-139">String</span><span class="sxs-lookup"><span data-stu-id="7d41a-139">String</span></span>|<span data-ttu-id="7d41a-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7d41a-140">Key of the entity.</span></span> <span data-ttu-id="7d41a-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7d41a-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7d41a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d41a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7d41a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d41a-143">DateTimeOffset</span></span>|<span data-ttu-id="7d41a-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7d41a-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="7d41a-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7d41a-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7d41a-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="7d41a-146">defaultValue</span></span>|<span data-ttu-id="7d41a-147">Int64</span><span class="sxs-lookup"><span data-stu-id="7d41a-147">Int64</span></span>|<span data-ttu-id="7d41a-148">一个无符号整数，指定小数文本框的初始值。</span><span class="sxs-lookup"><span data-stu-id="7d41a-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="7d41a-149">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="7d41a-149">The default value is 1.</span></span>|
|<span data-ttu-id="7d41a-150">spin</span><span class="sxs-lookup"><span data-stu-id="7d41a-150">spin</span></span>|<span data-ttu-id="7d41a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d41a-151">Boolean</span></span>|<span data-ttu-id="7d41a-152">如果为 true，则创建旋转控件;否则，为数字输入创建一个文本框。</span><span class="sxs-lookup"><span data-stu-id="7d41a-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="7d41a-153">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="7d41a-153">The default value is true.</span></span>|
|<span data-ttu-id="7d41a-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="7d41a-154">spinStep</span></span>|<span data-ttu-id="7d41a-155">Int64</span><span class="sxs-lookup"><span data-stu-id="7d41a-155">Int64</span></span>|<span data-ttu-id="7d41a-156">一个无符号整数，指定旋转控件更改的增量。</span><span class="sxs-lookup"><span data-stu-id="7d41a-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="7d41a-157">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="7d41a-157">The default value is 1.</span></span>|
|<span data-ttu-id="7d41a-158">必需</span><span class="sxs-lookup"><span data-stu-id="7d41a-158">required</span></span>|<span data-ttu-id="7d41a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d41a-159">Boolean</span></span>|<span data-ttu-id="7d41a-160">要求在参数框中输入值。</span><span class="sxs-lookup"><span data-stu-id="7d41a-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="7d41a-161">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="7d41a-161">The default value is false.</span></span>|
|<span data-ttu-id="7d41a-162">minValue</span><span class="sxs-lookup"><span data-stu-id="7d41a-162">minValue</span></span>|<span data-ttu-id="7d41a-163">Int64</span><span class="sxs-lookup"><span data-stu-id="7d41a-163">Int64</span></span>|<span data-ttu-id="7d41a-164">指定允许的最小值的无符号长。</span><span class="sxs-lookup"><span data-stu-id="7d41a-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="7d41a-165">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="7d41a-165">The default value is 0.</span></span>|
|<span data-ttu-id="7d41a-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="7d41a-166">maxValue</span></span>|<span data-ttu-id="7d41a-167">Int64</span><span class="sxs-lookup"><span data-stu-id="7d41a-167">Int64</span></span>|<span data-ttu-id="7d41a-168">无符号长指定允许的最大值。</span><span class="sxs-lookup"><span data-stu-id="7d41a-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="7d41a-169">默认值为 9999。</span><span class="sxs-lookup"><span data-stu-id="7d41a-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="7d41a-170">响应</span><span class="sxs-lookup"><span data-stu-id="7d41a-170">Response</span></span>
<span data-ttu-id="7d41a-171">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d41a-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d41a-172">示例</span><span class="sxs-lookup"><span data-stu-id="7d41a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d41a-173">请求</span><span class="sxs-lookup"><span data-stu-id="7d41a-173">Request</span></span>
<span data-ttu-id="7d41a-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d41a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="7d41a-175">响应</span><span class="sxs-lookup"><span data-stu-id="7d41a-175">Response</span></span>
<span data-ttu-id="7d41a-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7d41a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




