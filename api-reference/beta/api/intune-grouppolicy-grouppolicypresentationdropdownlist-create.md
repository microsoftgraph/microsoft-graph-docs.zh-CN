---
title: 创建 groupPolicyPresentationDropdownList
description: 创建新的 groupPolicyPresentationDropdownList 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c332d7ede3da0c3f4faf50d49c2e24e6998027d8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942967"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="626f0-103">创建 groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="626f0-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="626f0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="626f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="626f0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="626f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="626f0-106">创建新的[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="626f0-106">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="626f0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="626f0-107">Prerequisites</span></span>
<span data-ttu-id="626f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="626f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626f0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="626f0-110">Permission type</span></span>|<span data-ttu-id="626f0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="626f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="626f0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="626f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="626f0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626f0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="626f0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="626f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="626f0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="626f0-115">Not supported.</span></span>|
|<span data-ttu-id="626f0-116">Application</span><span class="sxs-lookup"><span data-stu-id="626f0-116">Application</span></span>|<span data-ttu-id="626f0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626f0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="626f0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="626f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="626f0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="626f0-119">Request headers</span></span>
|<span data-ttu-id="626f0-120">标头</span><span class="sxs-lookup"><span data-stu-id="626f0-120">Header</span></span>|<span data-ttu-id="626f0-121">值</span><span class="sxs-lookup"><span data-stu-id="626f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="626f0-122">授权</span><span class="sxs-lookup"><span data-stu-id="626f0-122">Authorization</span></span>|<span data-ttu-id="626f0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="626f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="626f0-124">接受</span><span class="sxs-lookup"><span data-stu-id="626f0-124">Accept</span></span>|<span data-ttu-id="626f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="626f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="626f0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="626f0-126">Request body</span></span>
<span data-ttu-id="626f0-127">在请求正文中，提供 groupPolicyPresentationDropdownList 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="626f0-127">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="626f0-128">下表显示创建 groupPolicyPresentationDropdownList 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="626f0-128">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="626f0-129">属性</span><span class="sxs-lookup"><span data-stu-id="626f0-129">Property</span></span>|<span data-ttu-id="626f0-130">类型</span><span class="sxs-lookup"><span data-stu-id="626f0-130">Type</span></span>|<span data-ttu-id="626f0-131">说明</span><span class="sxs-lookup"><span data-stu-id="626f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="626f0-132">label</span><span class="sxs-lookup"><span data-stu-id="626f0-132">label</span></span>|<span data-ttu-id="626f0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="626f0-133">String</span></span>|<span data-ttu-id="626f0-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="626f0-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="626f0-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="626f0-135">The default value is empty.</span></span> <span data-ttu-id="626f0-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="626f0-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="626f0-137">id</span><span class="sxs-lookup"><span data-stu-id="626f0-137">id</span></span>|<span data-ttu-id="626f0-138">字符串</span><span class="sxs-lookup"><span data-stu-id="626f0-138">String</span></span>|<span data-ttu-id="626f0-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="626f0-139">Key of the entity.</span></span> <span data-ttu-id="626f0-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="626f0-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="626f0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="626f0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="626f0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="626f0-142">DateTimeOffset</span></span>|<span data-ttu-id="626f0-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="626f0-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="626f0-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="626f0-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="626f0-145">defaultItem</span><span class="sxs-lookup"><span data-stu-id="626f0-145">defaultItem</span></span>|[<span data-ttu-id="626f0-146">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="626f0-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="626f0-147">用于标识项目列表的默认选择的本地化字符串值。</span><span class="sxs-lookup"><span data-stu-id="626f0-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="626f0-148">items</span><span class="sxs-lookup"><span data-stu-id="626f0-148">items</span></span>|<span data-ttu-id="626f0-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="626f0-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="626f0-150">表示一组本地化的显示名称及其关联的值。</span><span class="sxs-lookup"><span data-stu-id="626f0-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="626f0-151">必需</span><span class="sxs-lookup"><span data-stu-id="626f0-151">required</span></span>|<span data-ttu-id="626f0-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="626f0-152">Boolean</span></span>|<span data-ttu-id="626f0-153">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="626f0-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="626f0-154">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="626f0-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="626f0-155">响应</span><span class="sxs-lookup"><span data-stu-id="626f0-155">Response</span></span>
<span data-ttu-id="626f0-156">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="626f0-156">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="626f0-157">示例</span><span class="sxs-lookup"><span data-stu-id="626f0-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="626f0-158">请求</span><span class="sxs-lookup"><span data-stu-id="626f0-158">Request</span></span>
<span data-ttu-id="626f0-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="626f0-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="626f0-160">响应</span><span class="sxs-lookup"><span data-stu-id="626f0-160">Response</span></span>
<span data-ttu-id="626f0-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="626f0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





