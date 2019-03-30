---
title: 更新 groupPolicyPresentation
description: 更新 groupPolicyPresentation 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44da489c3cdf124b434ba35d52d39d63dba54209
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986976"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="765db-103">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="765db-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="765db-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="765db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="765db-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="765db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="765db-106">更新[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="765db-106">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="765db-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="765db-107">Prerequisites</span></span>
<span data-ttu-id="765db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="765db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="765db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="765db-110">Permission type</span></span>|<span data-ttu-id="765db-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="765db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="765db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="765db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="765db-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="765db-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="765db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="765db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="765db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="765db-115">Not supported.</span></span>|
|<span data-ttu-id="765db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="765db-116">Application</span></span>|<span data-ttu-id="765db-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="765db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="765db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="765db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="765db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="765db-119">Request headers</span></span>
|<span data-ttu-id="765db-120">标头</span><span class="sxs-lookup"><span data-stu-id="765db-120">Header</span></span>|<span data-ttu-id="765db-121">值</span><span class="sxs-lookup"><span data-stu-id="765db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="765db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="765db-122">Authorization</span></span>|<span data-ttu-id="765db-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="765db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="765db-124">接受</span><span class="sxs-lookup"><span data-stu-id="765db-124">Accept</span></span>|<span data-ttu-id="765db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="765db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="765db-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="765db-126">Request body</span></span>
<span data-ttu-id="765db-127">在请求正文中, 提供[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="765db-127">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="765db-128">下表显示创建[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="765db-128">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="765db-129">属性</span><span class="sxs-lookup"><span data-stu-id="765db-129">Property</span></span>|<span data-ttu-id="765db-130">类型</span><span class="sxs-lookup"><span data-stu-id="765db-130">Type</span></span>|<span data-ttu-id="765db-131">说明</span><span class="sxs-lookup"><span data-stu-id="765db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="765db-132">label</span><span class="sxs-lookup"><span data-stu-id="765db-132">label</span></span>|<span data-ttu-id="765db-133">String</span><span class="sxs-lookup"><span data-stu-id="765db-133">String</span></span>|<span data-ttu-id="765db-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="765db-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="765db-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="765db-135">The default value is empty.</span></span>|
|<span data-ttu-id="765db-136">id</span><span class="sxs-lookup"><span data-stu-id="765db-136">id</span></span>|<span data-ttu-id="765db-137">String</span><span class="sxs-lookup"><span data-stu-id="765db-137">String</span></span>|<span data-ttu-id="765db-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="765db-138">Key of the entity.</span></span>|
|<span data-ttu-id="765db-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="765db-139">lastModifiedDateTime</span></span>|<span data-ttu-id="765db-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="765db-140">DateTimeOffset</span></span>|<span data-ttu-id="765db-141">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="765db-141">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="765db-142">响应</span><span class="sxs-lookup"><span data-stu-id="765db-142">Response</span></span>
<span data-ttu-id="765db-143">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="765db-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="765db-144">示例</span><span class="sxs-lookup"><span data-stu-id="765db-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="765db-145">请求</span><span class="sxs-lookup"><span data-stu-id="765db-145">Request</span></span>
<span data-ttu-id="765db-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="765db-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="765db-147">响应</span><span class="sxs-lookup"><span data-stu-id="765db-147">Response</span></span>
<span data-ttu-id="765db-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="765db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




