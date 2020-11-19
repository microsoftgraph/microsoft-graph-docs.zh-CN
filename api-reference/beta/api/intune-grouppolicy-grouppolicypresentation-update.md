---
title: 更新 groupPolicyPresentation
description: 更新 groupPolicyPresentation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38b80f055369354e4e73c74a44220940999142f9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212136"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="10355-103">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="10355-103">Update groupPolicyPresentation</span></span>

<span data-ttu-id="10355-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10355-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10355-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10355-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10355-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10355-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10355-107">更新 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10355-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10355-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="10355-108">Prerequisites</span></span>
<span data-ttu-id="10355-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10355-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10355-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="10355-111">Permission type</span></span>|<span data-ttu-id="10355-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10355-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10355-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10355-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10355-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10355-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10355-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10355-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10355-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10355-116">Not supported.</span></span>|
|<span data-ttu-id="10355-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="10355-117">Application</span></span>|<span data-ttu-id="10355-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10355-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10355-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10355-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="10355-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="10355-120">Request headers</span></span>
|<span data-ttu-id="10355-121">标头</span><span class="sxs-lookup"><span data-stu-id="10355-121">Header</span></span>|<span data-ttu-id="10355-122">值</span><span class="sxs-lookup"><span data-stu-id="10355-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10355-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10355-123">Authorization</span></span>|<span data-ttu-id="10355-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10355-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10355-125">接受</span><span class="sxs-lookup"><span data-stu-id="10355-125">Accept</span></span>|<span data-ttu-id="10355-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10355-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10355-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10355-127">Request body</span></span>
<span data-ttu-id="10355-128">在请求正文中，提供 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10355-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="10355-129">下表显示创建 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="10355-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="10355-130">属性</span><span class="sxs-lookup"><span data-stu-id="10355-130">Property</span></span>|<span data-ttu-id="10355-131">类型</span><span class="sxs-lookup"><span data-stu-id="10355-131">Type</span></span>|<span data-ttu-id="10355-132">说明</span><span class="sxs-lookup"><span data-stu-id="10355-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10355-133">label</span><span class="sxs-lookup"><span data-stu-id="10355-133">label</span></span>|<span data-ttu-id="10355-134">String</span><span class="sxs-lookup"><span data-stu-id="10355-134">String</span></span>|<span data-ttu-id="10355-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="10355-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="10355-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="10355-136">The default value is empty.</span></span>|
|<span data-ttu-id="10355-137">id</span><span class="sxs-lookup"><span data-stu-id="10355-137">id</span></span>|<span data-ttu-id="10355-138">String</span><span class="sxs-lookup"><span data-stu-id="10355-138">String</span></span>|<span data-ttu-id="10355-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="10355-139">Key of the entity.</span></span>|
|<span data-ttu-id="10355-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10355-140">lastModifiedDateTime</span></span>|<span data-ttu-id="10355-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10355-141">DateTimeOffset</span></span>|<span data-ttu-id="10355-142">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="10355-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="10355-143">响应</span><span class="sxs-lookup"><span data-stu-id="10355-143">Response</span></span>
<span data-ttu-id="10355-144">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10355-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10355-145">示例</span><span class="sxs-lookup"><span data-stu-id="10355-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="10355-146">请求</span><span class="sxs-lookup"><span data-stu-id="10355-146">Request</span></span>
<span data-ttu-id="10355-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10355-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="10355-148">响应</span><span class="sxs-lookup"><span data-stu-id="10355-148">Response</span></span>
<span data-ttu-id="10355-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10355-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




