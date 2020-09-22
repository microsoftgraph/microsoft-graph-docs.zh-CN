---
title: 更新 groupPolicyPresentation
description: 更新 groupPolicyPresentation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e18c2e2cbc7669f82d43dd4ac01676f2630b5382
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043253"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="db6b4-103">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="db6b4-103">Update groupPolicyPresentation</span></span>

<span data-ttu-id="db6b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db6b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db6b4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db6b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db6b4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db6b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db6b4-107">更新 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="db6b4-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db6b4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="db6b4-108">Prerequisites</span></span>
<span data-ttu-id="db6b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db6b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db6b4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="db6b4-111">Permission type</span></span>|<span data-ttu-id="db6b4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db6b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db6b4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db6b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db6b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db6b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db6b4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db6b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db6b4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db6b4-116">Not supported.</span></span>|
|<span data-ttu-id="db6b4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="db6b4-117">Application</span></span>|<span data-ttu-id="db6b4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db6b4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db6b4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db6b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="db6b4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db6b4-120">Request headers</span></span>
|<span data-ttu-id="db6b4-121">标头</span><span class="sxs-lookup"><span data-stu-id="db6b4-121">Header</span></span>|<span data-ttu-id="db6b4-122">值</span><span class="sxs-lookup"><span data-stu-id="db6b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db6b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db6b4-123">Authorization</span></span>|<span data-ttu-id="db6b4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db6b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db6b4-125">接受</span><span class="sxs-lookup"><span data-stu-id="db6b4-125">Accept</span></span>|<span data-ttu-id="db6b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db6b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db6b4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="db6b4-127">Request body</span></span>
<span data-ttu-id="db6b4-128">在请求正文中，提供 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db6b4-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="db6b4-129">下表显示创建 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db6b4-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="db6b4-130">属性</span><span class="sxs-lookup"><span data-stu-id="db6b4-130">Property</span></span>|<span data-ttu-id="db6b4-131">类型</span><span class="sxs-lookup"><span data-stu-id="db6b4-131">Type</span></span>|<span data-ttu-id="db6b4-132">说明</span><span class="sxs-lookup"><span data-stu-id="db6b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db6b4-133">label</span><span class="sxs-lookup"><span data-stu-id="db6b4-133">label</span></span>|<span data-ttu-id="db6b4-134">String</span><span class="sxs-lookup"><span data-stu-id="db6b4-134">String</span></span>|<span data-ttu-id="db6b4-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="db6b4-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="db6b4-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="db6b4-136">The default value is empty.</span></span>|
|<span data-ttu-id="db6b4-137">id</span><span class="sxs-lookup"><span data-stu-id="db6b4-137">id</span></span>|<span data-ttu-id="db6b4-138">String</span><span class="sxs-lookup"><span data-stu-id="db6b4-138">String</span></span>|<span data-ttu-id="db6b4-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db6b4-139">Key of the entity.</span></span>|
|<span data-ttu-id="db6b4-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db6b4-140">lastModifiedDateTime</span></span>|<span data-ttu-id="db6b4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db6b4-141">DateTimeOffset</span></span>|<span data-ttu-id="db6b4-142">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="db6b4-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="db6b4-143">响应</span><span class="sxs-lookup"><span data-stu-id="db6b4-143">Response</span></span>
<span data-ttu-id="db6b4-144">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db6b4-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db6b4-145">示例</span><span class="sxs-lookup"><span data-stu-id="db6b4-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="db6b4-146">请求</span><span class="sxs-lookup"><span data-stu-id="db6b4-146">Request</span></span>
<span data-ttu-id="db6b4-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db6b4-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="db6b4-148">响应</span><span class="sxs-lookup"><span data-stu-id="db6b4-148">Response</span></span>
<span data-ttu-id="db6b4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db6b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






