---
title: 更新 groupPolicyUploadedCategory
description: 更新 groupPolicyUploadedCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03d6bdffff214ad7e095475adbd116644029a5bd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735405"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="fe968-103">更新 groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="fe968-103">Update groupPolicyUploadedCategory</span></span>

<span data-ttu-id="fe968-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe968-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe968-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe968-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe968-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe968-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe968-107">更新 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fe968-107">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe968-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe968-108">Prerequisites</span></span>
<span data-ttu-id="fe968-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe968-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe968-111">Permission type</span></span>|<span data-ttu-id="fe968-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe968-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe968-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe968-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe968-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe968-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe968-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe968-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe968-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe968-116">Not supported.</span></span>|
|<span data-ttu-id="fe968-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe968-117">Application</span></span>|<span data-ttu-id="fe968-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe968-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe968-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe968-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/parent
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children/{groupPolicyCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="fe968-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe968-120">Request headers</span></span>
|<span data-ttu-id="fe968-121">标头</span><span class="sxs-lookup"><span data-stu-id="fe968-121">Header</span></span>|<span data-ttu-id="fe968-122">值</span><span class="sxs-lookup"><span data-stu-id="fe968-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe968-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe968-123">Authorization</span></span>|<span data-ttu-id="fe968-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe968-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe968-125">接受</span><span class="sxs-lookup"><span data-stu-id="fe968-125">Accept</span></span>|<span data-ttu-id="fe968-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe968-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe968-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe968-127">Request body</span></span>
<span data-ttu-id="fe968-128">在请求正文中，提供 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe968-128">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="fe968-129">下表显示创建 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe968-129">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="fe968-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe968-130">Property</span></span>|<span data-ttu-id="fe968-131">类型</span><span class="sxs-lookup"><span data-stu-id="fe968-131">Type</span></span>|<span data-ttu-id="fe968-132">说明</span><span class="sxs-lookup"><span data-stu-id="fe968-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe968-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fe968-133">displayName</span></span>|<span data-ttu-id="fe968-134">String</span><span class="sxs-lookup"><span data-stu-id="fe968-134">String</span></span>|<span data-ttu-id="fe968-135">从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的类别的显示名称的字符串 id</span><span class="sxs-lookup"><span data-stu-id="fe968-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="fe968-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="fe968-136">isRoot</span></span>|<span data-ttu-id="fe968-137">布尔</span><span class="sxs-lookup"><span data-stu-id="fe968-137">Boolean</span></span>|<span data-ttu-id="fe968-138">定义类别是否是从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的根类别</span><span class="sxs-lookup"><span data-stu-id="fe968-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="fe968-139">id</span><span class="sxs-lookup"><span data-stu-id="fe968-139">id</span></span>|<span data-ttu-id="fe968-140">String</span><span class="sxs-lookup"><span data-stu-id="fe968-140">String</span></span>|<span data-ttu-id="fe968-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fe968-141">Key of the entity.</span></span> <span data-ttu-id="fe968-142">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="fe968-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="fe968-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe968-143">lastModifiedDateTime</span></span>|<span data-ttu-id="fe968-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe968-144">DateTimeOffset</span></span>|<span data-ttu-id="fe968-145">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fe968-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="fe968-146">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="fe968-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fe968-147">响应</span><span class="sxs-lookup"><span data-stu-id="fe968-147">Response</span></span>
<span data-ttu-id="fe968-148">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe968-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe968-149">示例</span><span class="sxs-lookup"><span data-stu-id="fe968-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe968-150">请求</span><span class="sxs-lookup"><span data-stu-id="fe968-150">Request</span></span>
<span data-ttu-id="fe968-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe968-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="fe968-152">响应</span><span class="sxs-lookup"><span data-stu-id="fe968-152">Response</span></span>
<span data-ttu-id="fe968-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe968-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true,
  "id": "7e373e80-3e80-7e37-803e-377e803e377e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





