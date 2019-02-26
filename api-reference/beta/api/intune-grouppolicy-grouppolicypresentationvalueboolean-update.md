---
title: 更新 groupPolicyPresentationValueBoolean
description: 更新 groupPolicyPresentationValueBoolean 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 656e7f358023a7e5294fe1ab84e58492848806b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152673"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="73299-103">更新 groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="73299-103">Update groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="73299-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73299-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73299-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73299-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73299-106">更新[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73299-106">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73299-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="73299-107">Prerequisites</span></span>
<span data-ttu-id="73299-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="73299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73299-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="73299-110">Permission type</span></span>|<span data-ttu-id="73299-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73299-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73299-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73299-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73299-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73299-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="73299-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73299-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73299-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="73299-115">Not supported.</span></span>|
|<span data-ttu-id="73299-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="73299-116">Application</span></span>|<span data-ttu-id="73299-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="73299-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73299-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73299-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="73299-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73299-119">Request headers</span></span>
|<span data-ttu-id="73299-120">标头</span><span class="sxs-lookup"><span data-stu-id="73299-120">Header</span></span>|<span data-ttu-id="73299-121">值</span><span class="sxs-lookup"><span data-stu-id="73299-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73299-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73299-122">Authorization</span></span>|<span data-ttu-id="73299-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73299-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73299-124">Accept</span><span class="sxs-lookup"><span data-stu-id="73299-124">Accept</span></span>|<span data-ttu-id="73299-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73299-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73299-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73299-126">Request body</span></span>
<span data-ttu-id="73299-127">在请求正文中, 提供[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73299-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="73299-128">下表显示创建[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73299-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="73299-129">属性</span><span class="sxs-lookup"><span data-stu-id="73299-129">Property</span></span>|<span data-ttu-id="73299-130">类型</span><span class="sxs-lookup"><span data-stu-id="73299-130">Type</span></span>|<span data-ttu-id="73299-131">说明</span><span class="sxs-lookup"><span data-stu-id="73299-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73299-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73299-132">lastModifiedDateTime</span></span>|<span data-ttu-id="73299-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73299-133">DateTimeOffset</span></span>|<span data-ttu-id="73299-134">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73299-134">The date and time the object was last modified.</span></span> <span data-ttu-id="73299-135">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="73299-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="73299-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73299-136">createdDateTime</span></span>|<span data-ttu-id="73299-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73299-137">DateTimeOffset</span></span>|<span data-ttu-id="73299-138">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73299-138">The date and time the object was created.</span></span> <span data-ttu-id="73299-139">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="73299-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="73299-140">id</span><span class="sxs-lookup"><span data-stu-id="73299-140">id</span></span>|<span data-ttu-id="73299-141">String</span><span class="sxs-lookup"><span data-stu-id="73299-141">String</span></span>|<span data-ttu-id="73299-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73299-142">Key of the entity.</span></span> <span data-ttu-id="73299-143">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="73299-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="73299-144">value</span><span class="sxs-lookup"><span data-stu-id="73299-144">value</span></span>|<span data-ttu-id="73299-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="73299-145">Boolean</span></span>|<span data-ttu-id="73299-146">一个布尔值, 用于关联的演示文稿。</span><span class="sxs-lookup"><span data-stu-id="73299-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="73299-147">响应</span><span class="sxs-lookup"><span data-stu-id="73299-147">Response</span></span>
<span data-ttu-id="73299-148">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象。</span><span class="sxs-lookup"><span data-stu-id="73299-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73299-149">示例</span><span class="sxs-lookup"><span data-stu-id="73299-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="73299-150">请求</span><span class="sxs-lookup"><span data-stu-id="73299-150">Request</span></span>
<span data-ttu-id="73299-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73299-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="73299-152">响应</span><span class="sxs-lookup"><span data-stu-id="73299-152">Response</span></span>
<span data-ttu-id="73299-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73299-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




