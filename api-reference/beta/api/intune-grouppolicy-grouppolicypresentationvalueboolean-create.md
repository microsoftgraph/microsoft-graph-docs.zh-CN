---
title: 创建 groupPolicyPresentationValueBoolean
description: 创建新的 groupPolicyPresentationValueBoolean 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e191fb84e3c3b2e9bb9d0b15a0e12a455d3f3b9d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965870"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="1441b-103">创建 groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="1441b-103">Create groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="1441b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1441b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1441b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1441b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1441b-106">创建新的[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1441b-106">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1441b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1441b-107">Prerequisites</span></span>
<span data-ttu-id="1441b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1441b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1441b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1441b-110">Permission type</span></span>|<span data-ttu-id="1441b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1441b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1441b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1441b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1441b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1441b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1441b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1441b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1441b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1441b-115">Not supported.</span></span>|
|<span data-ttu-id="1441b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1441b-116">Application</span></span>|<span data-ttu-id="1441b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1441b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1441b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1441b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="1441b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1441b-119">Request headers</span></span>
|<span data-ttu-id="1441b-120">标头</span><span class="sxs-lookup"><span data-stu-id="1441b-120">Header</span></span>|<span data-ttu-id="1441b-121">值</span><span class="sxs-lookup"><span data-stu-id="1441b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1441b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1441b-122">Authorization</span></span>|<span data-ttu-id="1441b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1441b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1441b-124">接受</span><span class="sxs-lookup"><span data-stu-id="1441b-124">Accept</span></span>|<span data-ttu-id="1441b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1441b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1441b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1441b-126">Request body</span></span>
<span data-ttu-id="1441b-127">在请求正文中, 提供 groupPolicyPresentationValueBoolean 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1441b-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="1441b-128">下表显示创建 groupPolicyPresentationValueBoolean 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1441b-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="1441b-129">属性</span><span class="sxs-lookup"><span data-stu-id="1441b-129">Property</span></span>|<span data-ttu-id="1441b-130">类型</span><span class="sxs-lookup"><span data-stu-id="1441b-130">Type</span></span>|<span data-ttu-id="1441b-131">说明</span><span class="sxs-lookup"><span data-stu-id="1441b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1441b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1441b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="1441b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1441b-133">DateTimeOffset</span></span>|<span data-ttu-id="1441b-134">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1441b-134">The date and time the object was last modified.</span></span> <span data-ttu-id="1441b-135">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1441b-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1441b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1441b-136">createdDateTime</span></span>|<span data-ttu-id="1441b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1441b-137">DateTimeOffset</span></span>|<span data-ttu-id="1441b-138">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1441b-138">The date and time the object was created.</span></span> <span data-ttu-id="1441b-139">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1441b-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1441b-140">id</span><span class="sxs-lookup"><span data-stu-id="1441b-140">id</span></span>|<span data-ttu-id="1441b-141">String</span><span class="sxs-lookup"><span data-stu-id="1441b-141">String</span></span>|<span data-ttu-id="1441b-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1441b-142">Key of the entity.</span></span> <span data-ttu-id="1441b-143">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1441b-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1441b-144">value</span><span class="sxs-lookup"><span data-stu-id="1441b-144">value</span></span>|<span data-ttu-id="1441b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1441b-145">Boolean</span></span>|<span data-ttu-id="1441b-146">一个布尔值, 用于关联的演示文稿。</span><span class="sxs-lookup"><span data-stu-id="1441b-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="1441b-147">响应</span><span class="sxs-lookup"><span data-stu-id="1441b-147">Response</span></span>
<span data-ttu-id="1441b-148">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1441b-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1441b-149">示例</span><span class="sxs-lookup"><span data-stu-id="1441b-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="1441b-150">请求</span><span class="sxs-lookup"><span data-stu-id="1441b-150">Request</span></span>
<span data-ttu-id="1441b-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1441b-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="1441b-152">响应</span><span class="sxs-lookup"><span data-stu-id="1441b-152">Response</span></span>
<span data-ttu-id="1441b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1441b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





