---
title: 更新 groupPolicyPresentationValue
description: 更新 groupPolicyPresentationValue 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec32917726d4816796716cfd9c92430d1a306bf8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050428"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="a9ac0-103">更新 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="a9ac0-103">Update groupPolicyPresentationValue</span></span>

<span data-ttu-id="a9ac0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9ac0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9ac0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9ac0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9ac0-107">更新 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9ac0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9ac0-108">Prerequisites</span></span>
<span data-ttu-id="a9ac0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9ac0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9ac0-111">Permission type</span></span>|<span data-ttu-id="a9ac0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9ac0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9ac0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9ac0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9ac0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9ac0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9ac0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9ac0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9ac0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-116">Not supported.</span></span>|
|<span data-ttu-id="a9ac0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9ac0-117">Application</span></span>|<span data-ttu-id="a9ac0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9ac0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9ac0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9ac0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="a9ac0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9ac0-120">Request headers</span></span>
|<span data-ttu-id="a9ac0-121">标头</span><span class="sxs-lookup"><span data-stu-id="a9ac0-121">Header</span></span>|<span data-ttu-id="a9ac0-122">值</span><span class="sxs-lookup"><span data-stu-id="a9ac0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9ac0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9ac0-123">Authorization</span></span>|<span data-ttu-id="a9ac0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9ac0-125">接受</span><span class="sxs-lookup"><span data-stu-id="a9ac0-125">Accept</span></span>|<span data-ttu-id="a9ac0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9ac0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9ac0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9ac0-127">Request body</span></span>
<span data-ttu-id="a9ac0-128">在请求正文中，提供 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="a9ac0-129">下表显示创建 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="a9ac0-130">属性</span><span class="sxs-lookup"><span data-stu-id="a9ac0-130">Property</span></span>|<span data-ttu-id="a9ac0-131">类型</span><span class="sxs-lookup"><span data-stu-id="a9ac0-131">Type</span></span>|<span data-ttu-id="a9ac0-132">说明</span><span class="sxs-lookup"><span data-stu-id="a9ac0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9ac0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9ac0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a9ac0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9ac0-134">DateTimeOffset</span></span>|<span data-ttu-id="a9ac0-135">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="a9ac0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9ac0-136">createdDateTime</span></span>|<span data-ttu-id="a9ac0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9ac0-137">DateTimeOffset</span></span>|<span data-ttu-id="a9ac0-138">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="a9ac0-139">id</span><span class="sxs-lookup"><span data-stu-id="a9ac0-139">id</span></span>|<span data-ttu-id="a9ac0-140">String</span><span class="sxs-lookup"><span data-stu-id="a9ac0-140">String</span></span>|<span data-ttu-id="a9ac0-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a9ac0-142">响应</span><span class="sxs-lookup"><span data-stu-id="a9ac0-142">Response</span></span>
<span data-ttu-id="a9ac0-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9ac0-144">示例</span><span class="sxs-lookup"><span data-stu-id="a9ac0-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9ac0-145">请求</span><span class="sxs-lookup"><span data-stu-id="a9ac0-145">Request</span></span>
<span data-ttu-id="a9ac0-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="a9ac0-147">响应</span><span class="sxs-lookup"><span data-stu-id="a9ac0-147">Response</span></span>
<span data-ttu-id="a9ac0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9ac0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






