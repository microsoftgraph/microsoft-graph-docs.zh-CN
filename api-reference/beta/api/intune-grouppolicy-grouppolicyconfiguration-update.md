---
title: 更新 groupPolicyConfiguration
description: 更新 groupPolicyConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 30ce815eef79de3fa091daede34c758699f27bc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429562"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="1d461-103">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d461-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="1d461-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1d461-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d461-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1d461-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d461-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d461-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d461-107">更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1d461-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d461-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d461-108">Prerequisites</span></span>
<span data-ttu-id="1d461-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1d461-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d461-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d461-111">Permission type</span></span>|<span data-ttu-id="1d461-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1d461-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d461-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d461-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d461-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d461-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d461-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d461-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d461-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d461-116">Not supported.</span></span>|
|<span data-ttu-id="1d461-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d461-117">Application</span></span>|<span data-ttu-id="1d461-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d461-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d461-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d461-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1d461-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d461-120">Request headers</span></span>
|<span data-ttu-id="1d461-121">标头</span><span class="sxs-lookup"><span data-stu-id="1d461-121">Header</span></span>|<span data-ttu-id="1d461-122">值</span><span class="sxs-lookup"><span data-stu-id="1d461-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d461-123">授权</span><span class="sxs-lookup"><span data-stu-id="1d461-123">Authorization</span></span>|<span data-ttu-id="1d461-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d461-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d461-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d461-125">Accept</span></span>|<span data-ttu-id="1d461-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d461-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d461-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d461-127">Request body</span></span>
<span data-ttu-id="1d461-128">在请求正文中，提供[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d461-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="1d461-129">下表显示时创建[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1d461-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="1d461-130">属性</span><span class="sxs-lookup"><span data-stu-id="1d461-130">Property</span></span>|<span data-ttu-id="1d461-131">类型</span><span class="sxs-lookup"><span data-stu-id="1d461-131">Type</span></span>|<span data-ttu-id="1d461-132">说明</span><span class="sxs-lookup"><span data-stu-id="1d461-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d461-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d461-133">createdDateTime</span></span>|<span data-ttu-id="1d461-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d461-134">DateTimeOffset</span></span>|<span data-ttu-id="1d461-135">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="1d461-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="1d461-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1d461-136">displayName</span></span>|<span data-ttu-id="1d461-137">String</span><span class="sxs-lookup"><span data-stu-id="1d461-137">String</span></span>|<span data-ttu-id="1d461-138">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="1d461-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="1d461-139">说明</span><span class="sxs-lookup"><span data-stu-id="1d461-139">description</span></span>|<span data-ttu-id="1d461-140">String</span><span class="sxs-lookup"><span data-stu-id="1d461-140">String</span></span>|<span data-ttu-id="1d461-141">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="1d461-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="1d461-142">id</span><span class="sxs-lookup"><span data-stu-id="1d461-142">id</span></span>|<span data-ttu-id="1d461-143">String</span><span class="sxs-lookup"><span data-stu-id="1d461-143">String</span></span>|<span data-ttu-id="1d461-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1d461-144">Key of the entity.</span></span>|
|<span data-ttu-id="1d461-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d461-145">lastModifiedDateTime</span></span>|<span data-ttu-id="1d461-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d461-146">DateTimeOffset</span></span>|<span data-ttu-id="1d461-147">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="1d461-147">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="1d461-148">响应</span><span class="sxs-lookup"><span data-stu-id="1d461-148">Response</span></span>
<span data-ttu-id="1d461-149">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1d461-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d461-150">示例</span><span class="sxs-lookup"><span data-stu-id="1d461-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d461-151">请求</span><span class="sxs-lookup"><span data-stu-id="1d461-151">Request</span></span>
<span data-ttu-id="1d461-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d461-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="1d461-153">响应</span><span class="sxs-lookup"><span data-stu-id="1d461-153">Response</span></span>
<span data-ttu-id="1d461-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d461-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




