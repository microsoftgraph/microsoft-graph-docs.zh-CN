---
title: 创建 groupPolicyPresentationCheckBox
description: 创建新的 groupPolicyPresentationCheckBox 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14f30192a8f73842f819d20cd2a2b2fb048e117f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464972"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="c9857-103">创建 groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="c9857-103">Create groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="c9857-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c9857-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9857-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9857-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9857-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9857-107">创建新的[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9857-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9857-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9857-108">Prerequisites</span></span>
<span data-ttu-id="c9857-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9857-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9857-111">Permission type</span></span>|<span data-ttu-id="c9857-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9857-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9857-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9857-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9857-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9857-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c9857-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9857-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9857-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9857-116">Not supported.</span></span>|
|<span data-ttu-id="c9857-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9857-117">Application</span></span>|<span data-ttu-id="c9857-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9857-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9857-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9857-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="c9857-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9857-120">Request headers</span></span>
|<span data-ttu-id="c9857-121">标头</span><span class="sxs-lookup"><span data-stu-id="c9857-121">Header</span></span>|<span data-ttu-id="c9857-122">值</span><span class="sxs-lookup"><span data-stu-id="c9857-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9857-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9857-123">Authorization</span></span>|<span data-ttu-id="c9857-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9857-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9857-125">接受</span><span class="sxs-lookup"><span data-stu-id="c9857-125">Accept</span></span>|<span data-ttu-id="c9857-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9857-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9857-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9857-127">Request body</span></span>
<span data-ttu-id="c9857-128">在请求正文中，提供 groupPolicyPresentationCheckBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9857-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="c9857-129">下表显示创建 groupPolicyPresentationCheckBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9857-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="c9857-130">属性</span><span class="sxs-lookup"><span data-stu-id="c9857-130">Property</span></span>|<span data-ttu-id="c9857-131">类型</span><span class="sxs-lookup"><span data-stu-id="c9857-131">Type</span></span>|<span data-ttu-id="c9857-132">说明</span><span class="sxs-lookup"><span data-stu-id="c9857-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9857-133">label</span><span class="sxs-lookup"><span data-stu-id="c9857-133">label</span></span>|<span data-ttu-id="c9857-134">String</span><span class="sxs-lookup"><span data-stu-id="c9857-134">String</span></span>|<span data-ttu-id="c9857-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="c9857-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c9857-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="c9857-136">The default value is empty.</span></span> <span data-ttu-id="c9857-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c9857-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c9857-138">id</span><span class="sxs-lookup"><span data-stu-id="c9857-138">id</span></span>|<span data-ttu-id="c9857-139">String</span><span class="sxs-lookup"><span data-stu-id="c9857-139">String</span></span>|<span data-ttu-id="c9857-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9857-140">Key of the entity.</span></span> <span data-ttu-id="c9857-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c9857-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c9857-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9857-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c9857-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9857-143">DateTimeOffset</span></span>|<span data-ttu-id="c9857-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c9857-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c9857-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c9857-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c9857-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="c9857-146">defaultChecked</span></span>|<span data-ttu-id="c9857-147">布尔</span><span class="sxs-lookup"><span data-stu-id="c9857-147">Boolean</span></span>|<span data-ttu-id="c9857-148">复选框的默认值。</span><span class="sxs-lookup"><span data-stu-id="c9857-148">Default value for the check box.</span></span> <span data-ttu-id="c9857-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="c9857-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="c9857-150">响应</span><span class="sxs-lookup"><span data-stu-id="c9857-150">Response</span></span>
<span data-ttu-id="c9857-151">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9857-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9857-152">示例</span><span class="sxs-lookup"><span data-stu-id="c9857-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9857-153">请求</span><span class="sxs-lookup"><span data-stu-id="c9857-153">Request</span></span>
<span data-ttu-id="c9857-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9857-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9857-155">响应</span><span class="sxs-lookup"><span data-stu-id="c9857-155">Response</span></span>
<span data-ttu-id="c9857-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9857-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





