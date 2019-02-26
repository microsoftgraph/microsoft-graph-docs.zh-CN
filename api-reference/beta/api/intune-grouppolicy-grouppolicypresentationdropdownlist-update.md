---
title: 更新 groupPolicyPresentationDropdownList
description: 更新 groupPolicyPresentationDropdownList 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eea975cca630cdc3af99a4a8c737c91d7c64fe0d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162830"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="db09c-103">更新 groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="db09c-103">Update groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="db09c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db09c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db09c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db09c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db09c-106">更新[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="db09c-106">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db09c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="db09c-107">Prerequisites</span></span>
<span data-ttu-id="db09c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="db09c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="db09c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db09c-110">Permission type</span></span>|<span data-ttu-id="db09c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db09c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db09c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db09c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db09c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db09c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db09c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db09c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db09c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db09c-115">Not supported.</span></span>|
|<span data-ttu-id="db09c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db09c-116">Application</span></span>|<span data-ttu-id="db09c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db09c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db09c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db09c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="db09c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db09c-119">Request headers</span></span>
|<span data-ttu-id="db09c-120">标头</span><span class="sxs-lookup"><span data-stu-id="db09c-120">Header</span></span>|<span data-ttu-id="db09c-121">值</span><span class="sxs-lookup"><span data-stu-id="db09c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db09c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db09c-122">Authorization</span></span>|<span data-ttu-id="db09c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db09c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db09c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="db09c-124">Accept</span></span>|<span data-ttu-id="db09c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db09c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db09c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db09c-126">Request body</span></span>
<span data-ttu-id="db09c-127">在请求正文中, 提供[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db09c-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="db09c-128">下表显示创建[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db09c-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="db09c-129">属性</span><span class="sxs-lookup"><span data-stu-id="db09c-129">Property</span></span>|<span data-ttu-id="db09c-130">类型</span><span class="sxs-lookup"><span data-stu-id="db09c-130">Type</span></span>|<span data-ttu-id="db09c-131">说明</span><span class="sxs-lookup"><span data-stu-id="db09c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db09c-132">标签</span><span class="sxs-lookup"><span data-stu-id="db09c-132">label</span></span>|<span data-ttu-id="db09c-133">String</span><span class="sxs-lookup"><span data-stu-id="db09c-133">String</span></span>|<span data-ttu-id="db09c-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="db09c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="db09c-135">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="db09c-135">The default value is empty.</span></span> <span data-ttu-id="db09c-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="db09c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="db09c-137">id</span><span class="sxs-lookup"><span data-stu-id="db09c-137">id</span></span>|<span data-ttu-id="db09c-138">String</span><span class="sxs-lookup"><span data-stu-id="db09c-138">String</span></span>|<span data-ttu-id="db09c-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db09c-139">Key of the entity.</span></span> <span data-ttu-id="db09c-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="db09c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="db09c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db09c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="db09c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db09c-142">DateTimeOffset</span></span>|<span data-ttu-id="db09c-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="db09c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="db09c-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="db09c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="db09c-145">defaultItem</span><span class="sxs-lookup"><span data-stu-id="db09c-145">defaultItem</span></span>|[<span data-ttu-id="db09c-146">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="db09c-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="db09c-147">用于标识项目列表的默认选择的本地化字符串值。</span><span class="sxs-lookup"><span data-stu-id="db09c-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="db09c-148">项目</span><span class="sxs-lookup"><span data-stu-id="db09c-148">items</span></span>|<span data-ttu-id="db09c-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="db09c-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="db09c-150">表示一组本地化的显示名称及其关联的值。</span><span class="sxs-lookup"><span data-stu-id="db09c-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="db09c-151">必需</span><span class="sxs-lookup"><span data-stu-id="db09c-151">required</span></span>|<span data-ttu-id="db09c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="db09c-152">Boolean</span></span>|<span data-ttu-id="db09c-153">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="db09c-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="db09c-154">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="db09c-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="db09c-155">响应</span><span class="sxs-lookup"><span data-stu-id="db09c-155">Response</span></span>
<span data-ttu-id="db09c-156">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="db09c-156">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db09c-157">示例</span><span class="sxs-lookup"><span data-stu-id="db09c-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="db09c-158">请求</span><span class="sxs-lookup"><span data-stu-id="db09c-158">Request</span></span>
<span data-ttu-id="db09c-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db09c-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```

### <a name="response"></a><span data-ttu-id="db09c-160">响应</span><span class="sxs-lookup"><span data-stu-id="db09c-160">Response</span></span>
<span data-ttu-id="db09c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db09c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```




