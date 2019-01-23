---
title: 创建 groupPolicyPresentationCheckBox
description: 创建新的 groupPolicyPresentationCheckBox 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc0d5ff04aedfbbf0e9bac3967f5f502a13e5e57
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429383"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="df633-103">创建 groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="df633-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="df633-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="df633-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df633-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df633-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df633-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df633-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df633-107">创建新的[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="df633-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df633-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df633-108">Prerequisites</span></span>
<span data-ttu-id="df633-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="df633-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df633-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df633-111">Permission type</span></span>|<span data-ttu-id="df633-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df633-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df633-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df633-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df633-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df633-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df633-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df633-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df633-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df633-116">Not supported.</span></span>|
|<span data-ttu-id="df633-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df633-117">Application</span></span>|<span data-ttu-id="df633-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="df633-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df633-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df633-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="df633-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df633-120">Request headers</span></span>
|<span data-ttu-id="df633-121">标头</span><span class="sxs-lookup"><span data-stu-id="df633-121">Header</span></span>|<span data-ttu-id="df633-122">值</span><span class="sxs-lookup"><span data-stu-id="df633-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df633-123">授权</span><span class="sxs-lookup"><span data-stu-id="df633-123">Authorization</span></span>|<span data-ttu-id="df633-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df633-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df633-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df633-125">Accept</span></span>|<span data-ttu-id="df633-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df633-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df633-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df633-127">Request body</span></span>
<span data-ttu-id="df633-128">在请求正文中，提供 groupPolicyPresentationCheckBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df633-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="df633-129">下表显示时创建 groupPolicyPresentationCheckBox 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df633-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="df633-130">属性</span><span class="sxs-lookup"><span data-stu-id="df633-130">Property</span></span>|<span data-ttu-id="df633-131">类型</span><span class="sxs-lookup"><span data-stu-id="df633-131">Type</span></span>|<span data-ttu-id="df633-132">说明</span><span class="sxs-lookup"><span data-stu-id="df633-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df633-133">标签</span><span class="sxs-lookup"><span data-stu-id="df633-133">label</span></span>|<span data-ttu-id="df633-134">String</span><span class="sxs-lookup"><span data-stu-id="df633-134">String</span></span>|<span data-ttu-id="df633-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="df633-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="df633-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="df633-136">The default value is empty.</span></span> <span data-ttu-id="df633-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="df633-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="df633-138">id</span><span class="sxs-lookup"><span data-stu-id="df633-138">id</span></span>|<span data-ttu-id="df633-139">String</span><span class="sxs-lookup"><span data-stu-id="df633-139">String</span></span>|<span data-ttu-id="df633-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df633-140">Key of the entity.</span></span> <span data-ttu-id="df633-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="df633-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="df633-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df633-142">lastModifiedDateTime</span></span>|<span data-ttu-id="df633-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df633-143">DateTimeOffset</span></span>|<span data-ttu-id="df633-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="df633-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="df633-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="df633-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="df633-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="df633-146">defaultChecked</span></span>|<span data-ttu-id="df633-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="df633-147">Boolean</span></span>|<span data-ttu-id="df633-148">默认值复选框。</span><span class="sxs-lookup"><span data-stu-id="df633-148">Default value for the check box.</span></span> <span data-ttu-id="df633-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="df633-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="df633-150">响应</span><span class="sxs-lookup"><span data-stu-id="df633-150">Response</span></span>
<span data-ttu-id="df633-151">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="df633-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df633-152">示例</span><span class="sxs-lookup"><span data-stu-id="df633-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="df633-153">请求</span><span class="sxs-lookup"><span data-stu-id="df633-153">Request</span></span>
<span data-ttu-id="df633-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df633-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df633-155">响应</span><span class="sxs-lookup"><span data-stu-id="df633-155">Response</span></span>
<span data-ttu-id="df633-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df633-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




