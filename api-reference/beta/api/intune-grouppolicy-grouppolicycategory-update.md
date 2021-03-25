---
title: 更新 groupPolicyCategory
description: 更新 groupPolicyCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a70edcb1f05ceb19a7dbb7a65d2d4b501a724dc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153480"
---
# <a name="update-grouppolicycategory"></a><span data-ttu-id="735b1-103">更新 groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="735b1-103">Update groupPolicyCategory</span></span>

<span data-ttu-id="735b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="735b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="735b1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="735b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="735b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="735b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="735b1-107">更新 [groupPolicyCategory 对象](../resources/intune-grouppolicy-grouppolicycategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="735b1-107">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="735b1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="735b1-108">Prerequisites</span></span>
<span data-ttu-id="735b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="735b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="735b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="735b1-111">Permission type</span></span>|<span data-ttu-id="735b1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="735b1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="735b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="735b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="735b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="735b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="735b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="735b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="735b1-116">Not supported.</span></span>|
|<span data-ttu-id="735b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="735b1-117">Application</span></span>|<span data-ttu-id="735b1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735b1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="735b1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="735b1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="735b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="735b1-120">Request headers</span></span>
|<span data-ttu-id="735b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="735b1-121">Header</span></span>|<span data-ttu-id="735b1-122">值</span><span class="sxs-lookup"><span data-stu-id="735b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="735b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="735b1-123">Authorization</span></span>|<span data-ttu-id="735b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="735b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="735b1-125">接受</span><span class="sxs-lookup"><span data-stu-id="735b1-125">Accept</span></span>|<span data-ttu-id="735b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="735b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="735b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="735b1-127">Request body</span></span>
<span data-ttu-id="735b1-128">在请求正文中，提供 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="735b1-128">In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

<span data-ttu-id="735b1-129">下表显示创建 [groupPolicyCategory 时所需的属性](../resources/intune-grouppolicy-grouppolicycategory.md)。</span><span class="sxs-lookup"><span data-stu-id="735b1-129">The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span></span>

|<span data-ttu-id="735b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="735b1-130">Property</span></span>|<span data-ttu-id="735b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="735b1-131">Type</span></span>|<span data-ttu-id="735b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="735b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="735b1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="735b1-133">displayName</span></span>|<span data-ttu-id="735b1-134">String</span><span class="sxs-lookup"><span data-stu-id="735b1-134">String</span></span>|<span data-ttu-id="735b1-135">类别名称的字符串 id 显示名称</span><span class="sxs-lookup"><span data-stu-id="735b1-135">The string id of the category's display name</span></span>|
|<span data-ttu-id="735b1-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="735b1-136">isRoot</span></span>|<span data-ttu-id="735b1-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="735b1-137">Boolean</span></span>|<span data-ttu-id="735b1-138">定义类别是否属于根类别</span><span class="sxs-lookup"><span data-stu-id="735b1-138">Defines if the category is a root category</span></span>|
|<span data-ttu-id="735b1-139">id</span><span class="sxs-lookup"><span data-stu-id="735b1-139">id</span></span>|<span data-ttu-id="735b1-140">String</span><span class="sxs-lookup"><span data-stu-id="735b1-140">String</span></span>|<span data-ttu-id="735b1-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="735b1-141">Key of the entity.</span></span>|
|<span data-ttu-id="735b1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="735b1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="735b1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="735b1-143">DateTimeOffset</span></span>|<span data-ttu-id="735b1-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="735b1-144">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="735b1-145">响应</span><span class="sxs-lookup"><span data-stu-id="735b1-145">Response</span></span>
<span data-ttu-id="735b1-146">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="735b1-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="735b1-147">示例</span><span class="sxs-lookup"><span data-stu-id="735b1-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="735b1-148">请求</span><span class="sxs-lookup"><span data-stu-id="735b1-148">Request</span></span>
<span data-ttu-id="735b1-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="735b1-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="735b1-150">响应</span><span class="sxs-lookup"><span data-stu-id="735b1-150">Response</span></span>
<span data-ttu-id="735b1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="735b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true,
  "id": "d0641e36-1e36-d064-361e-64d0361e64d0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




