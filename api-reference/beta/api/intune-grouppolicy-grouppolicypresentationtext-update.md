---
title: 更新 groupPolicyPresentationText
description: 更新 groupPolicyPresentationText 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 750a98c0c0dbeb90e6e8a7987d8988bb1aebe5d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429556"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="d501a-103">更新 groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="d501a-103">Update groupPolicyPresentationText</span></span>

> <span data-ttu-id="d501a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d501a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d501a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d501a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d501a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d501a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d501a-107">更新[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d501a-107">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d501a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d501a-108">Prerequisites</span></span>
<span data-ttu-id="d501a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d501a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d501a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d501a-111">Permission type</span></span>|<span data-ttu-id="d501a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d501a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d501a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d501a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d501a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d501a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d501a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d501a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d501a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d501a-116">Not supported.</span></span>|
|<span data-ttu-id="d501a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d501a-117">Application</span></span>|<span data-ttu-id="d501a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d501a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d501a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d501a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d501a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d501a-120">Request headers</span></span>
|<span data-ttu-id="d501a-121">标头</span><span class="sxs-lookup"><span data-stu-id="d501a-121">Header</span></span>|<span data-ttu-id="d501a-122">值</span><span class="sxs-lookup"><span data-stu-id="d501a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d501a-123">授权</span><span class="sxs-lookup"><span data-stu-id="d501a-123">Authorization</span></span>|<span data-ttu-id="d501a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d501a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d501a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d501a-125">Accept</span></span>|<span data-ttu-id="d501a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d501a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d501a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d501a-127">Request body</span></span>
<span data-ttu-id="d501a-128">在请求正文中，提供[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d501a-128">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="d501a-129">下表显示时创建[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d501a-129">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="d501a-130">属性</span><span class="sxs-lookup"><span data-stu-id="d501a-130">Property</span></span>|<span data-ttu-id="d501a-131">类型</span><span class="sxs-lookup"><span data-stu-id="d501a-131">Type</span></span>|<span data-ttu-id="d501a-132">说明</span><span class="sxs-lookup"><span data-stu-id="d501a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d501a-133">标签</span><span class="sxs-lookup"><span data-stu-id="d501a-133">label</span></span>|<span data-ttu-id="d501a-134">String</span><span class="sxs-lookup"><span data-stu-id="d501a-134">String</span></span>|<span data-ttu-id="d501a-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="d501a-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d501a-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="d501a-136">The default value is empty.</span></span> <span data-ttu-id="d501a-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d501a-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d501a-138">id</span><span class="sxs-lookup"><span data-stu-id="d501a-138">id</span></span>|<span data-ttu-id="d501a-139">String</span><span class="sxs-lookup"><span data-stu-id="d501a-139">String</span></span>|<span data-ttu-id="d501a-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d501a-140">Key of the entity.</span></span> <span data-ttu-id="d501a-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d501a-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d501a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d501a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d501a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d501a-143">DateTimeOffset</span></span>|<span data-ttu-id="d501a-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="d501a-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="d501a-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d501a-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d501a-146">响应</span><span class="sxs-lookup"><span data-stu-id="d501a-146">Response</span></span>
<span data-ttu-id="d501a-147">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d501a-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d501a-148">示例</span><span class="sxs-lookup"><span data-stu-id="d501a-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d501a-149">请求</span><span class="sxs-lookup"><span data-stu-id="d501a-149">Request</span></span>
<span data-ttu-id="d501a-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d501a-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="d501a-151">响应</span><span class="sxs-lookup"><span data-stu-id="d501a-151">Response</span></span>
<span data-ttu-id="d501a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d501a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




