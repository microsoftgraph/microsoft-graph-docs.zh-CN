---
title: 创建 groupPolicyUploadedCategory
description: 创建新的 groupPolicyUploadedCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7996f9e28deeefd2dcac04d3496dc67a216708e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157085"
---
# <a name="create-grouppolicyuploadedcategory"></a><span data-ttu-id="a4a9f-103">创建 groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="a4a9f-103">Create groupPolicyUploadedCategory</span></span>

<span data-ttu-id="a4a9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4a9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4a9f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4a9f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4a9f-107">创建新的 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-107">Create a new [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4a9f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4a9f-108">Prerequisites</span></span>
<span data-ttu-id="a4a9f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4a9f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4a9f-111">Permission type</span></span>|<span data-ttu-id="a4a9f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4a9f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4a9f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4a9f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4a9f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a9f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4a9f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4a9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4a9f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-116">Not supported.</span></span>|
|<span data-ttu-id="a4a9f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4a9f-117">Application</span></span>|<span data-ttu-id="a4a9f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a9f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4a9f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4a9f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyCategories
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children
```

## <a name="request-headers"></a><span data-ttu-id="a4a9f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4a9f-120">Request headers</span></span>
|<span data-ttu-id="a4a9f-121">标头</span><span class="sxs-lookup"><span data-stu-id="a4a9f-121">Header</span></span>|<span data-ttu-id="a4a9f-122">值</span><span class="sxs-lookup"><span data-stu-id="a4a9f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4a9f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a9f-123">Authorization</span></span>|<span data-ttu-id="a4a9f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4a9f-125">接受</span><span class="sxs-lookup"><span data-stu-id="a4a9f-125">Accept</span></span>|<span data-ttu-id="a4a9f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4a9f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4a9f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4a9f-127">Request body</span></span>
<span data-ttu-id="a4a9f-128">在请求正文中，提供 groupPolicyUploadedCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-128">In the request body, supply a JSON representation for the groupPolicyUploadedCategory object.</span></span>

<span data-ttu-id="a4a9f-129">下表显示创建 groupPolicyUploadedCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-129">The following table shows the properties that are required when you create the groupPolicyUploadedCategory.</span></span>

|<span data-ttu-id="a4a9f-130">属性</span><span class="sxs-lookup"><span data-stu-id="a4a9f-130">Property</span></span>|<span data-ttu-id="a4a9f-131">类型</span><span class="sxs-lookup"><span data-stu-id="a4a9f-131">Type</span></span>|<span data-ttu-id="a4a9f-132">说明</span><span class="sxs-lookup"><span data-stu-id="a4a9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4a9f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a4a9f-133">displayName</span></span>|<span data-ttu-id="a4a9f-134">String</span><span class="sxs-lookup"><span data-stu-id="a4a9f-134">String</span></span>|<span data-ttu-id="a4a9f-135">类别名称的字符串 id 显示名称继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="a4a9f-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="a4a9f-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="a4a9f-136">isRoot</span></span>|<span data-ttu-id="a4a9f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4a9f-137">Boolean</span></span>|<span data-ttu-id="a4a9f-138">定义类别是否属于根类别 继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="a4a9f-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="a4a9f-139">id</span><span class="sxs-lookup"><span data-stu-id="a4a9f-139">id</span></span>|<span data-ttu-id="a4a9f-140">String</span><span class="sxs-lookup"><span data-stu-id="a4a9f-140">String</span></span>|<span data-ttu-id="a4a9f-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-141">Key of the entity.</span></span> <span data-ttu-id="a4a9f-142">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="a4a9f-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="a4a9f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4a9f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="a4a9f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4a9f-144">DateTimeOffset</span></span>|<span data-ttu-id="a4a9f-145">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="a4a9f-146">继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="a4a9f-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a4a9f-147">响应</span><span class="sxs-lookup"><span data-stu-id="a4a9f-147">Response</span></span>
<span data-ttu-id="a4a9f-148">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-148">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a9f-149">示例</span><span class="sxs-lookup"><span data-stu-id="a4a9f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4a9f-150">请求</span><span class="sxs-lookup"><span data-stu-id="a4a9f-150">Request</span></span>
<span data-ttu-id="a4a9f-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4a9f-152">响应</span><span class="sxs-lookup"><span data-stu-id="a4a9f-152">Response</span></span>
<span data-ttu-id="a4a9f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4a9f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




