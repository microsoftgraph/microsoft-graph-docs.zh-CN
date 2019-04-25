---
title: 创建 groupPolicyPresentationCheckBox
description: 创建新的 groupPolicyPresentationCheckBox 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5a74200d6cf85c02a91d50e8522fb79c58ae67f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531318"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="97cdc-103">创建 groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="97cdc-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="97cdc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97cdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97cdc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97cdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97cdc-106">创建新的[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97cdc-106">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97cdc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="97cdc-107">Prerequisites</span></span>
<span data-ttu-id="97cdc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97cdc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="97cdc-110">Permission type</span></span>|<span data-ttu-id="97cdc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="97cdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97cdc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97cdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97cdc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97cdc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97cdc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97cdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97cdc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="97cdc-115">Not supported.</span></span>|
|<span data-ttu-id="97cdc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="97cdc-116">Application</span></span>|<span data-ttu-id="97cdc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="97cdc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97cdc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97cdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="97cdc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="97cdc-119">Request headers</span></span>
|<span data-ttu-id="97cdc-120">标头</span><span class="sxs-lookup"><span data-stu-id="97cdc-120">Header</span></span>|<span data-ttu-id="97cdc-121">值</span><span class="sxs-lookup"><span data-stu-id="97cdc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97cdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97cdc-122">Authorization</span></span>|<span data-ttu-id="97cdc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="97cdc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97cdc-124">接受</span><span class="sxs-lookup"><span data-stu-id="97cdc-124">Accept</span></span>|<span data-ttu-id="97cdc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97cdc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97cdc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="97cdc-126">Request body</span></span>
<span data-ttu-id="97cdc-127">在请求正文中, 提供 groupPolicyPresentationCheckBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97cdc-127">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="97cdc-128">下表显示创建 groupPolicyPresentationCheckBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="97cdc-128">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="97cdc-129">属性</span><span class="sxs-lookup"><span data-stu-id="97cdc-129">Property</span></span>|<span data-ttu-id="97cdc-130">类型</span><span class="sxs-lookup"><span data-stu-id="97cdc-130">Type</span></span>|<span data-ttu-id="97cdc-131">说明</span><span class="sxs-lookup"><span data-stu-id="97cdc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97cdc-132">label</span><span class="sxs-lookup"><span data-stu-id="97cdc-132">label</span></span>|<span data-ttu-id="97cdc-133">String</span><span class="sxs-lookup"><span data-stu-id="97cdc-133">String</span></span>|<span data-ttu-id="97cdc-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="97cdc-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="97cdc-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="97cdc-135">The default value is empty.</span></span> <span data-ttu-id="97cdc-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="97cdc-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="97cdc-137">id</span><span class="sxs-lookup"><span data-stu-id="97cdc-137">id</span></span>|<span data-ttu-id="97cdc-138">String</span><span class="sxs-lookup"><span data-stu-id="97cdc-138">String</span></span>|<span data-ttu-id="97cdc-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="97cdc-139">Key of the entity.</span></span> <span data-ttu-id="97cdc-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="97cdc-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="97cdc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97cdc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="97cdc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97cdc-142">DateTimeOffset</span></span>|<span data-ttu-id="97cdc-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="97cdc-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="97cdc-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="97cdc-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="97cdc-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="97cdc-145">defaultChecked</span></span>|<span data-ttu-id="97cdc-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="97cdc-146">Boolean</span></span>|<span data-ttu-id="97cdc-147">复选框的默认值。</span><span class="sxs-lookup"><span data-stu-id="97cdc-147">Default value for the check box.</span></span> <span data-ttu-id="97cdc-148">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="97cdc-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="97cdc-149">响应</span><span class="sxs-lookup"><span data-stu-id="97cdc-149">Response</span></span>
<span data-ttu-id="97cdc-150">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97cdc-150">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97cdc-151">示例</span><span class="sxs-lookup"><span data-stu-id="97cdc-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="97cdc-152">请求</span><span class="sxs-lookup"><span data-stu-id="97cdc-152">Request</span></span>
<span data-ttu-id="97cdc-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97cdc-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97cdc-154">响应</span><span class="sxs-lookup"><span data-stu-id="97cdc-154">Response</span></span>
<span data-ttu-id="97cdc-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97cdc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





