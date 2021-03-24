---
title: 更新 groupPolicyPresentationValueLongDecimal
description: 更新 groupPolicyPresentationValueLongDecimal 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29db585995728b84f6f4157c5e3c61c0ffa3fe7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145731"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="6c750-103">更新 groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="6c750-103">Update groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="6c750-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c750-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c750-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c750-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c750-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c750-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c750-107">更新 [groupPolicyPresentationValueLongDecimal 对象](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6c750-107">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c750-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c750-108">Prerequisites</span></span>
<span data-ttu-id="6c750-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c750-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c750-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c750-111">Permission type</span></span>|<span data-ttu-id="6c750-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c750-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c750-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c750-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c750-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c750-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c750-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c750-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c750-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c750-116">Not supported.</span></span>|
|<span data-ttu-id="6c750-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c750-117">Application</span></span>|<span data-ttu-id="6c750-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c750-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c750-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c750-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="6c750-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c750-120">Request headers</span></span>
|<span data-ttu-id="6c750-121">标头</span><span class="sxs-lookup"><span data-stu-id="6c750-121">Header</span></span>|<span data-ttu-id="6c750-122">值</span><span class="sxs-lookup"><span data-stu-id="6c750-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c750-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c750-123">Authorization</span></span>|<span data-ttu-id="6c750-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c750-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c750-125">接受</span><span class="sxs-lookup"><span data-stu-id="6c750-125">Accept</span></span>|<span data-ttu-id="6c750-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c750-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c750-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c750-127">Request body</span></span>
<span data-ttu-id="6c750-128">在请求正文中，提供 [groupPolicyPresentationValueLongDecimal 对象的](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c750-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="6c750-129">下表显示创建 [groupPolicyPresentationValueLongDecimal 时所需的属性](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)。</span><span class="sxs-lookup"><span data-stu-id="6c750-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="6c750-130">属性</span><span class="sxs-lookup"><span data-stu-id="6c750-130">Property</span></span>|<span data-ttu-id="6c750-131">类型</span><span class="sxs-lookup"><span data-stu-id="6c750-131">Type</span></span>|<span data-ttu-id="6c750-132">说明</span><span class="sxs-lookup"><span data-stu-id="6c750-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c750-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c750-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6c750-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c750-134">DateTimeOffset</span></span>|<span data-ttu-id="6c750-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6c750-135">The date and time the object was last modified.</span></span> <span data-ttu-id="6c750-136">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6c750-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6c750-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c750-137">createdDateTime</span></span>|<span data-ttu-id="6c750-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c750-138">DateTimeOffset</span></span>|<span data-ttu-id="6c750-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6c750-139">The date and time the object was created.</span></span> <span data-ttu-id="6c750-140">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6c750-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6c750-141">id</span><span class="sxs-lookup"><span data-stu-id="6c750-141">id</span></span>|<span data-ttu-id="6c750-142">String</span><span class="sxs-lookup"><span data-stu-id="6c750-142">String</span></span>|<span data-ttu-id="6c750-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c750-143">Key of the entity.</span></span> <span data-ttu-id="6c750-144">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6c750-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6c750-145">值</span><span class="sxs-lookup"><span data-stu-id="6c750-145">value</span></span>|<span data-ttu-id="6c750-146">Int64</span><span class="sxs-lookup"><span data-stu-id="6c750-146">Int64</span></span>|<span data-ttu-id="6c750-147">关联的演示文稿的无符号长值。</span><span class="sxs-lookup"><span data-stu-id="6c750-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="6c750-148">响应</span><span class="sxs-lookup"><span data-stu-id="6c750-148">Response</span></span>
<span data-ttu-id="6c750-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c750-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c750-150">示例</span><span class="sxs-lookup"><span data-stu-id="6c750-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c750-151">请求</span><span class="sxs-lookup"><span data-stu-id="6c750-151">Request</span></span>
<span data-ttu-id="6c750-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c750-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="6c750-153">响应</span><span class="sxs-lookup"><span data-stu-id="6c750-153">Response</span></span>
<span data-ttu-id="6c750-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c750-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```




