---
title: 创建 groupPolicyPresentationDropdownList
description: 创建新的 groupPolicyPresentationDropdownList 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 415ccd634e4206b2849fc5feecc4131d2f417d16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431381"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="9c635-103">创建 groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="9c635-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="9c635-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9c635-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9c635-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9c635-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c635-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c635-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c635-107">创建新的[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c635-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c635-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c635-108">Prerequisites</span></span>
<span data-ttu-id="9c635-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9c635-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9c635-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c635-111">Permission type</span></span>|<span data-ttu-id="9c635-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c635-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c635-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c635-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c635-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c635-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9c635-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c635-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c635-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c635-116">Not supported.</span></span>|
|<span data-ttu-id="9c635-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c635-117">Application</span></span>|<span data-ttu-id="9c635-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c635-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c635-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c635-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="9c635-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c635-120">Request headers</span></span>
|<span data-ttu-id="9c635-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c635-121">Header</span></span>|<span data-ttu-id="9c635-122">值</span><span class="sxs-lookup"><span data-stu-id="9c635-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c635-123">授权</span><span class="sxs-lookup"><span data-stu-id="9c635-123">Authorization</span></span>|<span data-ttu-id="9c635-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c635-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c635-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c635-125">Accept</span></span>|<span data-ttu-id="9c635-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c635-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c635-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c635-127">Request body</span></span>
<span data-ttu-id="9c635-128">在请求正文中，提供 groupPolicyPresentationDropdownList 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c635-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="9c635-129">下表显示时创建 groupPolicyPresentationDropdownList 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c635-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="9c635-130">属性</span><span class="sxs-lookup"><span data-stu-id="9c635-130">Property</span></span>|<span data-ttu-id="9c635-131">类型</span><span class="sxs-lookup"><span data-stu-id="9c635-131">Type</span></span>|<span data-ttu-id="9c635-132">说明</span><span class="sxs-lookup"><span data-stu-id="9c635-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c635-133">标签</span><span class="sxs-lookup"><span data-stu-id="9c635-133">label</span></span>|<span data-ttu-id="9c635-134">String</span><span class="sxs-lookup"><span data-stu-id="9c635-134">String</span></span>|<span data-ttu-id="9c635-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="9c635-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9c635-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="9c635-136">The default value is empty.</span></span> <span data-ttu-id="9c635-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9c635-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9c635-138">id</span><span class="sxs-lookup"><span data-stu-id="9c635-138">id</span></span>|<span data-ttu-id="9c635-139">String</span><span class="sxs-lookup"><span data-stu-id="9c635-139">String</span></span>|<span data-ttu-id="9c635-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9c635-140">Key of the entity.</span></span> <span data-ttu-id="9c635-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9c635-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9c635-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c635-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9c635-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c635-143">DateTimeOffset</span></span>|<span data-ttu-id="9c635-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="9c635-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="9c635-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9c635-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9c635-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="9c635-146">defaultItem</span></span>|[<span data-ttu-id="9c635-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="9c635-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="9c635-148">标识项目的列表的默认选项的本地化的字符串值。</span><span class="sxs-lookup"><span data-stu-id="9c635-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="9c635-149">项目</span><span class="sxs-lookup"><span data-stu-id="9c635-149">items</span></span>|<span data-ttu-id="9c635-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="9c635-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="9c635-151">表示一的本地化的显示名称和及其关联的值。</span><span class="sxs-lookup"><span data-stu-id="9c635-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="9c635-152">必需</span><span class="sxs-lookup"><span data-stu-id="9c635-152">required</span></span>|<span data-ttu-id="9c635-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c635-153">Boolean</span></span>|<span data-ttu-id="9c635-154">在参数框中输入值的要求。</span><span class="sxs-lookup"><span data-stu-id="9c635-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="9c635-155">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="9c635-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="9c635-156">响应</span><span class="sxs-lookup"><span data-stu-id="9c635-156">Response</span></span>
<span data-ttu-id="9c635-157">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c635-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c635-158">示例</span><span class="sxs-lookup"><span data-stu-id="9c635-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c635-159">请求</span><span class="sxs-lookup"><span data-stu-id="9c635-159">Request</span></span>
<span data-ttu-id="9c635-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c635-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c635-161">响应</span><span class="sxs-lookup"><span data-stu-id="9c635-161">Response</span></span>
<span data-ttu-id="9c635-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c635-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




