---
title: 创建 groupPolicyPresentationValueDecimal
description: 创建新的 groupPolicyPresentationValueDecimal 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 584329d8e31d2d6b71c4fe0ac3bda004588d47ae
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942680"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="3caa8-103">创建 groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="3caa8-103">Create groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="3caa8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3caa8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3caa8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3caa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3caa8-106">创建新的[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3caa8-106">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3caa8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3caa8-107">Prerequisites</span></span>
<span data-ttu-id="3caa8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3caa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3caa8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3caa8-110">Permission type</span></span>|<span data-ttu-id="3caa8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3caa8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3caa8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3caa8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3caa8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3caa8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3caa8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3caa8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3caa8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3caa8-115">Not supported.</span></span>|
|<span data-ttu-id="3caa8-116">Application</span><span class="sxs-lookup"><span data-stu-id="3caa8-116">Application</span></span>|<span data-ttu-id="3caa8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3caa8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3caa8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3caa8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="3caa8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3caa8-119">Request headers</span></span>
|<span data-ttu-id="3caa8-120">标头</span><span class="sxs-lookup"><span data-stu-id="3caa8-120">Header</span></span>|<span data-ttu-id="3caa8-121">值</span><span class="sxs-lookup"><span data-stu-id="3caa8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3caa8-122">授权</span><span class="sxs-lookup"><span data-stu-id="3caa8-122">Authorization</span></span>|<span data-ttu-id="3caa8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3caa8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3caa8-124">接受</span><span class="sxs-lookup"><span data-stu-id="3caa8-124">Accept</span></span>|<span data-ttu-id="3caa8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3caa8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3caa8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3caa8-126">Request body</span></span>
<span data-ttu-id="3caa8-127">在请求正文中，提供 groupPolicyPresentationValueDecimal 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3caa8-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="3caa8-128">下表显示创建 groupPolicyPresentationValueDecimal 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3caa8-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="3caa8-129">属性</span><span class="sxs-lookup"><span data-stu-id="3caa8-129">Property</span></span>|<span data-ttu-id="3caa8-130">类型</span><span class="sxs-lookup"><span data-stu-id="3caa8-130">Type</span></span>|<span data-ttu-id="3caa8-131">说明</span><span class="sxs-lookup"><span data-stu-id="3caa8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3caa8-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3caa8-132">lastModifiedDateTime</span></span>|<span data-ttu-id="3caa8-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caa8-133">DateTimeOffset</span></span>|<span data-ttu-id="3caa8-134">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3caa8-134">The date and time the object was last modified.</span></span> <span data-ttu-id="3caa8-135">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3caa8-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3caa8-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3caa8-136">createdDateTime</span></span>|<span data-ttu-id="3caa8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3caa8-137">DateTimeOffset</span></span>|<span data-ttu-id="3caa8-138">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3caa8-138">The date and time the object was created.</span></span> <span data-ttu-id="3caa8-139">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3caa8-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3caa8-140">id</span><span class="sxs-lookup"><span data-stu-id="3caa8-140">id</span></span>|<span data-ttu-id="3caa8-141">字符串</span><span class="sxs-lookup"><span data-stu-id="3caa8-141">String</span></span>|<span data-ttu-id="3caa8-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3caa8-142">Key of the entity.</span></span> <span data-ttu-id="3caa8-143">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3caa8-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3caa8-144">值</span><span class="sxs-lookup"><span data-stu-id="3caa8-144">value</span></span>|<span data-ttu-id="3caa8-145">Int64</span><span class="sxs-lookup"><span data-stu-id="3caa8-145">Int64</span></span>|<span data-ttu-id="3caa8-146">关联的演示文稿的无符号整数值。</span><span class="sxs-lookup"><span data-stu-id="3caa8-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="3caa8-147">响应</span><span class="sxs-lookup"><span data-stu-id="3caa8-147">Response</span></span>
<span data-ttu-id="3caa8-148">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3caa8-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3caa8-149">示例</span><span class="sxs-lookup"><span data-stu-id="3caa8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="3caa8-150">请求</span><span class="sxs-lookup"><span data-stu-id="3caa8-150">Request</span></span>
<span data-ttu-id="3caa8-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3caa8-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="3caa8-152">响应</span><span class="sxs-lookup"><span data-stu-id="3caa8-152">Response</span></span>
<span data-ttu-id="3caa8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3caa8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```





