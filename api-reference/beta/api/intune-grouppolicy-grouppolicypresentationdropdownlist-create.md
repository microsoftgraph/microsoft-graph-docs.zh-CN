---
title: 创建 groupPolicyPresentationDropdownList
description: 创建新的 groupPolicyPresentationDropdownList 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7b36416d280bd3234b51203bf8e99d824a16934
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904872"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="0b7a9-103">创建 groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="0b7a9-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="0b7a9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b7a9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b7a9-106">创建新的[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-106">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b7a9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b7a9-107">Prerequisites</span></span>
<span data-ttu-id="0b7a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b7a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b7a9-110">Permission type</span></span>|<span data-ttu-id="0b7a9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b7a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b7a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b7a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b7a9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b7a9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0b7a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b7a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b7a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-115">Not supported.</span></span>|
|<span data-ttu-id="0b7a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b7a9-116">Application</span></span>|<span data-ttu-id="0b7a9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b7a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b7a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="0b7a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b7a9-119">Request headers</span></span>
|<span data-ttu-id="0b7a9-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b7a9-120">Header</span></span>|<span data-ttu-id="0b7a9-121">值</span><span class="sxs-lookup"><span data-stu-id="0b7a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b7a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b7a9-122">Authorization</span></span>|<span data-ttu-id="0b7a9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b7a9-124">接受</span><span class="sxs-lookup"><span data-stu-id="0b7a9-124">Accept</span></span>|<span data-ttu-id="0b7a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b7a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b7a9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b7a9-126">Request body</span></span>
<span data-ttu-id="0b7a9-127">在请求正文中, 提供 groupPolicyPresentationDropdownList 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-127">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="0b7a9-128">下表显示创建 groupPolicyPresentationDropdownList 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-128">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="0b7a9-129">属性</span><span class="sxs-lookup"><span data-stu-id="0b7a9-129">Property</span></span>|<span data-ttu-id="0b7a9-130">类型</span><span class="sxs-lookup"><span data-stu-id="0b7a9-130">Type</span></span>|<span data-ttu-id="0b7a9-131">说明</span><span class="sxs-lookup"><span data-stu-id="0b7a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b7a9-132">label</span><span class="sxs-lookup"><span data-stu-id="0b7a9-132">label</span></span>|<span data-ttu-id="0b7a9-133">String</span><span class="sxs-lookup"><span data-stu-id="0b7a9-133">String</span></span>|<span data-ttu-id="0b7a9-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="0b7a9-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-135">The default value is empty.</span></span> <span data-ttu-id="0b7a9-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="0b7a9-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0b7a9-137">id</span><span class="sxs-lookup"><span data-stu-id="0b7a9-137">id</span></span>|<span data-ttu-id="0b7a9-138">String</span><span class="sxs-lookup"><span data-stu-id="0b7a9-138">String</span></span>|<span data-ttu-id="0b7a9-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-139">Key of the entity.</span></span> <span data-ttu-id="0b7a9-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="0b7a9-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0b7a9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b7a9-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0b7a9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b7a9-142">DateTimeOffset</span></span>|<span data-ttu-id="0b7a9-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="0b7a9-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="0b7a9-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0b7a9-145">defaultItem</span><span class="sxs-lookup"><span data-stu-id="0b7a9-145">defaultItem</span></span>|[<span data-ttu-id="0b7a9-146">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="0b7a9-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="0b7a9-147">用于标识项目列表的默认选择的本地化字符串值。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="0b7a9-148">items</span><span class="sxs-lookup"><span data-stu-id="0b7a9-148">items</span></span>|<span data-ttu-id="0b7a9-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b7a9-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="0b7a9-150">表示一组本地化的显示名称及其关联的值。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="0b7a9-151">必需</span><span class="sxs-lookup"><span data-stu-id="0b7a9-151">required</span></span>|<span data-ttu-id="0b7a9-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7a9-152">Boolean</span></span>|<span data-ttu-id="0b7a9-153">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="0b7a9-154">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="0b7a9-155">响应</span><span class="sxs-lookup"><span data-stu-id="0b7a9-155">Response</span></span>
<span data-ttu-id="0b7a9-156">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-156">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b7a9-157">示例</span><span class="sxs-lookup"><span data-stu-id="0b7a9-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b7a9-158">请求</span><span class="sxs-lookup"><span data-stu-id="0b7a9-158">Request</span></span>
<span data-ttu-id="0b7a9-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="0b7a9-160">响应</span><span class="sxs-lookup"><span data-stu-id="0b7a9-160">Response</span></span>
<span data-ttu-id="0b7a9-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b7a9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




