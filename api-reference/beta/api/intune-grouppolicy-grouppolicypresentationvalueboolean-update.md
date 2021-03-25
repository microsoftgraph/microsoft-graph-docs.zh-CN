---
title: 更新 groupPolicyPresentationValueBoolean
description: 更新 groupPolicyPresentationValueBoolean 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e4857af7b7891e62b772eb1bee786693a8bde74
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157227"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="2bb16-103">更新 groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="2bb16-103">Update groupPolicyPresentationValueBoolean</span></span>

<span data-ttu-id="2bb16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bb16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bb16-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2bb16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bb16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bb16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bb16-107">更新 [groupPolicyPresentationValueBoolean 对象](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2bb16-107">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bb16-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2bb16-108">Prerequisites</span></span>
<span data-ttu-id="2bb16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bb16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bb16-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bb16-111">Permission type</span></span>|<span data-ttu-id="2bb16-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bb16-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bb16-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bb16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2bb16-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bb16-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bb16-116">Not supported.</span></span>|
|<span data-ttu-id="2bb16-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bb16-117">Application</span></span>|<span data-ttu-id="2bb16-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb16-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bb16-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bb16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="2bb16-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bb16-120">Request headers</span></span>
|<span data-ttu-id="2bb16-121">标头</span><span class="sxs-lookup"><span data-stu-id="2bb16-121">Header</span></span>|<span data-ttu-id="2bb16-122">值</span><span class="sxs-lookup"><span data-stu-id="2bb16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bb16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bb16-123">Authorization</span></span>|<span data-ttu-id="2bb16-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2bb16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bb16-125">接受</span><span class="sxs-lookup"><span data-stu-id="2bb16-125">Accept</span></span>|<span data-ttu-id="2bb16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bb16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bb16-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bb16-127">Request body</span></span>
<span data-ttu-id="2bb16-128">在请求正文中，提供 [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bb16-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="2bb16-129">下表显示创建 [groupPolicyPresentationValueBoolean 时所需的属性](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)。</span><span class="sxs-lookup"><span data-stu-id="2bb16-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="2bb16-130">属性</span><span class="sxs-lookup"><span data-stu-id="2bb16-130">Property</span></span>|<span data-ttu-id="2bb16-131">类型</span><span class="sxs-lookup"><span data-stu-id="2bb16-131">Type</span></span>|<span data-ttu-id="2bb16-132">说明</span><span class="sxs-lookup"><span data-stu-id="2bb16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bb16-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb16-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2bb16-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb16-134">DateTimeOffset</span></span>|<span data-ttu-id="2bb16-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2bb16-135">The date and time the object was last modified.</span></span> <span data-ttu-id="2bb16-136">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2bb16-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2bb16-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb16-137">createdDateTime</span></span>|<span data-ttu-id="2bb16-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb16-138">DateTimeOffset</span></span>|<span data-ttu-id="2bb16-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2bb16-139">The date and time the object was created.</span></span> <span data-ttu-id="2bb16-140">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2bb16-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2bb16-141">id</span><span class="sxs-lookup"><span data-stu-id="2bb16-141">id</span></span>|<span data-ttu-id="2bb16-142">String</span><span class="sxs-lookup"><span data-stu-id="2bb16-142">String</span></span>|<span data-ttu-id="2bb16-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2bb16-143">Key of the entity.</span></span> <span data-ttu-id="2bb16-144">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2bb16-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2bb16-145">value</span><span class="sxs-lookup"><span data-stu-id="2bb16-145">value</span></span>|<span data-ttu-id="2bb16-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb16-146">Boolean</span></span>|<span data-ttu-id="2bb16-147">关联的演示文稿的布尔值。</span><span class="sxs-lookup"><span data-stu-id="2bb16-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="2bb16-148">响应</span><span class="sxs-lookup"><span data-stu-id="2bb16-148">Response</span></span>
<span data-ttu-id="2bb16-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2bb16-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bb16-150">示例</span><span class="sxs-lookup"><span data-stu-id="2bb16-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bb16-151">请求</span><span class="sxs-lookup"><span data-stu-id="2bb16-151">Request</span></span>
<span data-ttu-id="2bb16-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bb16-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="2bb16-153">响应</span><span class="sxs-lookup"><span data-stu-id="2bb16-153">Response</span></span>
<span data-ttu-id="2bb16-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2bb16-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "be61344f-344f-be61-4f34-61be4f3461be",
  "value": true
}
```




