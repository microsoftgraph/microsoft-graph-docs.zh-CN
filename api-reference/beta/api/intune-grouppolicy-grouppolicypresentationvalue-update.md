---
title: 更新 groupPolicyPresentationValue
description: 更新 groupPolicyPresentationValue 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfec8c5c0a228bf4ba1ed360339d4194cc877faf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429472"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="163bb-103">更新 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="163bb-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="163bb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="163bb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="163bb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="163bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="163bb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="163bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="163bb-107">更新[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="163bb-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="163bb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="163bb-108">Prerequisites</span></span>
<span data-ttu-id="163bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="163bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="163bb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="163bb-111">Permission type</span></span>|<span data-ttu-id="163bb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="163bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="163bb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="163bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="163bb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="163bb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="163bb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="163bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="163bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="163bb-116">Not supported.</span></span>|
|<span data-ttu-id="163bb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="163bb-117">Application</span></span>|<span data-ttu-id="163bb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="163bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="163bb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="163bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="163bb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="163bb-120">Request headers</span></span>
|<span data-ttu-id="163bb-121">标头</span><span class="sxs-lookup"><span data-stu-id="163bb-121">Header</span></span>|<span data-ttu-id="163bb-122">值</span><span class="sxs-lookup"><span data-stu-id="163bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="163bb-123">授权</span><span class="sxs-lookup"><span data-stu-id="163bb-123">Authorization</span></span>|<span data-ttu-id="163bb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="163bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="163bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="163bb-125">Accept</span></span>|<span data-ttu-id="163bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="163bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="163bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="163bb-127">Request body</span></span>
<span data-ttu-id="163bb-128">在请求正文中，提供[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="163bb-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="163bb-129">下表显示时创建[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="163bb-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="163bb-130">属性</span><span class="sxs-lookup"><span data-stu-id="163bb-130">Property</span></span>|<span data-ttu-id="163bb-131">类型</span><span class="sxs-lookup"><span data-stu-id="163bb-131">Type</span></span>|<span data-ttu-id="163bb-132">说明</span><span class="sxs-lookup"><span data-stu-id="163bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="163bb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="163bb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="163bb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="163bb-134">DateTimeOffset</span></span>|<span data-ttu-id="163bb-135">日期和时间上次修改对象。</span><span class="sxs-lookup"><span data-stu-id="163bb-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="163bb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="163bb-136">createdDateTime</span></span>|<span data-ttu-id="163bb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="163bb-137">DateTimeOffset</span></span>|<span data-ttu-id="163bb-138">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="163bb-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="163bb-139">id</span><span class="sxs-lookup"><span data-stu-id="163bb-139">id</span></span>|<span data-ttu-id="163bb-140">String</span><span class="sxs-lookup"><span data-stu-id="163bb-140">String</span></span>|<span data-ttu-id="163bb-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="163bb-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="163bb-142">响应</span><span class="sxs-lookup"><span data-stu-id="163bb-142">Response</span></span>
<span data-ttu-id="163bb-143">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="163bb-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="163bb-144">示例</span><span class="sxs-lookup"><span data-stu-id="163bb-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="163bb-145">请求</span><span class="sxs-lookup"><span data-stu-id="163bb-145">Request</span></span>
<span data-ttu-id="163bb-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="163bb-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="163bb-147">响应</span><span class="sxs-lookup"><span data-stu-id="163bb-147">Response</span></span>
<span data-ttu-id="163bb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="163bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




