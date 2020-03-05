---
title: 创建 groupPolicyPresentationValueText
description: 创建新的 groupPolicyPresentationValueText 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d55d0722bd2dea44c1c4f787a72d183b202d6535
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463957"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="729d9-103">创建 groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="729d9-103">Create groupPolicyPresentationValueText</span></span>

<span data-ttu-id="729d9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="729d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="729d9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="729d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="729d9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="729d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="729d9-107">创建新的[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="729d9-107">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="729d9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="729d9-108">Prerequisites</span></span>
<span data-ttu-id="729d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="729d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="729d9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="729d9-111">Permission type</span></span>|<span data-ttu-id="729d9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="729d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="729d9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="729d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="729d9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="729d9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="729d9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="729d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="729d9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="729d9-116">Not supported.</span></span>|
|<span data-ttu-id="729d9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="729d9-117">Application</span></span>|<span data-ttu-id="729d9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="729d9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="729d9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="729d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="729d9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="729d9-120">Request headers</span></span>
|<span data-ttu-id="729d9-121">标头</span><span class="sxs-lookup"><span data-stu-id="729d9-121">Header</span></span>|<span data-ttu-id="729d9-122">值</span><span class="sxs-lookup"><span data-stu-id="729d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="729d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="729d9-123">Authorization</span></span>|<span data-ttu-id="729d9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="729d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="729d9-125">接受</span><span class="sxs-lookup"><span data-stu-id="729d9-125">Accept</span></span>|<span data-ttu-id="729d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="729d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="729d9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="729d9-127">Request body</span></span>
<span data-ttu-id="729d9-128">在请求正文中，提供 groupPolicyPresentationValueText 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="729d9-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="729d9-129">下表显示创建 groupPolicyPresentationValueText 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="729d9-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="729d9-130">属性</span><span class="sxs-lookup"><span data-stu-id="729d9-130">Property</span></span>|<span data-ttu-id="729d9-131">类型</span><span class="sxs-lookup"><span data-stu-id="729d9-131">Type</span></span>|<span data-ttu-id="729d9-132">说明</span><span class="sxs-lookup"><span data-stu-id="729d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="729d9-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="729d9-133">lastModifiedDateTime</span></span>|<span data-ttu-id="729d9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="729d9-134">DateTimeOffset</span></span>|<span data-ttu-id="729d9-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="729d9-135">The date and time the object was last modified.</span></span> <span data-ttu-id="729d9-136">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="729d9-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="729d9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="729d9-137">createdDateTime</span></span>|<span data-ttu-id="729d9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="729d9-138">DateTimeOffset</span></span>|<span data-ttu-id="729d9-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="729d9-139">The date and time the object was created.</span></span> <span data-ttu-id="729d9-140">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="729d9-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="729d9-141">id</span><span class="sxs-lookup"><span data-stu-id="729d9-141">id</span></span>|<span data-ttu-id="729d9-142">String</span><span class="sxs-lookup"><span data-stu-id="729d9-142">String</span></span>|<span data-ttu-id="729d9-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="729d9-143">Key of the entity.</span></span> <span data-ttu-id="729d9-144">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="729d9-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="729d9-145">value</span><span class="sxs-lookup"><span data-stu-id="729d9-145">value</span></span>|<span data-ttu-id="729d9-146">String</span><span class="sxs-lookup"><span data-stu-id="729d9-146">String</span></span>|<span data-ttu-id="729d9-147">关联的演示文稿的字符串值。</span><span class="sxs-lookup"><span data-stu-id="729d9-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="729d9-148">响应</span><span class="sxs-lookup"><span data-stu-id="729d9-148">Response</span></span>
<span data-ttu-id="729d9-149">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="729d9-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="729d9-150">示例</span><span class="sxs-lookup"><span data-stu-id="729d9-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="729d9-151">请求</span><span class="sxs-lookup"><span data-stu-id="729d9-151">Request</span></span>
<span data-ttu-id="729d9-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="729d9-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="729d9-153">响应</span><span class="sxs-lookup"><span data-stu-id="729d9-153">Response</span></span>
<span data-ttu-id="729d9-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="729d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```





