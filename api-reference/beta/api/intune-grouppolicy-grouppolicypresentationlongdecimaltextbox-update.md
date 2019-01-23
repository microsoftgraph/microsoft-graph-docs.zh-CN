---
title: 更新 groupPolicyPresentationLongDecimalTextBox
description: 更新 groupPolicyPresentationLongDecimalTextBox 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0b206a557ebd4715aede7e8becbeae672c8bea4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428855"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="aa85f-103">更新 groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="aa85f-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="aa85f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="aa85f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa85f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa85f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa85f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa85f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa85f-107">更新[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa85f-107">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa85f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa85f-108">Prerequisites</span></span>
<span data-ttu-id="aa85f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aa85f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aa85f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa85f-111">Permission type</span></span>|<span data-ttu-id="aa85f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa85f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa85f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa85f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa85f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa85f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa85f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa85f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa85f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa85f-116">Not supported.</span></span>|
|<span data-ttu-id="aa85f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa85f-117">Application</span></span>|<span data-ttu-id="aa85f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa85f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa85f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa85f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="aa85f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa85f-120">Request headers</span></span>
|<span data-ttu-id="aa85f-121">标头</span><span class="sxs-lookup"><span data-stu-id="aa85f-121">Header</span></span>|<span data-ttu-id="aa85f-122">值</span><span class="sxs-lookup"><span data-stu-id="aa85f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa85f-123">授权</span><span class="sxs-lookup"><span data-stu-id="aa85f-123">Authorization</span></span>|<span data-ttu-id="aa85f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa85f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa85f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa85f-125">Accept</span></span>|<span data-ttu-id="aa85f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa85f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa85f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa85f-127">Request body</span></span>
<span data-ttu-id="aa85f-128">在请求正文中，提供[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa85f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="aa85f-129">下表显示时创建[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aa85f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="aa85f-130">属性</span><span class="sxs-lookup"><span data-stu-id="aa85f-130">Property</span></span>|<span data-ttu-id="aa85f-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa85f-131">Type</span></span>|<span data-ttu-id="aa85f-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa85f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa85f-133">标签</span><span class="sxs-lookup"><span data-stu-id="aa85f-133">label</span></span>|<span data-ttu-id="aa85f-134">String</span><span class="sxs-lookup"><span data-stu-id="aa85f-134">String</span></span>|<span data-ttu-id="aa85f-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="aa85f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="aa85f-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="aa85f-136">The default value is empty.</span></span> <span data-ttu-id="aa85f-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="aa85f-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="aa85f-138">id</span><span class="sxs-lookup"><span data-stu-id="aa85f-138">id</span></span>|<span data-ttu-id="aa85f-139">String</span><span class="sxs-lookup"><span data-stu-id="aa85f-139">String</span></span>|<span data-ttu-id="aa85f-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aa85f-140">Key of the entity.</span></span> <span data-ttu-id="aa85f-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="aa85f-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="aa85f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa85f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="aa85f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa85f-143">DateTimeOffset</span></span>|<span data-ttu-id="aa85f-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="aa85f-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="aa85f-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="aa85f-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="aa85f-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="aa85f-146">defaultValue</span></span>|<span data-ttu-id="aa85f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="aa85f-147">Int64</span></span>|<span data-ttu-id="aa85f-148">指定小数文本框的初始值无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="aa85f-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="aa85f-149">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="aa85f-149">The default value is 1.</span></span>|
|<span data-ttu-id="aa85f-150">旋转</span><span class="sxs-lookup"><span data-stu-id="aa85f-150">spin</span></span>|<span data-ttu-id="aa85f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa85f-151">Boolean</span></span>|<span data-ttu-id="aa85f-152">如果为 true，则创建调节控件;否则，创建文本框中输入数字。</span><span class="sxs-lookup"><span data-stu-id="aa85f-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="aa85f-153">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="aa85f-153">The default value is true.</span></span>|
|<span data-ttu-id="aa85f-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="aa85f-154">spinStep</span></span>|<span data-ttu-id="aa85f-155">Int64</span><span class="sxs-lookup"><span data-stu-id="aa85f-155">Int64</span></span>|<span data-ttu-id="aa85f-156">指定的增量更改数字调整控件的无符号的整数。</span><span class="sxs-lookup"><span data-stu-id="aa85f-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="aa85f-157">默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="aa85f-157">The default value is 1.</span></span>|
|<span data-ttu-id="aa85f-158">必需</span><span class="sxs-lookup"><span data-stu-id="aa85f-158">required</span></span>|<span data-ttu-id="aa85f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa85f-159">Boolean</span></span>|<span data-ttu-id="aa85f-160">在参数框中输入值的要求。</span><span class="sxs-lookup"><span data-stu-id="aa85f-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="aa85f-161">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="aa85f-161">The default value is false.</span></span>|
|<span data-ttu-id="aa85f-162">minValue</span><span class="sxs-lookup"><span data-stu-id="aa85f-162">minValue</span></span>|<span data-ttu-id="aa85f-163">Int64</span><span class="sxs-lookup"><span data-stu-id="aa85f-163">Int64</span></span>|<span data-ttu-id="aa85f-164">无符号指定允许最小值的 long。</span><span class="sxs-lookup"><span data-stu-id="aa85f-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="aa85f-165">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="aa85f-165">The default value is 0.</span></span>|
|<span data-ttu-id="aa85f-166">值</span><span class="sxs-lookup"><span data-stu-id="aa85f-166">maxValue</span></span>|<span data-ttu-id="aa85f-167">Int64</span><span class="sxs-lookup"><span data-stu-id="aa85f-167">Int64</span></span>|<span data-ttu-id="aa85f-168">无符号指定最大允许值的 long。</span><span class="sxs-lookup"><span data-stu-id="aa85f-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="aa85f-169">默认值是 9999。</span><span class="sxs-lookup"><span data-stu-id="aa85f-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="aa85f-170">响应</span><span class="sxs-lookup"><span data-stu-id="aa85f-170">Response</span></span>
<span data-ttu-id="aa85f-171">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aa85f-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa85f-172">示例</span><span class="sxs-lookup"><span data-stu-id="aa85f-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa85f-173">请求</span><span class="sxs-lookup"><span data-stu-id="aa85f-173">Request</span></span>
<span data-ttu-id="aa85f-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa85f-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa85f-175">响应</span><span class="sxs-lookup"><span data-stu-id="aa85f-175">Response</span></span>
<span data-ttu-id="aa85f-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa85f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




