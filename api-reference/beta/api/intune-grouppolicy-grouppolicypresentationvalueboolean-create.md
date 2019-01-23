---
title: 创建 groupPolicyPresentationValueBoolean
description: 创建新的 groupPolicyPresentationValueBoolean 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcf9a25b882bc9b952ed2b052e7b096ac45223dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429281"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="54839-103">创建 groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="54839-103">Create groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="54839-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="54839-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54839-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54839-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54839-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54839-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54839-107">创建新的[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象。</span><span class="sxs-lookup"><span data-stu-id="54839-107">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54839-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="54839-108">Prerequisites</span></span>
<span data-ttu-id="54839-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="54839-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54839-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="54839-111">Permission type</span></span>|<span data-ttu-id="54839-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="54839-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54839-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54839-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54839-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54839-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54839-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54839-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54839-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="54839-116">Not supported.</span></span>|
|<span data-ttu-id="54839-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="54839-117">Application</span></span>|<span data-ttu-id="54839-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="54839-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54839-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54839-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="54839-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="54839-120">Request headers</span></span>
|<span data-ttu-id="54839-121">标头</span><span class="sxs-lookup"><span data-stu-id="54839-121">Header</span></span>|<span data-ttu-id="54839-122">值</span><span class="sxs-lookup"><span data-stu-id="54839-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54839-123">授权</span><span class="sxs-lookup"><span data-stu-id="54839-123">Authorization</span></span>|<span data-ttu-id="54839-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54839-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54839-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54839-125">Accept</span></span>|<span data-ttu-id="54839-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54839-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54839-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="54839-127">Request body</span></span>
<span data-ttu-id="54839-128">在请求正文中，提供 groupPolicyPresentationValueBoolean 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54839-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="54839-129">下表显示时创建 groupPolicyPresentationValueBoolean 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="54839-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="54839-130">属性</span><span class="sxs-lookup"><span data-stu-id="54839-130">Property</span></span>|<span data-ttu-id="54839-131">类型</span><span class="sxs-lookup"><span data-stu-id="54839-131">Type</span></span>|<span data-ttu-id="54839-132">说明</span><span class="sxs-lookup"><span data-stu-id="54839-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54839-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54839-133">lastModifiedDateTime</span></span>|<span data-ttu-id="54839-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54839-134">DateTimeOffset</span></span>|<span data-ttu-id="54839-135">日期和时间上次修改对象。</span><span class="sxs-lookup"><span data-stu-id="54839-135">The date and time the object was last modified.</span></span> <span data-ttu-id="54839-136">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="54839-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="54839-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54839-137">createdDateTime</span></span>|<span data-ttu-id="54839-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54839-138">DateTimeOffset</span></span>|<span data-ttu-id="54839-139">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="54839-139">The date and time the object was created.</span></span> <span data-ttu-id="54839-140">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="54839-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="54839-141">id</span><span class="sxs-lookup"><span data-stu-id="54839-141">id</span></span>|<span data-ttu-id="54839-142">String</span><span class="sxs-lookup"><span data-stu-id="54839-142">String</span></span>|<span data-ttu-id="54839-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="54839-143">Key of the entity.</span></span> <span data-ttu-id="54839-144">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="54839-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="54839-145">value</span><span class="sxs-lookup"><span data-stu-id="54839-145">value</span></span>|<span data-ttu-id="54839-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="54839-146">Boolean</span></span>|<span data-ttu-id="54839-147">关联的演示文稿一个布尔值。</span><span class="sxs-lookup"><span data-stu-id="54839-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="54839-148">响应</span><span class="sxs-lookup"><span data-stu-id="54839-148">Response</span></span>
<span data-ttu-id="54839-149">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象。</span><span class="sxs-lookup"><span data-stu-id="54839-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54839-150">示例</span><span class="sxs-lookup"><span data-stu-id="54839-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="54839-151">请求</span><span class="sxs-lookup"><span data-stu-id="54839-151">Request</span></span>
<span data-ttu-id="54839-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54839-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="54839-153">响应</span><span class="sxs-lookup"><span data-stu-id="54839-153">Response</span></span>
<span data-ttu-id="54839-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54839-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




