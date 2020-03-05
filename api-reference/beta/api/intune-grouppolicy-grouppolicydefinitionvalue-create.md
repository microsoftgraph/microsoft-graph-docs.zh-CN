---
title: 创建 groupPolicyDefinitionValue
description: 创建新的 groupPolicyDefinitionValue 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ca08cc47517d16103b3133dfe8aa5e16838fec4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465042"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="9b85c-103">创建 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="9b85c-103">Create groupPolicyDefinitionValue</span></span>

<span data-ttu-id="9b85c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9b85c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b85c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b85c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b85c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b85c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b85c-107">创建新的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b85c-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b85c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9b85c-108">Prerequisites</span></span>
<span data-ttu-id="9b85c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b85c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b85c-111">Permission type</span></span>|<span data-ttu-id="9b85c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9b85c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b85c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b85c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b85c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b85c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9b85c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b85c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b85c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b85c-116">Not supported.</span></span>|
|<span data-ttu-id="9b85c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b85c-117">Application</span></span>|<span data-ttu-id="9b85c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b85c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b85c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b85c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="9b85c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b85c-120">Request headers</span></span>
|<span data-ttu-id="9b85c-121">标头</span><span class="sxs-lookup"><span data-stu-id="9b85c-121">Header</span></span>|<span data-ttu-id="9b85c-122">值</span><span class="sxs-lookup"><span data-stu-id="9b85c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b85c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b85c-123">Authorization</span></span>|<span data-ttu-id="9b85c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9b85c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b85c-125">接受</span><span class="sxs-lookup"><span data-stu-id="9b85c-125">Accept</span></span>|<span data-ttu-id="9b85c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b85c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b85c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b85c-127">Request body</span></span>
<span data-ttu-id="9b85c-128">在请求正文中，提供 groupPolicyDefinitionValue 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b85c-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="9b85c-129">下表显示创建 groupPolicyDefinitionValue 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9b85c-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="9b85c-130">属性</span><span class="sxs-lookup"><span data-stu-id="9b85c-130">Property</span></span>|<span data-ttu-id="9b85c-131">类型</span><span class="sxs-lookup"><span data-stu-id="9b85c-131">Type</span></span>|<span data-ttu-id="9b85c-132">说明</span><span class="sxs-lookup"><span data-stu-id="9b85c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b85c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b85c-133">createdDateTime</span></span>|<span data-ttu-id="9b85c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b85c-134">DateTimeOffset</span></span>|<span data-ttu-id="9b85c-135">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9b85c-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="9b85c-136">enabled</span><span class="sxs-lookup"><span data-stu-id="9b85c-136">enabled</span></span>|<span data-ttu-id="9b85c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b85c-137">Boolean</span></span>|<span data-ttu-id="9b85c-138">启用或禁用关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="9b85c-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="9b85c-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="9b85c-139">configurationType</span></span>|[<span data-ttu-id="9b85c-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="9b85c-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="9b85c-141">指定应如何配置值。</span><span class="sxs-lookup"><span data-stu-id="9b85c-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="9b85c-142">这可以是策略，也可以是首选项。</span><span class="sxs-lookup"><span data-stu-id="9b85c-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="9b85c-143">可能的值是：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="9b85c-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="9b85c-144">id</span><span class="sxs-lookup"><span data-stu-id="9b85c-144">id</span></span>|<span data-ttu-id="9b85c-145">String</span><span class="sxs-lookup"><span data-stu-id="9b85c-145">String</span></span>|<span data-ttu-id="9b85c-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b85c-146">Key of the entity.</span></span>|
|<span data-ttu-id="9b85c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b85c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="9b85c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b85c-148">DateTimeOffset</span></span>|<span data-ttu-id="9b85c-149">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9b85c-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="9b85c-150">响应</span><span class="sxs-lookup"><span data-stu-id="9b85c-150">Response</span></span>
<span data-ttu-id="9b85c-151">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b85c-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b85c-152">示例</span><span class="sxs-lookup"><span data-stu-id="9b85c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b85c-153">请求</span><span class="sxs-lookup"><span data-stu-id="9b85c-153">Request</span></span>
<span data-ttu-id="9b85c-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b85c-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="9b85c-155">响应</span><span class="sxs-lookup"><span data-stu-id="9b85c-155">Response</span></span>
<span data-ttu-id="9b85c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b85c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





