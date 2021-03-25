---
title: 更新 groupPolicyUploadedCategory
description: 更新 groupPolicyUploadedCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 907df2881555cf651442bffd29c2cd98b0e25d0e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157015"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="53862-103">更新 groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="53862-103">Update groupPolicyUploadedCategory</span></span>

<span data-ttu-id="53862-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53862-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53862-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53862-107">更新 [groupPolicyUploadedCategory 对象](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="53862-107">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53862-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="53862-108">Prerequisites</span></span>
<span data-ttu-id="53862-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53862-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53862-111">Permission type</span></span>|<span data-ttu-id="53862-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53862-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53862-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53862-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53862-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53862-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53862-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53862-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53862-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53862-116">Not supported.</span></span>|
|<span data-ttu-id="53862-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53862-117">Application</span></span>|<span data-ttu-id="53862-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53862-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53862-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53862-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="53862-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53862-120">Request headers</span></span>
|<span data-ttu-id="53862-121">标头</span><span class="sxs-lookup"><span data-stu-id="53862-121">Header</span></span>|<span data-ttu-id="53862-122">值</span><span class="sxs-lookup"><span data-stu-id="53862-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53862-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53862-123">Authorization</span></span>|<span data-ttu-id="53862-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53862-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53862-125">接受</span><span class="sxs-lookup"><span data-stu-id="53862-125">Accept</span></span>|<span data-ttu-id="53862-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53862-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53862-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53862-127">Request body</span></span>
<span data-ttu-id="53862-128">在请求正文中，提供 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53862-128">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="53862-129">下表显示创建 [groupPolicyUploadedCategory 时所需的属性](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="53862-129">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="53862-130">属性</span><span class="sxs-lookup"><span data-stu-id="53862-130">Property</span></span>|<span data-ttu-id="53862-131">类型</span><span class="sxs-lookup"><span data-stu-id="53862-131">Type</span></span>|<span data-ttu-id="53862-132">说明</span><span class="sxs-lookup"><span data-stu-id="53862-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53862-133">displayName</span><span class="sxs-lookup"><span data-stu-id="53862-133">displayName</span></span>|<span data-ttu-id="53862-134">String</span><span class="sxs-lookup"><span data-stu-id="53862-134">String</span></span>|<span data-ttu-id="53862-135">类别名称的字符串 id 显示名称继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="53862-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="53862-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="53862-136">isRoot</span></span>|<span data-ttu-id="53862-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="53862-137">Boolean</span></span>|<span data-ttu-id="53862-138">定义类别是否属于根类别 继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="53862-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="53862-139">id</span><span class="sxs-lookup"><span data-stu-id="53862-139">id</span></span>|<span data-ttu-id="53862-140">String</span><span class="sxs-lookup"><span data-stu-id="53862-140">String</span></span>|<span data-ttu-id="53862-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="53862-141">Key of the entity.</span></span> <span data-ttu-id="53862-142">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="53862-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="53862-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53862-143">lastModifiedDateTime</span></span>|<span data-ttu-id="53862-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53862-144">DateTimeOffset</span></span>|<span data-ttu-id="53862-145">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="53862-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="53862-146">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="53862-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="53862-147">响应</span><span class="sxs-lookup"><span data-stu-id="53862-147">Response</span></span>
<span data-ttu-id="53862-148">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53862-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53862-149">示例</span><span class="sxs-lookup"><span data-stu-id="53862-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="53862-150">请求</span><span class="sxs-lookup"><span data-stu-id="53862-150">Request</span></span>
<span data-ttu-id="53862-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53862-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53862-152">响应</span><span class="sxs-lookup"><span data-stu-id="53862-152">Response</span></span>
<span data-ttu-id="53862-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53862-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




