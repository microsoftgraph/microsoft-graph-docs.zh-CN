---
title: 创建 groupPolicyDefinitionValue
description: 创建新的 groupPolicyDefinitionValue 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d859a1405c9b2879da1c9b57f31c1ffde3ce0cfc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429385"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="b289a-103">创建 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="b289a-103">Create groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="b289a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b289a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b289a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b289a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b289a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b289a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b289a-107">创建新的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b289a-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b289a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b289a-108">Prerequisites</span></span>
<span data-ttu-id="b289a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b289a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b289a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b289a-111">Permission type</span></span>|<span data-ttu-id="b289a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b289a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b289a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b289a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b289a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b289a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b289a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b289a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b289a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b289a-116">Not supported.</span></span>|
|<span data-ttu-id="b289a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b289a-117">Application</span></span>|<span data-ttu-id="b289a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b289a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b289a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b289a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="b289a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b289a-120">Request headers</span></span>
|<span data-ttu-id="b289a-121">标头</span><span class="sxs-lookup"><span data-stu-id="b289a-121">Header</span></span>|<span data-ttu-id="b289a-122">值</span><span class="sxs-lookup"><span data-stu-id="b289a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b289a-123">授权</span><span class="sxs-lookup"><span data-stu-id="b289a-123">Authorization</span></span>|<span data-ttu-id="b289a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b289a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b289a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b289a-125">Accept</span></span>|<span data-ttu-id="b289a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b289a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b289a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b289a-127">Request body</span></span>
<span data-ttu-id="b289a-128">在请求正文中，提供 groupPolicyDefinitionValue 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b289a-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="b289a-129">下表显示时创建 groupPolicyDefinitionValue 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b289a-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="b289a-130">属性</span><span class="sxs-lookup"><span data-stu-id="b289a-130">Property</span></span>|<span data-ttu-id="b289a-131">类型</span><span class="sxs-lookup"><span data-stu-id="b289a-131">Type</span></span>|<span data-ttu-id="b289a-132">说明</span><span class="sxs-lookup"><span data-stu-id="b289a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b289a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b289a-133">createdDateTime</span></span>|<span data-ttu-id="b289a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b289a-134">DateTimeOffset</span></span>|<span data-ttu-id="b289a-135">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="b289a-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="b289a-136">enabled</span><span class="sxs-lookup"><span data-stu-id="b289a-136">enabled</span></span>|<span data-ttu-id="b289a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b289a-137">Boolean</span></span>|<span data-ttu-id="b289a-138">启用或禁用相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="b289a-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="b289a-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="b289a-139">configurationType</span></span>|[<span data-ttu-id="b289a-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="b289a-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="b289a-141">指定应如何配置的值。</span><span class="sxs-lookup"><span data-stu-id="b289a-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="b289a-142">这可以是一个策略作为或首选项。</span><span class="sxs-lookup"><span data-stu-id="b289a-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="b289a-143">可取值为：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="b289a-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="b289a-144">id</span><span class="sxs-lookup"><span data-stu-id="b289a-144">id</span></span>|<span data-ttu-id="b289a-145">String</span><span class="sxs-lookup"><span data-stu-id="b289a-145">String</span></span>|<span data-ttu-id="b289a-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b289a-146">Key of the entity.</span></span>|
|<span data-ttu-id="b289a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b289a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="b289a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b289a-148">DateTimeOffset</span></span>|<span data-ttu-id="b289a-149">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="b289a-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b289a-150">响应</span><span class="sxs-lookup"><span data-stu-id="b289a-150">Response</span></span>
<span data-ttu-id="b289a-151">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b289a-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b289a-152">示例</span><span class="sxs-lookup"><span data-stu-id="b289a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b289a-153">请求</span><span class="sxs-lookup"><span data-stu-id="b289a-153">Request</span></span>
<span data-ttu-id="b289a-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b289a-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b289a-155">响应</span><span class="sxs-lookup"><span data-stu-id="b289a-155">Response</span></span>
<span data-ttu-id="b289a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b289a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




