---
title: 创建 groupPolicyPresentationDropdownList
description: 创建新的 groupPolicyPresentationDropdownList 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 28ea40014bd87f9f032c2a831b18a25016f13ee5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020417"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="f48f1-103">创建 groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="f48f1-103">Create groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="f48f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f48f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f48f1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f48f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f48f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f48f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f48f1-107">创建新的 [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f48f1-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f48f1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f48f1-108">Prerequisites</span></span>
<span data-ttu-id="f48f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f48f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f48f1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f48f1-111">Permission type</span></span>|<span data-ttu-id="f48f1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f48f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f48f1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f48f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f48f1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48f1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f48f1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f48f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f48f1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f48f1-116">Not supported.</span></span>|
|<span data-ttu-id="f48f1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f48f1-117">Application</span></span>|<span data-ttu-id="f48f1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48f1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f48f1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f48f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="f48f1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f48f1-120">Request headers</span></span>
|<span data-ttu-id="f48f1-121">标头</span><span class="sxs-lookup"><span data-stu-id="f48f1-121">Header</span></span>|<span data-ttu-id="f48f1-122">值</span><span class="sxs-lookup"><span data-stu-id="f48f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f48f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f48f1-123">Authorization</span></span>|<span data-ttu-id="f48f1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f48f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f48f1-125">接受</span><span class="sxs-lookup"><span data-stu-id="f48f1-125">Accept</span></span>|<span data-ttu-id="f48f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f48f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f48f1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f48f1-127">Request body</span></span>
<span data-ttu-id="f48f1-128">在请求正文中，提供 groupPolicyPresentationDropdownList 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f48f1-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="f48f1-129">下表显示创建 groupPolicyPresentationDropdownList 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f48f1-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="f48f1-130">属性</span><span class="sxs-lookup"><span data-stu-id="f48f1-130">Property</span></span>|<span data-ttu-id="f48f1-131">类型</span><span class="sxs-lookup"><span data-stu-id="f48f1-131">Type</span></span>|<span data-ttu-id="f48f1-132">说明</span><span class="sxs-lookup"><span data-stu-id="f48f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f48f1-133">label</span><span class="sxs-lookup"><span data-stu-id="f48f1-133">label</span></span>|<span data-ttu-id="f48f1-134">String</span><span class="sxs-lookup"><span data-stu-id="f48f1-134">String</span></span>|<span data-ttu-id="f48f1-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="f48f1-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f48f1-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="f48f1-136">The default value is empty.</span></span> <span data-ttu-id="f48f1-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f48f1-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f48f1-138">id</span><span class="sxs-lookup"><span data-stu-id="f48f1-138">id</span></span>|<span data-ttu-id="f48f1-139">String</span><span class="sxs-lookup"><span data-stu-id="f48f1-139">String</span></span>|<span data-ttu-id="f48f1-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f48f1-140">Key of the entity.</span></span> <span data-ttu-id="f48f1-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f48f1-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f48f1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f48f1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f48f1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f48f1-143">DateTimeOffset</span></span>|<span data-ttu-id="f48f1-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f48f1-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="f48f1-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f48f1-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f48f1-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="f48f1-146">defaultItem</span></span>|[<span data-ttu-id="f48f1-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="f48f1-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="f48f1-148">用于标识项目列表的默认选择的本地化字符串值。</span><span class="sxs-lookup"><span data-stu-id="f48f1-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="f48f1-149">items</span><span class="sxs-lookup"><span data-stu-id="f48f1-149">items</span></span>|<span data-ttu-id="f48f1-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f48f1-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="f48f1-151">表示一组本地化的显示名称及其关联的值。</span><span class="sxs-lookup"><span data-stu-id="f48f1-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="f48f1-152">必需</span><span class="sxs-lookup"><span data-stu-id="f48f1-152">required</span></span>|<span data-ttu-id="f48f1-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f48f1-153">Boolean</span></span>|<span data-ttu-id="f48f1-154">要求在 "参数" 框中输入值。</span><span class="sxs-lookup"><span data-stu-id="f48f1-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="f48f1-155">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="f48f1-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="f48f1-156">响应</span><span class="sxs-lookup"><span data-stu-id="f48f1-156">Response</span></span>
<span data-ttu-id="f48f1-157">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f48f1-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f48f1-158">示例</span><span class="sxs-lookup"><span data-stu-id="f48f1-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f48f1-159">请求</span><span class="sxs-lookup"><span data-stu-id="f48f1-159">Request</span></span>
<span data-ttu-id="f48f1-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f48f1-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f48f1-161">响应</span><span class="sxs-lookup"><span data-stu-id="f48f1-161">Response</span></span>
<span data-ttu-id="f48f1-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f48f1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






