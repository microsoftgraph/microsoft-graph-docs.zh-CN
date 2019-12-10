---
title: 创建 groupPolicyPresentationCheckBox
description: 创建新的 groupPolicyPresentationCheckBox 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b6084772f7264e784dde858d32d7e0c47b49795
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943079"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="68a62-103">创建 groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="68a62-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="68a62-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68a62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68a62-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68a62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68a62-106">创建新的[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="68a62-106">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68a62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="68a62-107">Prerequisites</span></span>
<span data-ttu-id="68a62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68a62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68a62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="68a62-110">Permission type</span></span>|<span data-ttu-id="68a62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="68a62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68a62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68a62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68a62-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a62-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="68a62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68a62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68a62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="68a62-115">Not supported.</span></span>|
|<span data-ttu-id="68a62-116">Application</span><span class="sxs-lookup"><span data-stu-id="68a62-116">Application</span></span>|<span data-ttu-id="68a62-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a62-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68a62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68a62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="68a62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="68a62-119">Request headers</span></span>
|<span data-ttu-id="68a62-120">标头</span><span class="sxs-lookup"><span data-stu-id="68a62-120">Header</span></span>|<span data-ttu-id="68a62-121">值</span><span class="sxs-lookup"><span data-stu-id="68a62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68a62-122">授权</span><span class="sxs-lookup"><span data-stu-id="68a62-122">Authorization</span></span>|<span data-ttu-id="68a62-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="68a62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68a62-124">接受</span><span class="sxs-lookup"><span data-stu-id="68a62-124">Accept</span></span>|<span data-ttu-id="68a62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68a62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68a62-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="68a62-126">Request body</span></span>
<span data-ttu-id="68a62-127">在请求正文中，提供 groupPolicyPresentationCheckBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68a62-127">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="68a62-128">下表显示创建 groupPolicyPresentationCheckBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="68a62-128">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="68a62-129">属性</span><span class="sxs-lookup"><span data-stu-id="68a62-129">Property</span></span>|<span data-ttu-id="68a62-130">类型</span><span class="sxs-lookup"><span data-stu-id="68a62-130">Type</span></span>|<span data-ttu-id="68a62-131">说明</span><span class="sxs-lookup"><span data-stu-id="68a62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68a62-132">label</span><span class="sxs-lookup"><span data-stu-id="68a62-132">label</span></span>|<span data-ttu-id="68a62-133">字符串</span><span class="sxs-lookup"><span data-stu-id="68a62-133">String</span></span>|<span data-ttu-id="68a62-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="68a62-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="68a62-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="68a62-135">The default value is empty.</span></span> <span data-ttu-id="68a62-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="68a62-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="68a62-137">id</span><span class="sxs-lookup"><span data-stu-id="68a62-137">id</span></span>|<span data-ttu-id="68a62-138">字符串</span><span class="sxs-lookup"><span data-stu-id="68a62-138">String</span></span>|<span data-ttu-id="68a62-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="68a62-139">Key of the entity.</span></span> <span data-ttu-id="68a62-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="68a62-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="68a62-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68a62-141">lastModifiedDateTime</span></span>|<span data-ttu-id="68a62-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68a62-142">DateTimeOffset</span></span>|<span data-ttu-id="68a62-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="68a62-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="68a62-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="68a62-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="68a62-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="68a62-145">defaultChecked</span></span>|<span data-ttu-id="68a62-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="68a62-146">Boolean</span></span>|<span data-ttu-id="68a62-147">复选框的默认值。</span><span class="sxs-lookup"><span data-stu-id="68a62-147">Default value for the check box.</span></span> <span data-ttu-id="68a62-148">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="68a62-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="68a62-149">响应</span><span class="sxs-lookup"><span data-stu-id="68a62-149">Response</span></span>
<span data-ttu-id="68a62-150">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="68a62-150">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68a62-151">示例</span><span class="sxs-lookup"><span data-stu-id="68a62-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="68a62-152">请求</span><span class="sxs-lookup"><span data-stu-id="68a62-152">Request</span></span>
<span data-ttu-id="68a62-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68a62-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="68a62-154">响应</span><span class="sxs-lookup"><span data-stu-id="68a62-154">Response</span></span>
<span data-ttu-id="68a62-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68a62-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```





