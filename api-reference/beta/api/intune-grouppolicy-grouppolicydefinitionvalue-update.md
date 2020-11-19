---
title: 更新 groupPolicyDefinitionValue
description: 更新 groupPolicyDefinitionValue 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 539cbeacdc873569a54c03c1b10cbcd67079fb86
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49262838"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="0d331-103">更新 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="0d331-103">Update groupPolicyDefinitionValue</span></span>

<span data-ttu-id="0d331-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d331-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d331-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d331-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d331-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d331-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d331-107">更新 [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0d331-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d331-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0d331-108">Prerequisites</span></span>
<span data-ttu-id="0d331-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d331-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d331-111">Permission type</span></span>|<span data-ttu-id="0d331-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0d331-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d331-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d331-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d331-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d331-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d331-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d331-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d331-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d331-116">Not supported.</span></span>|
|<span data-ttu-id="0d331-117">Application</span><span class="sxs-lookup"><span data-stu-id="0d331-117">Application</span></span>|<span data-ttu-id="0d331-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d331-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d331-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d331-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="0d331-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d331-120">Request headers</span></span>
|<span data-ttu-id="0d331-121">标头</span><span class="sxs-lookup"><span data-stu-id="0d331-121">Header</span></span>|<span data-ttu-id="0d331-122">值</span><span class="sxs-lookup"><span data-stu-id="0d331-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d331-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d331-123">Authorization</span></span>|<span data-ttu-id="0d331-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0d331-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d331-125">接受</span><span class="sxs-lookup"><span data-stu-id="0d331-125">Accept</span></span>|<span data-ttu-id="0d331-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d331-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d331-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d331-127">Request body</span></span>
<span data-ttu-id="0d331-128">在请求正文中，提供 [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d331-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="0d331-129">下表显示创建 [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0d331-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="0d331-130">属性</span><span class="sxs-lookup"><span data-stu-id="0d331-130">Property</span></span>|<span data-ttu-id="0d331-131">类型</span><span class="sxs-lookup"><span data-stu-id="0d331-131">Type</span></span>|<span data-ttu-id="0d331-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d331-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d331-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d331-133">createdDateTime</span></span>|<span data-ttu-id="0d331-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d331-134">DateTimeOffset</span></span>|<span data-ttu-id="0d331-135">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0d331-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="0d331-136">enabled</span><span class="sxs-lookup"><span data-stu-id="0d331-136">enabled</span></span>|<span data-ttu-id="0d331-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d331-137">Boolean</span></span>|<span data-ttu-id="0d331-138">启用或禁用关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="0d331-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="0d331-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="0d331-139">configurationType</span></span>|[<span data-ttu-id="0d331-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="0d331-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="0d331-141">指定应如何配置值。</span><span class="sxs-lookup"><span data-stu-id="0d331-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="0d331-142">这可以是策略，也可以是首选项。</span><span class="sxs-lookup"><span data-stu-id="0d331-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="0d331-143">可能的值是：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="0d331-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="0d331-144">id</span><span class="sxs-lookup"><span data-stu-id="0d331-144">id</span></span>|<span data-ttu-id="0d331-145">字符串</span><span class="sxs-lookup"><span data-stu-id="0d331-145">String</span></span>|<span data-ttu-id="0d331-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0d331-146">Key of the entity.</span></span>|
|<span data-ttu-id="0d331-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d331-147">lastModifiedDateTime</span></span>|<span data-ttu-id="0d331-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d331-148">DateTimeOffset</span></span>|<span data-ttu-id="0d331-149">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0d331-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0d331-150">响应</span><span class="sxs-lookup"><span data-stu-id="0d331-150">Response</span></span>
<span data-ttu-id="0d331-151">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d331-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d331-152">示例</span><span class="sxs-lookup"><span data-stu-id="0d331-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d331-153">请求</span><span class="sxs-lookup"><span data-stu-id="0d331-153">Request</span></span>
<span data-ttu-id="0d331-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d331-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d331-155">响应</span><span class="sxs-lookup"><span data-stu-id="0d331-155">Response</span></span>
<span data-ttu-id="0d331-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d331-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




