---
title: 更新 groupPolicyPresentationValueText
description: 更新 groupPolicyPresentationValueText 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49e65216583e4e928562b5e7b5c053ae97beef3d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157092"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="36454-103">更新 groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="36454-103">Update groupPolicyPresentationValueText</span></span>

<span data-ttu-id="36454-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36454-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36454-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36454-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36454-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36454-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36454-107">更新 [groupPolicyPresentationValueText 对象](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="36454-107">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36454-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="36454-108">Prerequisites</span></span>
<span data-ttu-id="36454-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36454-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36454-111">Permission type</span></span>|<span data-ttu-id="36454-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36454-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36454-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36454-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36454-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36454-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36454-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36454-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36454-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36454-116">Not supported.</span></span>|
|<span data-ttu-id="36454-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36454-117">Application</span></span>|<span data-ttu-id="36454-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36454-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36454-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36454-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="36454-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36454-120">Request headers</span></span>
|<span data-ttu-id="36454-121">标头</span><span class="sxs-lookup"><span data-stu-id="36454-121">Header</span></span>|<span data-ttu-id="36454-122">值</span><span class="sxs-lookup"><span data-stu-id="36454-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36454-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36454-123">Authorization</span></span>|<span data-ttu-id="36454-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36454-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36454-125">接受</span><span class="sxs-lookup"><span data-stu-id="36454-125">Accept</span></span>|<span data-ttu-id="36454-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36454-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36454-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36454-127">Request body</span></span>
<span data-ttu-id="36454-128">在请求正文中，提供 [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36454-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="36454-129">下表显示创建 [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36454-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="36454-130">属性</span><span class="sxs-lookup"><span data-stu-id="36454-130">Property</span></span>|<span data-ttu-id="36454-131">类型</span><span class="sxs-lookup"><span data-stu-id="36454-131">Type</span></span>|<span data-ttu-id="36454-132">说明</span><span class="sxs-lookup"><span data-stu-id="36454-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36454-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36454-133">lastModifiedDateTime</span></span>|<span data-ttu-id="36454-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36454-134">DateTimeOffset</span></span>|<span data-ttu-id="36454-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="36454-135">The date and time the object was last modified.</span></span> <span data-ttu-id="36454-136">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="36454-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="36454-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36454-137">createdDateTime</span></span>|<span data-ttu-id="36454-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36454-138">DateTimeOffset</span></span>|<span data-ttu-id="36454-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="36454-139">The date and time the object was created.</span></span> <span data-ttu-id="36454-140">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="36454-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="36454-141">id</span><span class="sxs-lookup"><span data-stu-id="36454-141">id</span></span>|<span data-ttu-id="36454-142">String</span><span class="sxs-lookup"><span data-stu-id="36454-142">String</span></span>|<span data-ttu-id="36454-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="36454-143">Key of the entity.</span></span> <span data-ttu-id="36454-144">继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="36454-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="36454-145">value</span><span class="sxs-lookup"><span data-stu-id="36454-145">value</span></span>|<span data-ttu-id="36454-146">String</span><span class="sxs-lookup"><span data-stu-id="36454-146">String</span></span>|<span data-ttu-id="36454-147">关联的演示文稿的字符串值。</span><span class="sxs-lookup"><span data-stu-id="36454-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="36454-148">响应</span><span class="sxs-lookup"><span data-stu-id="36454-148">Response</span></span>
<span data-ttu-id="36454-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36454-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36454-150">示例</span><span class="sxs-lookup"><span data-stu-id="36454-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="36454-151">请求</span><span class="sxs-lookup"><span data-stu-id="36454-151">Request</span></span>
<span data-ttu-id="36454-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36454-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="36454-153">响应</span><span class="sxs-lookup"><span data-stu-id="36454-153">Response</span></span>
<span data-ttu-id="36454-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36454-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




