---
title: 更新 groupPolicyPresentationValueLongDecimal
description: 更新 groupPolicyPresentationValueLongDecimal 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5264964eaf3882f83e48be3fb92bbed3065ce03a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771353"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="74e1c-103">更新 groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="74e1c-103">Update groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="74e1c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74e1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74e1c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74e1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74e1c-106">更新[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74e1c-106">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74e1c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="74e1c-107">Prerequisites</span></span>
<span data-ttu-id="74e1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74e1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e1c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="74e1c-110">Permission type</span></span>|<span data-ttu-id="74e1c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74e1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74e1c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74e1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74e1c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e1c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74e1c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74e1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74e1c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="74e1c-115">Not supported.</span></span>|
|<span data-ttu-id="74e1c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="74e1c-116">Application</span></span>|<span data-ttu-id="74e1c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="74e1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74e1c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74e1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="74e1c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="74e1c-119">Request headers</span></span>
|<span data-ttu-id="74e1c-120">标头</span><span class="sxs-lookup"><span data-stu-id="74e1c-120">Header</span></span>|<span data-ttu-id="74e1c-121">值</span><span class="sxs-lookup"><span data-stu-id="74e1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74e1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e1c-122">Authorization</span></span>|<span data-ttu-id="74e1c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74e1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74e1c-124">接受</span><span class="sxs-lookup"><span data-stu-id="74e1c-124">Accept</span></span>|<span data-ttu-id="74e1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74e1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e1c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="74e1c-126">Request body</span></span>
<span data-ttu-id="74e1c-127">在请求正文中, 提供[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74e1c-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="74e1c-128">下表显示创建[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74e1c-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="74e1c-129">属性</span><span class="sxs-lookup"><span data-stu-id="74e1c-129">Property</span></span>|<span data-ttu-id="74e1c-130">类型</span><span class="sxs-lookup"><span data-stu-id="74e1c-130">Type</span></span>|<span data-ttu-id="74e1c-131">说明</span><span class="sxs-lookup"><span data-stu-id="74e1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74e1c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74e1c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="74e1c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74e1c-133">DateTimeOffset</span></span>|<span data-ttu-id="74e1c-134">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="74e1c-134">The date and time the object was last modified.</span></span> <span data-ttu-id="74e1c-135">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="74e1c-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="74e1c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74e1c-136">createdDateTime</span></span>|<span data-ttu-id="74e1c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74e1c-137">DateTimeOffset</span></span>|<span data-ttu-id="74e1c-138">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="74e1c-138">The date and time the object was created.</span></span> <span data-ttu-id="74e1c-139">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="74e1c-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="74e1c-140">id</span><span class="sxs-lookup"><span data-stu-id="74e1c-140">id</span></span>|<span data-ttu-id="74e1c-141">String</span><span class="sxs-lookup"><span data-stu-id="74e1c-141">String</span></span>|<span data-ttu-id="74e1c-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74e1c-142">Key of the entity.</span></span> <span data-ttu-id="74e1c-143">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="74e1c-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="74e1c-144">value</span><span class="sxs-lookup"><span data-stu-id="74e1c-144">value</span></span>|<span data-ttu-id="74e1c-145">Int64</span><span class="sxs-lookup"><span data-stu-id="74e1c-145">Int64</span></span>|<span data-ttu-id="74e1c-146">关联演示文稿的无符号长值。</span><span class="sxs-lookup"><span data-stu-id="74e1c-146">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="74e1c-147">响应</span><span class="sxs-lookup"><span data-stu-id="74e1c-147">Response</span></span>
<span data-ttu-id="74e1c-148">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74e1c-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e1c-149">示例</span><span class="sxs-lookup"><span data-stu-id="74e1c-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="74e1c-150">请求</span><span class="sxs-lookup"><span data-stu-id="74e1c-150">Request</span></span>
<span data-ttu-id="74e1c-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74e1c-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="74e1c-152">响应</span><span class="sxs-lookup"><span data-stu-id="74e1c-152">Response</span></span>
<span data-ttu-id="74e1c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74e1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





