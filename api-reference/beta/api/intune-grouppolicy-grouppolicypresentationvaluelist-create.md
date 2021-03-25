---
title: 创建 groupPolicyPresentationValueList
description: 创建新的 groupPolicyPresentationValueList 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b70dc810050e9c6ebbe46a6d9af2f5ea5a9b3d31
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153235"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="94228-103">创建 groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="94228-103">Create groupPolicyPresentationValueList</span></span>

<span data-ttu-id="94228-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94228-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94228-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94228-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94228-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94228-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94228-107">创建新的 [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94228-107">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94228-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="94228-108">Prerequisites</span></span>
<span data-ttu-id="94228-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94228-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="94228-111">Permission type</span></span>|<span data-ttu-id="94228-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94228-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94228-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94228-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94228-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94228-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94228-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94228-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94228-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94228-116">Not supported.</span></span>|
|<span data-ttu-id="94228-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="94228-117">Application</span></span>|<span data-ttu-id="94228-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94228-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94228-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94228-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="94228-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="94228-120">Request headers</span></span>
|<span data-ttu-id="94228-121">标头</span><span class="sxs-lookup"><span data-stu-id="94228-121">Header</span></span>|<span data-ttu-id="94228-122">值</span><span class="sxs-lookup"><span data-stu-id="94228-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94228-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94228-123">Authorization</span></span>|<span data-ttu-id="94228-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94228-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94228-125">接受</span><span class="sxs-lookup"><span data-stu-id="94228-125">Accept</span></span>|<span data-ttu-id="94228-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94228-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94228-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94228-127">Request body</span></span>
<span data-ttu-id="94228-128">在请求正文中，提供 groupPolicyPresentationValueList 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94228-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="94228-129">下表显示创建 groupPolicyPresentationValueList 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="94228-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="94228-130">属性</span><span class="sxs-lookup"><span data-stu-id="94228-130">Property</span></span>|<span data-ttu-id="94228-131">类型</span><span class="sxs-lookup"><span data-stu-id="94228-131">Type</span></span>|<span data-ttu-id="94228-132">说明</span><span class="sxs-lookup"><span data-stu-id="94228-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94228-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94228-133">lastModifiedDateTime</span></span>|<span data-ttu-id="94228-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94228-134">DateTimeOffset</span></span>|<span data-ttu-id="94228-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="94228-135">The date and time the object was last modified.</span></span> <span data-ttu-id="94228-136">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="94228-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="94228-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94228-137">createdDateTime</span></span>|<span data-ttu-id="94228-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94228-138">DateTimeOffset</span></span>|<span data-ttu-id="94228-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="94228-139">The date and time the object was created.</span></span> <span data-ttu-id="94228-140">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="94228-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="94228-141">id</span><span class="sxs-lookup"><span data-stu-id="94228-141">id</span></span>|<span data-ttu-id="94228-142">String</span><span class="sxs-lookup"><span data-stu-id="94228-142">String</span></span>|<span data-ttu-id="94228-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="94228-143">Key of the entity.</span></span> <span data-ttu-id="94228-144">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="94228-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="94228-145">值</span><span class="sxs-lookup"><span data-stu-id="94228-145">values</span></span>|<span data-ttu-id="94228-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94228-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="94228-147">关联的演示文稿的对列表。</span><span class="sxs-lookup"><span data-stu-id="94228-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="94228-148">响应</span><span class="sxs-lookup"><span data-stu-id="94228-148">Response</span></span>
<span data-ttu-id="94228-149">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94228-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94228-150">示例</span><span class="sxs-lookup"><span data-stu-id="94228-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="94228-151">请求</span><span class="sxs-lookup"><span data-stu-id="94228-151">Request</span></span>
<span data-ttu-id="94228-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94228-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="94228-153">响应</span><span class="sxs-lookup"><span data-stu-id="94228-153">Response</span></span>
<span data-ttu-id="94228-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94228-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




