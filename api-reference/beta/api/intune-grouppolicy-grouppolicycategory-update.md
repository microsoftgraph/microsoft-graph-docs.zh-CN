---
title: 更新 groupPolicyCategory
description: 更新 groupPolicyCategory 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72aec785250fe38f8733964fcf140aacc95a09cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804525"
---
# <a name="update-grouppolicycategory"></a><span data-ttu-id="bddcb-103">更新 groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="bddcb-103">Update groupPolicyCategory</span></span>

> <span data-ttu-id="bddcb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bddcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bddcb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bddcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bddcb-106">更新[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bddcb-106">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bddcb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bddcb-107">Prerequisites</span></span>
<span data-ttu-id="bddcb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bddcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bddcb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bddcb-110">Permission type</span></span>|<span data-ttu-id="bddcb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bddcb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bddcb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bddcb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bddcb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bddcb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bddcb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bddcb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bddcb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bddcb-115">Not supported.</span></span>|
|<span data-ttu-id="bddcb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bddcb-116">Application</span></span>|<span data-ttu-id="bddcb-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bddcb-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bddcb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bddcb-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bddcb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bddcb-119">Request headers</span></span>
|<span data-ttu-id="bddcb-120">标头</span><span class="sxs-lookup"><span data-stu-id="bddcb-120">Header</span></span>|<span data-ttu-id="bddcb-121">值</span><span class="sxs-lookup"><span data-stu-id="bddcb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bddcb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bddcb-122">Authorization</span></span>|<span data-ttu-id="bddcb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bddcb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bddcb-124">接受</span><span class="sxs-lookup"><span data-stu-id="bddcb-124">Accept</span></span>|<span data-ttu-id="bddcb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bddcb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bddcb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bddcb-126">Request body</span></span>
<span data-ttu-id="bddcb-127">在请求正文中，提供[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bddcb-127">In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

<span data-ttu-id="bddcb-128">下表显示创建[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bddcb-128">The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span></span>

|<span data-ttu-id="bddcb-129">属性</span><span class="sxs-lookup"><span data-stu-id="bddcb-129">Property</span></span>|<span data-ttu-id="bddcb-130">类型</span><span class="sxs-lookup"><span data-stu-id="bddcb-130">Type</span></span>|<span data-ttu-id="bddcb-131">说明</span><span class="sxs-lookup"><span data-stu-id="bddcb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bddcb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bddcb-132">displayName</span></span>|<span data-ttu-id="bddcb-133">String</span><span class="sxs-lookup"><span data-stu-id="bddcb-133">String</span></span>|<span data-ttu-id="bddcb-134">类别的显示名称的字符串 id</span><span class="sxs-lookup"><span data-stu-id="bddcb-134">The string id of the category's display name</span></span>|
|<span data-ttu-id="bddcb-135">isRoot</span><span class="sxs-lookup"><span data-stu-id="bddcb-135">isRoot</span></span>|<span data-ttu-id="bddcb-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="bddcb-136">Boolean</span></span>|<span data-ttu-id="bddcb-137">定义类别是否为根类别</span><span class="sxs-lookup"><span data-stu-id="bddcb-137">Defines if the category is a root category</span></span>|
|<span data-ttu-id="bddcb-138">id</span><span class="sxs-lookup"><span data-stu-id="bddcb-138">id</span></span>|<span data-ttu-id="bddcb-139">String</span><span class="sxs-lookup"><span data-stu-id="bddcb-139">String</span></span>|<span data-ttu-id="bddcb-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bddcb-140">Key of the entity.</span></span>|
|<span data-ttu-id="bddcb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bddcb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bddcb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bddcb-142">DateTimeOffset</span></span>|<span data-ttu-id="bddcb-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bddcb-143">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bddcb-144">响应</span><span class="sxs-lookup"><span data-stu-id="bddcb-144">Response</span></span>
<span data-ttu-id="bddcb-145">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bddcb-145">If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bddcb-146">示例</span><span class="sxs-lookup"><span data-stu-id="bddcb-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="bddcb-147">请求</span><span class="sxs-lookup"><span data-stu-id="bddcb-147">Request</span></span>
<span data-ttu-id="bddcb-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bddcb-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bddcb-149">响应</span><span class="sxs-lookup"><span data-stu-id="bddcb-149">Response</span></span>
<span data-ttu-id="bddcb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bddcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




