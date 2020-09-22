---
title: 更新 groupPolicyUploadedCategory
description: 更新 groupPolicyUploadedCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 173daedb6a7ce03ff4417f04d3d9357db18ad831
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974252"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="52ef3-103">更新 groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="52ef3-103">Update groupPolicyUploadedCategory</span></span>

<span data-ttu-id="52ef3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52ef3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52ef3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="52ef3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52ef3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="52ef3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52ef3-107">更新 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="52ef3-107">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52ef3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="52ef3-108">Prerequisites</span></span>
<span data-ttu-id="52ef3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52ef3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="52ef3-111">Permission type</span></span>|<span data-ttu-id="52ef3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="52ef3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52ef3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52ef3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52ef3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52ef3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52ef3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52ef3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52ef3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52ef3-116">Not supported.</span></span>|
|<span data-ttu-id="52ef3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="52ef3-117">Application</span></span>|<span data-ttu-id="52ef3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52ef3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52ef3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52ef3-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="52ef3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="52ef3-120">Request headers</span></span>
|<span data-ttu-id="52ef3-121">标头</span><span class="sxs-lookup"><span data-stu-id="52ef3-121">Header</span></span>|<span data-ttu-id="52ef3-122">值</span><span class="sxs-lookup"><span data-stu-id="52ef3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52ef3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52ef3-123">Authorization</span></span>|<span data-ttu-id="52ef3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="52ef3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52ef3-125">接受</span><span class="sxs-lookup"><span data-stu-id="52ef3-125">Accept</span></span>|<span data-ttu-id="52ef3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52ef3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52ef3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="52ef3-127">Request body</span></span>
<span data-ttu-id="52ef3-128">在请求正文中，提供 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52ef3-128">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="52ef3-129">下表显示创建 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="52ef3-129">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="52ef3-130">属性</span><span class="sxs-lookup"><span data-stu-id="52ef3-130">Property</span></span>|<span data-ttu-id="52ef3-131">类型</span><span class="sxs-lookup"><span data-stu-id="52ef3-131">Type</span></span>|<span data-ttu-id="52ef3-132">说明</span><span class="sxs-lookup"><span data-stu-id="52ef3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52ef3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="52ef3-133">displayName</span></span>|<span data-ttu-id="52ef3-134">String</span><span class="sxs-lookup"><span data-stu-id="52ef3-134">String</span></span>|<span data-ttu-id="52ef3-135">从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的类别的显示名称的字符串 id</span><span class="sxs-lookup"><span data-stu-id="52ef3-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="52ef3-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="52ef3-136">isRoot</span></span>|<span data-ttu-id="52ef3-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="52ef3-137">Boolean</span></span>|<span data-ttu-id="52ef3-138">定义类别是否是从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的根类别</span><span class="sxs-lookup"><span data-stu-id="52ef3-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="52ef3-139">id</span><span class="sxs-lookup"><span data-stu-id="52ef3-139">id</span></span>|<span data-ttu-id="52ef3-140">String</span><span class="sxs-lookup"><span data-stu-id="52ef3-140">String</span></span>|<span data-ttu-id="52ef3-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="52ef3-141">Key of the entity.</span></span> <span data-ttu-id="52ef3-142">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="52ef3-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="52ef3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52ef3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="52ef3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52ef3-144">DateTimeOffset</span></span>|<span data-ttu-id="52ef3-145">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="52ef3-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="52ef3-146">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="52ef3-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="52ef3-147">响应</span><span class="sxs-lookup"><span data-stu-id="52ef3-147">Response</span></span>
<span data-ttu-id="52ef3-148">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52ef3-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52ef3-149">示例</span><span class="sxs-lookup"><span data-stu-id="52ef3-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="52ef3-150">请求</span><span class="sxs-lookup"><span data-stu-id="52ef3-150">Request</span></span>
<span data-ttu-id="52ef3-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52ef3-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52ef3-152">响应</span><span class="sxs-lookup"><span data-stu-id="52ef3-152">Response</span></span>
<span data-ttu-id="52ef3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52ef3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






