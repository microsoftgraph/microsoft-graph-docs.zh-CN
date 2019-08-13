---
title: 更新 groupPolicyPresentationValueMultiText
description: 更新 groupPolicyPresentationValueMultiText 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83211e03491a5f93e7a10632e260dad319fd0030
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357437"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="30367-103">更新 groupPolicyPresentationValueMultiText</span><span class="sxs-lookup"><span data-stu-id="30367-103">Update groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="30367-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="30367-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30367-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="30367-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30367-106">更新[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30367-106">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30367-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="30367-107">Prerequisites</span></span>
<span data-ttu-id="30367-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30367-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30367-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="30367-110">Permission type</span></span>|<span data-ttu-id="30367-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="30367-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30367-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30367-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30367-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30367-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="30367-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30367-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30367-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="30367-115">Not supported.</span></span>|
|<span data-ttu-id="30367-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="30367-116">Application</span></span>|<span data-ttu-id="30367-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30367-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30367-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30367-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="30367-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="30367-119">Request headers</span></span>
|<span data-ttu-id="30367-120">标头</span><span class="sxs-lookup"><span data-stu-id="30367-120">Header</span></span>|<span data-ttu-id="30367-121">值</span><span class="sxs-lookup"><span data-stu-id="30367-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30367-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30367-122">Authorization</span></span>|<span data-ttu-id="30367-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="30367-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30367-124">接受</span><span class="sxs-lookup"><span data-stu-id="30367-124">Accept</span></span>|<span data-ttu-id="30367-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30367-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30367-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="30367-126">Request body</span></span>
<span data-ttu-id="30367-127">在请求正文中, 提供[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30367-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="30367-128">下表显示创建[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="30367-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="30367-129">属性</span><span class="sxs-lookup"><span data-stu-id="30367-129">Property</span></span>|<span data-ttu-id="30367-130">类型</span><span class="sxs-lookup"><span data-stu-id="30367-130">Type</span></span>|<span data-ttu-id="30367-131">说明</span><span class="sxs-lookup"><span data-stu-id="30367-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30367-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30367-132">lastModifiedDateTime</span></span>|<span data-ttu-id="30367-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30367-133">DateTimeOffset</span></span>|<span data-ttu-id="30367-134">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="30367-134">The date and time the object was last modified.</span></span> <span data-ttu-id="30367-135">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="30367-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="30367-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30367-136">createdDateTime</span></span>|<span data-ttu-id="30367-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30367-137">DateTimeOffset</span></span>|<span data-ttu-id="30367-138">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="30367-138">The date and time the object was created.</span></span> <span data-ttu-id="30367-139">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="30367-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="30367-140">id</span><span class="sxs-lookup"><span data-stu-id="30367-140">id</span></span>|<span data-ttu-id="30367-141">String</span><span class="sxs-lookup"><span data-stu-id="30367-141">String</span></span>|<span data-ttu-id="30367-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="30367-142">Key of the entity.</span></span> <span data-ttu-id="30367-143">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="30367-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="30367-144">values</span><span class="sxs-lookup"><span data-stu-id="30367-144">values</span></span>|<span data-ttu-id="30367-145">String collection</span><span class="sxs-lookup"><span data-stu-id="30367-145">String collection</span></span>|<span data-ttu-id="30367-146">关联演示文稿的非空字符串的集合。</span><span class="sxs-lookup"><span data-stu-id="30367-146">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="30367-147">响应</span><span class="sxs-lookup"><span data-stu-id="30367-147">Response</span></span>
<span data-ttu-id="30367-148">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="30367-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30367-149">示例</span><span class="sxs-lookup"><span data-stu-id="30367-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="30367-150">请求</span><span class="sxs-lookup"><span data-stu-id="30367-150">Request</span></span>
<span data-ttu-id="30367-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30367-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="30367-152">响应</span><span class="sxs-lookup"><span data-stu-id="30367-152">Response</span></span>
<span data-ttu-id="30367-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30367-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```






