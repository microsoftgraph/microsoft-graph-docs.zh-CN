---
title: 更新 groupPolicyPresentation
description: 更新 groupPolicyPresentation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da0b72b6818672c005c76170264f6749e3fab9bb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142014"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="6e684-103">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="6e684-103">Update groupPolicyPresentation</span></span>

<span data-ttu-id="6e684-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e684-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e684-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e684-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e684-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e684-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e684-107">更新 [groupPolicyPresentation 对象](../resources/intune-grouppolicy-grouppolicypresentation.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6e684-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e684-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e684-108">Prerequisites</span></span>
<span data-ttu-id="6e684-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e684-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e684-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e684-111">Permission type</span></span>|<span data-ttu-id="6e684-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e684-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e684-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e684-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e684-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e684-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e684-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e684-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e684-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e684-116">Not supported.</span></span>|
|<span data-ttu-id="6e684-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e684-117">Application</span></span>|<span data-ttu-id="6e684-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e684-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e684-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e684-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="6e684-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e684-120">Request headers</span></span>
|<span data-ttu-id="6e684-121">标头</span><span class="sxs-lookup"><span data-stu-id="6e684-121">Header</span></span>|<span data-ttu-id="6e684-122">值</span><span class="sxs-lookup"><span data-stu-id="6e684-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e684-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e684-123">Authorization</span></span>|<span data-ttu-id="6e684-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e684-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e684-125">接受</span><span class="sxs-lookup"><span data-stu-id="6e684-125">Accept</span></span>|<span data-ttu-id="6e684-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e684-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e684-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e684-127">Request body</span></span>
<span data-ttu-id="6e684-128">在请求正文中，提供 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e684-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="6e684-129">下表显示创建 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6e684-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="6e684-130">属性</span><span class="sxs-lookup"><span data-stu-id="6e684-130">Property</span></span>|<span data-ttu-id="6e684-131">类型</span><span class="sxs-lookup"><span data-stu-id="6e684-131">Type</span></span>|<span data-ttu-id="6e684-132">说明</span><span class="sxs-lookup"><span data-stu-id="6e684-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e684-133">label</span><span class="sxs-lookup"><span data-stu-id="6e684-133">label</span></span>|<span data-ttu-id="6e684-134">String</span><span class="sxs-lookup"><span data-stu-id="6e684-134">String</span></span>|<span data-ttu-id="6e684-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="6e684-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6e684-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="6e684-136">The default value is empty.</span></span>|
|<span data-ttu-id="6e684-137">id</span><span class="sxs-lookup"><span data-stu-id="6e684-137">id</span></span>|<span data-ttu-id="6e684-138">String</span><span class="sxs-lookup"><span data-stu-id="6e684-138">String</span></span>|<span data-ttu-id="6e684-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6e684-139">Key of the entity.</span></span>|
|<span data-ttu-id="6e684-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e684-140">lastModifiedDateTime</span></span>|<span data-ttu-id="6e684-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e684-141">DateTimeOffset</span></span>|<span data-ttu-id="6e684-142">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6e684-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6e684-143">响应</span><span class="sxs-lookup"><span data-stu-id="6e684-143">Response</span></span>
<span data-ttu-id="6e684-144">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e684-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e684-145">示例</span><span class="sxs-lookup"><span data-stu-id="6e684-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e684-146">请求</span><span class="sxs-lookup"><span data-stu-id="6e684-146">Request</span></span>
<span data-ttu-id="6e684-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e684-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="6e684-148">响应</span><span class="sxs-lookup"><span data-stu-id="6e684-148">Response</span></span>
<span data-ttu-id="6e684-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e684-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




