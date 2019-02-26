---
title: 更新 groupPolicyDefinitionValue
description: 更新 groupPolicyDefinitionValue 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 808136183ebbeb1a6691ab8ccf22b527950bf91d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169704"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="159fb-103">更新 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="159fb-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="159fb-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="159fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="159fb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="159fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="159fb-106">更新[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="159fb-106">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="159fb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="159fb-107">Prerequisites</span></span>
<span data-ttu-id="159fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="159fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="159fb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="159fb-110">Permission type</span></span>|<span data-ttu-id="159fb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="159fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="159fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="159fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="159fb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="159fb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="159fb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="159fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="159fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="159fb-115">Not supported.</span></span>|
|<span data-ttu-id="159fb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="159fb-116">Application</span></span>|<span data-ttu-id="159fb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="159fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="159fb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="159fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="159fb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="159fb-119">Request headers</span></span>
|<span data-ttu-id="159fb-120">标头</span><span class="sxs-lookup"><span data-stu-id="159fb-120">Header</span></span>|<span data-ttu-id="159fb-121">值</span><span class="sxs-lookup"><span data-stu-id="159fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="159fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="159fb-122">Authorization</span></span>|<span data-ttu-id="159fb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="159fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="159fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="159fb-124">Accept</span></span>|<span data-ttu-id="159fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="159fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="159fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="159fb-126">Request body</span></span>
<span data-ttu-id="159fb-127">在请求正文中, 提供[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="159fb-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="159fb-128">下表显示创建[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="159fb-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="159fb-129">属性</span><span class="sxs-lookup"><span data-stu-id="159fb-129">Property</span></span>|<span data-ttu-id="159fb-130">类型</span><span class="sxs-lookup"><span data-stu-id="159fb-130">Type</span></span>|<span data-ttu-id="159fb-131">说明</span><span class="sxs-lookup"><span data-stu-id="159fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="159fb-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="159fb-132">createdDateTime</span></span>|<span data-ttu-id="159fb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="159fb-133">DateTimeOffset</span></span>|<span data-ttu-id="159fb-134">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="159fb-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="159fb-135">enabled</span><span class="sxs-lookup"><span data-stu-id="159fb-135">enabled</span></span>|<span data-ttu-id="159fb-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="159fb-136">Boolean</span></span>|<span data-ttu-id="159fb-137">启用或禁用关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="159fb-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="159fb-138">configurationType</span><span class="sxs-lookup"><span data-stu-id="159fb-138">configurationType</span></span>|[<span data-ttu-id="159fb-139">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="159fb-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="159fb-140">指定应如何配置值。</span><span class="sxs-lookup"><span data-stu-id="159fb-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="159fb-141">这可以是策略, 也可以是首选项。</span><span class="sxs-lookup"><span data-stu-id="159fb-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="159fb-142">可取值为：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="159fb-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="159fb-143">id</span><span class="sxs-lookup"><span data-stu-id="159fb-143">id</span></span>|<span data-ttu-id="159fb-144">String</span><span class="sxs-lookup"><span data-stu-id="159fb-144">String</span></span>|<span data-ttu-id="159fb-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="159fb-145">Key of the entity.</span></span>|
|<span data-ttu-id="159fb-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="159fb-146">lastModifiedDateTime</span></span>|<span data-ttu-id="159fb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="159fb-147">DateTimeOffset</span></span>|<span data-ttu-id="159fb-148">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="159fb-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="159fb-149">响应</span><span class="sxs-lookup"><span data-stu-id="159fb-149">Response</span></span>
<span data-ttu-id="159fb-150">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="159fb-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="159fb-151">示例</span><span class="sxs-lookup"><span data-stu-id="159fb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="159fb-152">请求</span><span class="sxs-lookup"><span data-stu-id="159fb-152">Request</span></span>
<span data-ttu-id="159fb-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="159fb-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="159fb-154">响应</span><span class="sxs-lookup"><span data-stu-id="159fb-154">Response</span></span>
<span data-ttu-id="159fb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="159fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




