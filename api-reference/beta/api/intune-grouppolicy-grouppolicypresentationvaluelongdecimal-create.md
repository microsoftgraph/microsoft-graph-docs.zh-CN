---
title: 创建 groupPolicyPresentationValueLongDecimal
description: 创建新的 groupPolicyPresentationValueLongDecimal 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 51dacbea1970d042d4fe1fb5b3b2bd42f522b131
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429501"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="9e7a2-103">创建 groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="9e7a2-103">Create groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="9e7a2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e7a2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e7a2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e7a2-107">创建新的[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-107">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e7a2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e7a2-108">Prerequisites</span></span>
<span data-ttu-id="9e7a2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e7a2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e7a2-111">Permission type</span></span>|<span data-ttu-id="9e7a2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e7a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e7a2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e7a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e7a2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e7a2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9e7a2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e7a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e7a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-116">Not supported.</span></span>|
|<span data-ttu-id="9e7a2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e7a2-117">Application</span></span>|<span data-ttu-id="9e7a2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e7a2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e7a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="9e7a2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e7a2-120">Request headers</span></span>
|<span data-ttu-id="9e7a2-121">标头</span><span class="sxs-lookup"><span data-stu-id="9e7a2-121">Header</span></span>|<span data-ttu-id="9e7a2-122">值</span><span class="sxs-lookup"><span data-stu-id="9e7a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e7a2-123">授权</span><span class="sxs-lookup"><span data-stu-id="9e7a2-123">Authorization</span></span>|<span data-ttu-id="9e7a2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e7a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e7a2-125">Accept</span></span>|<span data-ttu-id="9e7a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e7a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e7a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e7a2-127">Request body</span></span>
<span data-ttu-id="9e7a2-128">在请求正文中，提供 groupPolicyPresentationValueLongDecimal 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="9e7a2-129">下表显示时创建 groupPolicyPresentationValueLongDecimal 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="9e7a2-130">属性</span><span class="sxs-lookup"><span data-stu-id="9e7a2-130">Property</span></span>|<span data-ttu-id="9e7a2-131">类型</span><span class="sxs-lookup"><span data-stu-id="9e7a2-131">Type</span></span>|<span data-ttu-id="9e7a2-132">说明</span><span class="sxs-lookup"><span data-stu-id="9e7a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e7a2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e7a2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="9e7a2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e7a2-134">DateTimeOffset</span></span>|<span data-ttu-id="9e7a2-135">日期和时间上次修改对象。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-135">The date and time the object was last modified.</span></span> <span data-ttu-id="9e7a2-136">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9e7a2-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9e7a2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e7a2-137">createdDateTime</span></span>|<span data-ttu-id="9e7a2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e7a2-138">DateTimeOffset</span></span>|<span data-ttu-id="9e7a2-139">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-139">The date and time the object was created.</span></span> <span data-ttu-id="9e7a2-140">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9e7a2-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9e7a2-141">id</span><span class="sxs-lookup"><span data-stu-id="9e7a2-141">id</span></span>|<span data-ttu-id="9e7a2-142">String</span><span class="sxs-lookup"><span data-stu-id="9e7a2-142">String</span></span>|<span data-ttu-id="9e7a2-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-143">Key of the entity.</span></span> <span data-ttu-id="9e7a2-144">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9e7a2-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9e7a2-145">值</span><span class="sxs-lookup"><span data-stu-id="9e7a2-145">value</span></span>|<span data-ttu-id="9e7a2-146">Int64</span><span class="sxs-lookup"><span data-stu-id="9e7a2-146">Int64</span></span>|<span data-ttu-id="9e7a2-147">关联的演示文稿未签署的 long 值。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="9e7a2-148">响应</span><span class="sxs-lookup"><span data-stu-id="9e7a2-148">Response</span></span>
<span data-ttu-id="9e7a2-149">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e7a2-150">示例</span><span class="sxs-lookup"><span data-stu-id="9e7a2-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e7a2-151">请求</span><span class="sxs-lookup"><span data-stu-id="9e7a2-151">Request</span></span>
<span data-ttu-id="9e7a2-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="9e7a2-153">响应</span><span class="sxs-lookup"><span data-stu-id="9e7a2-153">Response</span></span>
<span data-ttu-id="9e7a2-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e7a2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




