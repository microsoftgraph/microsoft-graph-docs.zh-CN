---
title: 更新 groupPolicyPresentationText
description: 更新 groupPolicyPresentationText 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edab3145c9618c0c298cd1502c6aed5965394713
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149434"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="c634c-103">更新 groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="c634c-103">Update groupPolicyPresentationText</span></span>

<span data-ttu-id="c634c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c634c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c634c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c634c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c634c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c634c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c634c-107">更新 [groupPolicyPresentationText 对象](../resources/intune-grouppolicy-grouppolicypresentationtext.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c634c-107">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c634c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c634c-108">Prerequisites</span></span>
<span data-ttu-id="c634c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c634c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c634c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c634c-111">Permission type</span></span>|<span data-ttu-id="c634c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c634c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c634c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c634c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c634c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c634c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c634c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c634c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c634c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c634c-116">Not supported.</span></span>|
|<span data-ttu-id="c634c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c634c-117">Application</span></span>|<span data-ttu-id="c634c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c634c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c634c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c634c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="c634c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c634c-120">Request headers</span></span>
|<span data-ttu-id="c634c-121">标头</span><span class="sxs-lookup"><span data-stu-id="c634c-121">Header</span></span>|<span data-ttu-id="c634c-122">值</span><span class="sxs-lookup"><span data-stu-id="c634c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c634c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c634c-123">Authorization</span></span>|<span data-ttu-id="c634c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c634c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c634c-125">接受</span><span class="sxs-lookup"><span data-stu-id="c634c-125">Accept</span></span>|<span data-ttu-id="c634c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c634c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c634c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c634c-127">Request body</span></span>
<span data-ttu-id="c634c-128">在请求正文中，提供 [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c634c-128">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="c634c-129">下表显示创建 [groupPolicyPresentationText 时所需的属性](../resources/intune-grouppolicy-grouppolicypresentationtext.md)。</span><span class="sxs-lookup"><span data-stu-id="c634c-129">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="c634c-130">属性</span><span class="sxs-lookup"><span data-stu-id="c634c-130">Property</span></span>|<span data-ttu-id="c634c-131">类型</span><span class="sxs-lookup"><span data-stu-id="c634c-131">Type</span></span>|<span data-ttu-id="c634c-132">说明</span><span class="sxs-lookup"><span data-stu-id="c634c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c634c-133">label</span><span class="sxs-lookup"><span data-stu-id="c634c-133">label</span></span>|<span data-ttu-id="c634c-134">String</span><span class="sxs-lookup"><span data-stu-id="c634c-134">String</span></span>|<span data-ttu-id="c634c-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="c634c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c634c-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="c634c-136">The default value is empty.</span></span> <span data-ttu-id="c634c-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c634c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c634c-138">id</span><span class="sxs-lookup"><span data-stu-id="c634c-138">id</span></span>|<span data-ttu-id="c634c-139">String</span><span class="sxs-lookup"><span data-stu-id="c634c-139">String</span></span>|<span data-ttu-id="c634c-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c634c-140">Key of the entity.</span></span> <span data-ttu-id="c634c-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c634c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c634c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c634c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c634c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c634c-143">DateTimeOffset</span></span>|<span data-ttu-id="c634c-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c634c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c634c-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c634c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c634c-146">响应</span><span class="sxs-lookup"><span data-stu-id="c634c-146">Response</span></span>
<span data-ttu-id="c634c-147">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c634c-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c634c-148">示例</span><span class="sxs-lookup"><span data-stu-id="c634c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c634c-149">请求</span><span class="sxs-lookup"><span data-stu-id="c634c-149">Request</span></span>
<span data-ttu-id="c634c-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c634c-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="c634c-151">响应</span><span class="sxs-lookup"><span data-stu-id="c634c-151">Response</span></span>
<span data-ttu-id="c634c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c634c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




