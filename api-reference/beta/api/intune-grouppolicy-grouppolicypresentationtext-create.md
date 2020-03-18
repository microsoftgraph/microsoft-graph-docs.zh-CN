---
title: 创建 groupPolicyPresentationText
description: 创建新的 groupPolicyPresentationText 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4888891d386582ce51d633a802dbf8d4c0db681c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804112"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="dfafc-103">创建 groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="dfafc-103">Create groupPolicyPresentationText</span></span>

> <span data-ttu-id="dfafc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfafc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfafc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfafc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfafc-106">创建新的[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dfafc-106">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfafc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfafc-107">Prerequisites</span></span>
<span data-ttu-id="dfafc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfafc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfafc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfafc-110">Permission type</span></span>|<span data-ttu-id="dfafc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dfafc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfafc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfafc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfafc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfafc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dfafc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfafc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfafc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfafc-115">Not supported.</span></span>|
|<span data-ttu-id="dfafc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfafc-116">Application</span></span>|<span data-ttu-id="dfafc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfafc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfafc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfafc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="dfafc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfafc-119">Request headers</span></span>
|<span data-ttu-id="dfafc-120">标头</span><span class="sxs-lookup"><span data-stu-id="dfafc-120">Header</span></span>|<span data-ttu-id="dfafc-121">值</span><span class="sxs-lookup"><span data-stu-id="dfafc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfafc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfafc-122">Authorization</span></span>|<span data-ttu-id="dfafc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfafc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfafc-124">接受</span><span class="sxs-lookup"><span data-stu-id="dfafc-124">Accept</span></span>|<span data-ttu-id="dfafc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfafc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfafc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfafc-126">Request body</span></span>
<span data-ttu-id="dfafc-127">在请求正文中，提供 groupPolicyPresentationText 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfafc-127">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="dfafc-128">下表显示创建 groupPolicyPresentationText 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dfafc-128">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="dfafc-129">属性</span><span class="sxs-lookup"><span data-stu-id="dfafc-129">Property</span></span>|<span data-ttu-id="dfafc-130">类型</span><span class="sxs-lookup"><span data-stu-id="dfafc-130">Type</span></span>|<span data-ttu-id="dfafc-131">说明</span><span class="sxs-lookup"><span data-stu-id="dfafc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfafc-132">label</span><span class="sxs-lookup"><span data-stu-id="dfafc-132">label</span></span>|<span data-ttu-id="dfafc-133">String</span><span class="sxs-lookup"><span data-stu-id="dfafc-133">String</span></span>|<span data-ttu-id="dfafc-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="dfafc-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="dfafc-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="dfafc-135">The default value is empty.</span></span> <span data-ttu-id="dfafc-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="dfafc-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="dfafc-137">id</span><span class="sxs-lookup"><span data-stu-id="dfafc-137">id</span></span>|<span data-ttu-id="dfafc-138">String</span><span class="sxs-lookup"><span data-stu-id="dfafc-138">String</span></span>|<span data-ttu-id="dfafc-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dfafc-139">Key of the entity.</span></span> <span data-ttu-id="dfafc-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="dfafc-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="dfafc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfafc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="dfafc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfafc-142">DateTimeOffset</span></span>|<span data-ttu-id="dfafc-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dfafc-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="dfafc-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="dfafc-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="dfafc-145">响应</span><span class="sxs-lookup"><span data-stu-id="dfafc-145">Response</span></span>
<span data-ttu-id="dfafc-146">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dfafc-146">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfafc-147">示例</span><span class="sxs-lookup"><span data-stu-id="dfafc-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfafc-148">请求</span><span class="sxs-lookup"><span data-stu-id="dfafc-148">Request</span></span>
<span data-ttu-id="dfafc-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfafc-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="dfafc-150">响应</span><span class="sxs-lookup"><span data-stu-id="dfafc-150">Response</span></span>
<span data-ttu-id="dfafc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfafc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




