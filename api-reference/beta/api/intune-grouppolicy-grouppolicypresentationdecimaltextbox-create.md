---
title: 创建 groupPolicyPresentationDecimalTextBox
description: 创建新的 groupPolicyPresentationDecimalTextBox 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1cc6e5cb8104cc4d9ff4cffcf2157fe954f991cf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429465"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="c1dfa-103">创建 groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="c1dfa-103">Create groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="c1dfa-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1dfa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1dfa-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1dfa-107">创建新的[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-107">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1dfa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1dfa-108">Prerequisites</span></span>
<span data-ttu-id="c1dfa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1dfa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1dfa-111">Permission type</span></span>|<span data-ttu-id="c1dfa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1dfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1dfa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1dfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1dfa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1dfa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1dfa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1dfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1dfa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-116">Not supported.</span></span>|
|<span data-ttu-id="c1dfa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1dfa-117">Application</span></span>|<span data-ttu-id="c1dfa-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1dfa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1dfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="c1dfa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1dfa-120">Request headers</span></span>
|<span data-ttu-id="c1dfa-121">标头</span><span class="sxs-lookup"><span data-stu-id="c1dfa-121">Header</span></span>|<span data-ttu-id="c1dfa-122">值</span><span class="sxs-lookup"><span data-stu-id="c1dfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1dfa-123">授权</span><span class="sxs-lookup"><span data-stu-id="c1dfa-123">Authorization</span></span>|<span data-ttu-id="c1dfa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1dfa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1dfa-125">Accept</span></span>|<span data-ttu-id="c1dfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1dfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1dfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1dfa-127">Request body</span></span>
<span data-ttu-id="c1dfa-128">在请求正文中，提供 groupPolicyPresentationDecimalTextBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-128">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="c1dfa-129">下表显示时创建 groupPolicyPresentationDecimalTextBox 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-129">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="c1dfa-130">属性</span><span class="sxs-lookup"><span data-stu-id="c1dfa-130">Property</span></span>|<span data-ttu-id="c1dfa-131">类型</span><span class="sxs-lookup"><span data-stu-id="c1dfa-131">Type</span></span>|<span data-ttu-id="c1dfa-132">说明</span><span class="sxs-lookup"><span data-stu-id="c1dfa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1dfa-133">标签</span><span class="sxs-lookup"><span data-stu-id="c1dfa-133">label</span></span>|<span data-ttu-id="c1dfa-134">String</span><span class="sxs-lookup"><span data-stu-id="c1dfa-134">String</span></span>|<span data-ttu-id="c1dfa-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c1dfa-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-136">The default value is empty.</span></span> <span data-ttu-id="c1dfa-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c1dfa-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c1dfa-138">id</span><span class="sxs-lookup"><span data-stu-id="c1dfa-138">id</span></span>|<span data-ttu-id="c1dfa-139">String</span><span class="sxs-lookup"><span data-stu-id="c1dfa-139">String</span></span>|<span data-ttu-id="c1dfa-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-140">Key of the entity.</span></span> <span data-ttu-id="c1dfa-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c1dfa-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c1dfa-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1dfa-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c1dfa-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1dfa-143">DateTimeOffset</span></span>|<span data-ttu-id="c1dfa-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c1dfa-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c1dfa-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c1dfa-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="c1dfa-146">defaultValue</span></span>|<span data-ttu-id="c1dfa-147">Int64</span><span class="sxs-lookup"><span data-stu-id="c1dfa-147">Int64</span></span>|<span data-ttu-id="c1dfa-148">指定小数文本框的初始值无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="c1dfa-149">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-149">The default value is 1.</span></span>|
|<span data-ttu-id="c1dfa-150">旋转</span><span class="sxs-lookup"><span data-stu-id="c1dfa-150">spin</span></span>|<span data-ttu-id="c1dfa-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1dfa-151">Boolean</span></span>|<span data-ttu-id="c1dfa-152">如果为 true，则创建调节控件;否则，创建文本框中输入数字。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="c1dfa-153">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-153">The default value is true.</span></span>|
|<span data-ttu-id="c1dfa-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="c1dfa-154">spinStep</span></span>|<span data-ttu-id="c1dfa-155">Int64</span><span class="sxs-lookup"><span data-stu-id="c1dfa-155">Int64</span></span>|<span data-ttu-id="c1dfa-156">指定的增量更改数字调整控件的无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="c1dfa-157">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-157">The default value is 1.</span></span>|
|<span data-ttu-id="c1dfa-158">必需</span><span class="sxs-lookup"><span data-stu-id="c1dfa-158">required</span></span>|<span data-ttu-id="c1dfa-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1dfa-159">Boolean</span></span>|<span data-ttu-id="c1dfa-160">在参数框中输入值的要求。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="c1dfa-161">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-161">The default value is false.</span></span>|
|<span data-ttu-id="c1dfa-162">minValue</span><span class="sxs-lookup"><span data-stu-id="c1dfa-162">minValue</span></span>|<span data-ttu-id="c1dfa-163">Int64</span><span class="sxs-lookup"><span data-stu-id="c1dfa-163">Int64</span></span>|<span data-ttu-id="c1dfa-164">指定允许的最小值无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="c1dfa-165">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-165">The default value is 0.</span></span>|
|<span data-ttu-id="c1dfa-166">值</span><span class="sxs-lookup"><span data-stu-id="c1dfa-166">maxValue</span></span>|<span data-ttu-id="c1dfa-167">Int64</span><span class="sxs-lookup"><span data-stu-id="c1dfa-167">Int64</span></span>|<span data-ttu-id="c1dfa-168">无符号的整数，指定允许的最大值。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="c1dfa-169">默认值是 9999。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="c1dfa-170">响应</span><span class="sxs-lookup"><span data-stu-id="c1dfa-170">Response</span></span>
<span data-ttu-id="c1dfa-171">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1dfa-172">示例</span><span class="sxs-lookup"><span data-stu-id="c1dfa-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1dfa-173">请求</span><span class="sxs-lookup"><span data-stu-id="c1dfa-173">Request</span></span>
<span data-ttu-id="c1dfa-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1dfa-175">响应</span><span class="sxs-lookup"><span data-stu-id="c1dfa-175">Response</span></span>
<span data-ttu-id="c1dfa-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1dfa-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




