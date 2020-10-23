---
title: 更新 groupPolicyPresentationValueMultiText
description: 更新 groupPolicyPresentationValueMultiText 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d4e1b5e19d1980046a2603812a660fbf2c0c407
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698587"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="f6819-103">更新 groupPolicyPresentationValueMultiText</span><span class="sxs-lookup"><span data-stu-id="f6819-103">Update groupPolicyPresentationValueMultiText</span></span>

<span data-ttu-id="f6819-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6819-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6819-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6819-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6819-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6819-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6819-107">更新 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f6819-107">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6819-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f6819-108">Prerequisites</span></span>
<span data-ttu-id="f6819-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6819-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6819-111">Permission type</span></span>|<span data-ttu-id="f6819-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f6819-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6819-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6819-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6819-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6819-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6819-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6819-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6819-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6819-116">Not supported.</span></span>|
|<span data-ttu-id="f6819-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6819-117">Application</span></span>|<span data-ttu-id="f6819-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6819-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6819-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6819-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="f6819-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6819-120">Request headers</span></span>
|<span data-ttu-id="f6819-121">标头</span><span class="sxs-lookup"><span data-stu-id="f6819-121">Header</span></span>|<span data-ttu-id="f6819-122">值</span><span class="sxs-lookup"><span data-stu-id="f6819-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6819-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6819-123">Authorization</span></span>|<span data-ttu-id="f6819-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f6819-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6819-125">接受</span><span class="sxs-lookup"><span data-stu-id="f6819-125">Accept</span></span>|<span data-ttu-id="f6819-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6819-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6819-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6819-127">Request body</span></span>
<span data-ttu-id="f6819-128">在请求正文中，提供 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6819-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="f6819-129">下表显示创建 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f6819-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="f6819-130">属性</span><span class="sxs-lookup"><span data-stu-id="f6819-130">Property</span></span>|<span data-ttu-id="f6819-131">类型</span><span class="sxs-lookup"><span data-stu-id="f6819-131">Type</span></span>|<span data-ttu-id="f6819-132">说明</span><span class="sxs-lookup"><span data-stu-id="f6819-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6819-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6819-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f6819-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6819-134">DateTimeOffset</span></span>|<span data-ttu-id="f6819-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f6819-135">The date and time the object was last modified.</span></span> <span data-ttu-id="f6819-136">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f6819-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f6819-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6819-137">createdDateTime</span></span>|<span data-ttu-id="f6819-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6819-138">DateTimeOffset</span></span>|<span data-ttu-id="f6819-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f6819-139">The date and time the object was created.</span></span> <span data-ttu-id="f6819-140">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f6819-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f6819-141">id</span><span class="sxs-lookup"><span data-stu-id="f6819-141">id</span></span>|<span data-ttu-id="f6819-142">String</span><span class="sxs-lookup"><span data-stu-id="f6819-142">String</span></span>|<span data-ttu-id="f6819-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f6819-143">Key of the entity.</span></span> <span data-ttu-id="f6819-144">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f6819-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f6819-145">values</span><span class="sxs-lookup"><span data-stu-id="f6819-145">values</span></span>|<span data-ttu-id="f6819-146">String collection</span><span class="sxs-lookup"><span data-stu-id="f6819-146">String collection</span></span>|<span data-ttu-id="f6819-147">关联演示文稿的非空字符串的集合。</span><span class="sxs-lookup"><span data-stu-id="f6819-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="f6819-148">响应</span><span class="sxs-lookup"><span data-stu-id="f6819-148">Response</span></span>
<span data-ttu-id="f6819-149">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6819-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6819-150">示例</span><span class="sxs-lookup"><span data-stu-id="f6819-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6819-151">请求</span><span class="sxs-lookup"><span data-stu-id="f6819-151">Request</span></span>
<span data-ttu-id="f6819-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6819-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6819-153">响应</span><span class="sxs-lookup"><span data-stu-id="f6819-153">Response</span></span>
<span data-ttu-id="f6819-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6819-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





