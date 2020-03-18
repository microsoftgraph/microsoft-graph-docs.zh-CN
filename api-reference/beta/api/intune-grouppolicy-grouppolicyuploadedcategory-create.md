---
title: 创建 groupPolicyUploadedCategory
description: 创建新的 groupPolicyUploadedCategory 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c85e0db90d7015182d90aac060048cea4042242
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803797"
---
# <a name="create-grouppolicyuploadedcategory"></a><span data-ttu-id="28cbb-103">创建 groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="28cbb-103">Create groupPolicyUploadedCategory</span></span>

> <span data-ttu-id="28cbb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28cbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28cbb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28cbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28cbb-106">创建新的[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28cbb-106">Create a new [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28cbb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="28cbb-107">Prerequisites</span></span>
<span data-ttu-id="28cbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28cbb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28cbb-110">Permission type</span></span>|<span data-ttu-id="28cbb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="28cbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28cbb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28cbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28cbb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28cbb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="28cbb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28cbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28cbb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28cbb-115">Not supported.</span></span>|
|<span data-ttu-id="28cbb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28cbb-116">Application</span></span>|<span data-ttu-id="28cbb-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28cbb-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28cbb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28cbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyCategories
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children
```

## <a name="request-headers"></a><span data-ttu-id="28cbb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="28cbb-119">Request headers</span></span>
|<span data-ttu-id="28cbb-120">标头</span><span class="sxs-lookup"><span data-stu-id="28cbb-120">Header</span></span>|<span data-ttu-id="28cbb-121">值</span><span class="sxs-lookup"><span data-stu-id="28cbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28cbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28cbb-122">Authorization</span></span>|<span data-ttu-id="28cbb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="28cbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28cbb-124">接受</span><span class="sxs-lookup"><span data-stu-id="28cbb-124">Accept</span></span>|<span data-ttu-id="28cbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28cbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28cbb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28cbb-126">Request body</span></span>
<span data-ttu-id="28cbb-127">在请求正文中，提供 groupPolicyUploadedCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28cbb-127">In the request body, supply a JSON representation for the groupPolicyUploadedCategory object.</span></span>

<span data-ttu-id="28cbb-128">下表显示创建 groupPolicyUploadedCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28cbb-128">The following table shows the properties that are required when you create the groupPolicyUploadedCategory.</span></span>

|<span data-ttu-id="28cbb-129">属性</span><span class="sxs-lookup"><span data-stu-id="28cbb-129">Property</span></span>|<span data-ttu-id="28cbb-130">类型</span><span class="sxs-lookup"><span data-stu-id="28cbb-130">Type</span></span>|<span data-ttu-id="28cbb-131">说明</span><span class="sxs-lookup"><span data-stu-id="28cbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28cbb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="28cbb-132">displayName</span></span>|<span data-ttu-id="28cbb-133">String</span><span class="sxs-lookup"><span data-stu-id="28cbb-133">String</span></span>|<span data-ttu-id="28cbb-134">从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的类别的显示名称的字符串 id</span><span class="sxs-lookup"><span data-stu-id="28cbb-134">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="28cbb-135">isRoot</span><span class="sxs-lookup"><span data-stu-id="28cbb-135">isRoot</span></span>|<span data-ttu-id="28cbb-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="28cbb-136">Boolean</span></span>|<span data-ttu-id="28cbb-137">定义类别是否是从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的根类别</span><span class="sxs-lookup"><span data-stu-id="28cbb-137">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="28cbb-138">id</span><span class="sxs-lookup"><span data-stu-id="28cbb-138">id</span></span>|<span data-ttu-id="28cbb-139">String</span><span class="sxs-lookup"><span data-stu-id="28cbb-139">String</span></span>|<span data-ttu-id="28cbb-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="28cbb-140">Key of the entity.</span></span> <span data-ttu-id="28cbb-141">继承自[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="28cbb-141">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="28cbb-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28cbb-142">lastModifiedDateTime</span></span>|<span data-ttu-id="28cbb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28cbb-143">DateTimeOffset</span></span>|<span data-ttu-id="28cbb-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="28cbb-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="28cbb-145">继承自[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="28cbb-145">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="28cbb-146">响应</span><span class="sxs-lookup"><span data-stu-id="28cbb-146">Response</span></span>
<span data-ttu-id="28cbb-147">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28cbb-147">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28cbb-148">示例</span><span class="sxs-lookup"><span data-stu-id="28cbb-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="28cbb-149">请求</span><span class="sxs-lookup"><span data-stu-id="28cbb-149">Request</span></span>
<span data-ttu-id="28cbb-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28cbb-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="28cbb-151">响应</span><span class="sxs-lookup"><span data-stu-id="28cbb-151">Response</span></span>
<span data-ttu-id="28cbb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28cbb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




