---
title: 更新 groupPolicyDefinitionValue
description: 更新 groupPolicyDefinitionValue 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d346a40e5ee8c2cba6f1510cf52d747e85a0b788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429288"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="41004-103">更新 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="41004-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="41004-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="41004-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="41004-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41004-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41004-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41004-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41004-107">更新[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41004-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41004-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41004-108">Prerequisites</span></span>
<span data-ttu-id="41004-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="41004-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="41004-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41004-111">Permission type</span></span>|<span data-ttu-id="41004-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41004-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41004-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41004-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41004-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41004-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="41004-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41004-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41004-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41004-116">Not supported.</span></span>|
|<span data-ttu-id="41004-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41004-117">Application</span></span>|<span data-ttu-id="41004-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="41004-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41004-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41004-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="41004-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41004-120">Request headers</span></span>
|<span data-ttu-id="41004-121">标头</span><span class="sxs-lookup"><span data-stu-id="41004-121">Header</span></span>|<span data-ttu-id="41004-122">值</span><span class="sxs-lookup"><span data-stu-id="41004-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41004-123">授权</span><span class="sxs-lookup"><span data-stu-id="41004-123">Authorization</span></span>|<span data-ttu-id="41004-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41004-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41004-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41004-125">Accept</span></span>|<span data-ttu-id="41004-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41004-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41004-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41004-127">Request body</span></span>
<span data-ttu-id="41004-128">在请求正文中，提供[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41004-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="41004-129">下表显示时创建[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41004-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="41004-130">属性</span><span class="sxs-lookup"><span data-stu-id="41004-130">Property</span></span>|<span data-ttu-id="41004-131">类型</span><span class="sxs-lookup"><span data-stu-id="41004-131">Type</span></span>|<span data-ttu-id="41004-132">说明</span><span class="sxs-lookup"><span data-stu-id="41004-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41004-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41004-133">createdDateTime</span></span>|<span data-ttu-id="41004-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41004-134">DateTimeOffset</span></span>|<span data-ttu-id="41004-135">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="41004-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="41004-136">enabled</span><span class="sxs-lookup"><span data-stu-id="41004-136">enabled</span></span>|<span data-ttu-id="41004-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="41004-137">Boolean</span></span>|<span data-ttu-id="41004-138">启用或禁用相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="41004-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="41004-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="41004-139">configurationType</span></span>|[<span data-ttu-id="41004-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="41004-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="41004-141">指定应如何配置的值。</span><span class="sxs-lookup"><span data-stu-id="41004-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="41004-142">这可以是一个策略作为或首选项。</span><span class="sxs-lookup"><span data-stu-id="41004-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="41004-143">可取值为：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="41004-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="41004-144">id</span><span class="sxs-lookup"><span data-stu-id="41004-144">id</span></span>|<span data-ttu-id="41004-145">String</span><span class="sxs-lookup"><span data-stu-id="41004-145">String</span></span>|<span data-ttu-id="41004-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41004-146">Key of the entity.</span></span>|
|<span data-ttu-id="41004-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41004-147">lastModifiedDateTime</span></span>|<span data-ttu-id="41004-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41004-148">DateTimeOffset</span></span>|<span data-ttu-id="41004-149">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="41004-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="41004-150">响应</span><span class="sxs-lookup"><span data-stu-id="41004-150">Response</span></span>
<span data-ttu-id="41004-151">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41004-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41004-152">示例</span><span class="sxs-lookup"><span data-stu-id="41004-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="41004-153">请求</span><span class="sxs-lookup"><span data-stu-id="41004-153">Request</span></span>
<span data-ttu-id="41004-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41004-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41004-155">响应</span><span class="sxs-lookup"><span data-stu-id="41004-155">Response</span></span>
<span data-ttu-id="41004-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41004-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




