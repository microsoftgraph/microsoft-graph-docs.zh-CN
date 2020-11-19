---
title: 创建 groupPolicyPresentationValueLongDecimal
description: 创建新的 groupPolicyPresentationValueLongDecimal 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0176aec5c67c851c923d23e5218e1888cecb1423
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300113"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="60a40-103">创建 groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="60a40-103">Create groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="60a40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60a40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60a40-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="60a40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60a40-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60a40-107">创建新的 [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60a40-107">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60a40-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="60a40-108">Prerequisites</span></span>
<span data-ttu-id="60a40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a40-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="60a40-111">Permission type</span></span>|<span data-ttu-id="60a40-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60a40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60a40-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60a40-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60a40-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60a40-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60a40-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60a40-116">Not supported.</span></span>|
|<span data-ttu-id="60a40-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60a40-117">Application</span></span>|<span data-ttu-id="60a40-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60a40-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60a40-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="60a40-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60a40-120">Request headers</span></span>
|<span data-ttu-id="60a40-121">标头</span><span class="sxs-lookup"><span data-stu-id="60a40-121">Header</span></span>|<span data-ttu-id="60a40-122">值</span><span class="sxs-lookup"><span data-stu-id="60a40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60a40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a40-123">Authorization</span></span>|<span data-ttu-id="60a40-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60a40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60a40-125">接受</span><span class="sxs-lookup"><span data-stu-id="60a40-125">Accept</span></span>|<span data-ttu-id="60a40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60a40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60a40-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60a40-127">Request body</span></span>
<span data-ttu-id="60a40-128">在请求正文中，提供 groupPolicyPresentationValueLongDecimal 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60a40-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="60a40-129">下表显示创建 groupPolicyPresentationValueLongDecimal 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60a40-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="60a40-130">属性</span><span class="sxs-lookup"><span data-stu-id="60a40-130">Property</span></span>|<span data-ttu-id="60a40-131">类型</span><span class="sxs-lookup"><span data-stu-id="60a40-131">Type</span></span>|<span data-ttu-id="60a40-132">Description</span><span class="sxs-lookup"><span data-stu-id="60a40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60a40-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60a40-133">lastModifiedDateTime</span></span>|<span data-ttu-id="60a40-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60a40-134">DateTimeOffset</span></span>|<span data-ttu-id="60a40-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="60a40-135">The date and time the object was last modified.</span></span> <span data-ttu-id="60a40-136">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="60a40-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="60a40-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60a40-137">createdDateTime</span></span>|<span data-ttu-id="60a40-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60a40-138">DateTimeOffset</span></span>|<span data-ttu-id="60a40-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="60a40-139">The date and time the object was created.</span></span> <span data-ttu-id="60a40-140">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="60a40-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="60a40-141">id</span><span class="sxs-lookup"><span data-stu-id="60a40-141">id</span></span>|<span data-ttu-id="60a40-142">字符串</span><span class="sxs-lookup"><span data-stu-id="60a40-142">String</span></span>|<span data-ttu-id="60a40-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60a40-143">Key of the entity.</span></span> <span data-ttu-id="60a40-144">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="60a40-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="60a40-145">值</span><span class="sxs-lookup"><span data-stu-id="60a40-145">value</span></span>|<span data-ttu-id="60a40-146">Int64</span><span class="sxs-lookup"><span data-stu-id="60a40-146">Int64</span></span>|<span data-ttu-id="60a40-147">关联演示文稿的无符号长值。</span><span class="sxs-lookup"><span data-stu-id="60a40-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="60a40-148">响应</span><span class="sxs-lookup"><span data-stu-id="60a40-148">Response</span></span>
<span data-ttu-id="60a40-149">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60a40-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a40-150">示例</span><span class="sxs-lookup"><span data-stu-id="60a40-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="60a40-151">请求</span><span class="sxs-lookup"><span data-stu-id="60a40-151">Request</span></span>
<span data-ttu-id="60a40-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60a40-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="60a40-153">响应</span><span class="sxs-lookup"><span data-stu-id="60a40-153">Response</span></span>
<span data-ttu-id="60a40-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60a40-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




