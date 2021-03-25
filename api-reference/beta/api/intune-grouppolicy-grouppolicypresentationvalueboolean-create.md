---
title: 创建 groupPolicyPresentationValueBoolean
description: 创建新的 groupPolicyPresentationValueBoolean 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 204ab6e117cd6a5b6f1e4084fd3673b403ba4e56
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157326"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="a2ba2-103">创建 groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="a2ba2-103">Create groupPolicyPresentationValueBoolean</span></span>

<span data-ttu-id="a2ba2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ba2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2ba2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2ba2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ba2-107">创建新的 [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-107">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2ba2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2ba2-108">Prerequisites</span></span>
<span data-ttu-id="a2ba2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2ba2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2ba2-111">Permission type</span></span>|<span data-ttu-id="a2ba2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2ba2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ba2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2ba2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2ba2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ba2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2ba2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2ba2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ba2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-116">Not supported.</span></span>|
|<span data-ttu-id="a2ba2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2ba2-117">Application</span></span>|<span data-ttu-id="a2ba2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ba2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ba2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2ba2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="a2ba2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2ba2-120">Request headers</span></span>
|<span data-ttu-id="a2ba2-121">标头</span><span class="sxs-lookup"><span data-stu-id="a2ba2-121">Header</span></span>|<span data-ttu-id="a2ba2-122">值</span><span class="sxs-lookup"><span data-stu-id="a2ba2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ba2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ba2-123">Authorization</span></span>|<span data-ttu-id="a2ba2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ba2-125">接受</span><span class="sxs-lookup"><span data-stu-id="a2ba2-125">Accept</span></span>|<span data-ttu-id="a2ba2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ba2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ba2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2ba2-127">Request body</span></span>
<span data-ttu-id="a2ba2-128">在请求正文中，提供 groupPolicyPresentationValueBoolean 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="a2ba2-129">下表显示创建 groupPolicyPresentationValueBoolean 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="a2ba2-130">属性</span><span class="sxs-lookup"><span data-stu-id="a2ba2-130">Property</span></span>|<span data-ttu-id="a2ba2-131">类型</span><span class="sxs-lookup"><span data-stu-id="a2ba2-131">Type</span></span>|<span data-ttu-id="a2ba2-132">说明</span><span class="sxs-lookup"><span data-stu-id="a2ba2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ba2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ba2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a2ba2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ba2-134">DateTimeOffset</span></span>|<span data-ttu-id="a2ba2-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-135">The date and time the object was last modified.</span></span> <span data-ttu-id="a2ba2-136">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a2ba2-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="a2ba2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ba2-137">createdDateTime</span></span>|<span data-ttu-id="a2ba2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ba2-138">DateTimeOffset</span></span>|<span data-ttu-id="a2ba2-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-139">The date and time the object was created.</span></span> <span data-ttu-id="a2ba2-140">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a2ba2-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="a2ba2-141">id</span><span class="sxs-lookup"><span data-stu-id="a2ba2-141">id</span></span>|<span data-ttu-id="a2ba2-142">String</span><span class="sxs-lookup"><span data-stu-id="a2ba2-142">String</span></span>|<span data-ttu-id="a2ba2-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-143">Key of the entity.</span></span> <span data-ttu-id="a2ba2-144">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a2ba2-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="a2ba2-145">value</span><span class="sxs-lookup"><span data-stu-id="a2ba2-145">value</span></span>|<span data-ttu-id="a2ba2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ba2-146">Boolean</span></span>|<span data-ttu-id="a2ba2-147">关联的演示文稿的布尔值。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="a2ba2-148">响应</span><span class="sxs-lookup"><span data-stu-id="a2ba2-148">Response</span></span>
<span data-ttu-id="a2ba2-149">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ba2-150">示例</span><span class="sxs-lookup"><span data-stu-id="a2ba2-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2ba2-151">请求</span><span class="sxs-lookup"><span data-stu-id="a2ba2-151">Request</span></span>
<span data-ttu-id="a2ba2-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="a2ba2-153">响应</span><span class="sxs-lookup"><span data-stu-id="a2ba2-153">Response</span></span>
<span data-ttu-id="a2ba2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2ba2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




