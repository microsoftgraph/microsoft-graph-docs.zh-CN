---
title: 更新 groupPolicyPresentationListBox
description: 更新 groupPolicyPresentationListBox 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e7792f1359b76804c57ff1d814b8141113b4c5d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357773"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="43037-103">更新 groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="43037-103">Update groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="43037-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43037-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43037-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43037-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43037-106">更新[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="43037-106">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43037-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="43037-107">Prerequisites</span></span>
<span data-ttu-id="43037-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43037-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="43037-110">Permission type</span></span>|<span data-ttu-id="43037-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43037-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43037-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43037-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43037-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43037-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43037-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43037-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43037-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="43037-115">Not supported.</span></span>|
|<span data-ttu-id="43037-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="43037-116">Application</span></span>|<span data-ttu-id="43037-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43037-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43037-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43037-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="43037-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="43037-119">Request headers</span></span>
|<span data-ttu-id="43037-120">标头</span><span class="sxs-lookup"><span data-stu-id="43037-120">Header</span></span>|<span data-ttu-id="43037-121">值</span><span class="sxs-lookup"><span data-stu-id="43037-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43037-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43037-122">Authorization</span></span>|<span data-ttu-id="43037-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43037-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43037-124">接受</span><span class="sxs-lookup"><span data-stu-id="43037-124">Accept</span></span>|<span data-ttu-id="43037-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43037-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43037-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="43037-126">Request body</span></span>
<span data-ttu-id="43037-127">在请求正文中, 提供[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43037-127">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="43037-128">下表显示创建[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="43037-128">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="43037-129">属性</span><span class="sxs-lookup"><span data-stu-id="43037-129">Property</span></span>|<span data-ttu-id="43037-130">类型</span><span class="sxs-lookup"><span data-stu-id="43037-130">Type</span></span>|<span data-ttu-id="43037-131">说明</span><span class="sxs-lookup"><span data-stu-id="43037-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43037-132">label</span><span class="sxs-lookup"><span data-stu-id="43037-132">label</span></span>|<span data-ttu-id="43037-133">String</span><span class="sxs-lookup"><span data-stu-id="43037-133">String</span></span>|<span data-ttu-id="43037-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="43037-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="43037-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="43037-135">The default value is empty.</span></span> <span data-ttu-id="43037-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="43037-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="43037-137">id</span><span class="sxs-lookup"><span data-stu-id="43037-137">id</span></span>|<span data-ttu-id="43037-138">String</span><span class="sxs-lookup"><span data-stu-id="43037-138">String</span></span>|<span data-ttu-id="43037-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="43037-139">Key of the entity.</span></span> <span data-ttu-id="43037-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="43037-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="43037-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43037-141">lastModifiedDateTime</span></span>|<span data-ttu-id="43037-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43037-142">DateTimeOffset</span></span>|<span data-ttu-id="43037-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="43037-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="43037-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="43037-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="43037-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="43037-145">explicitValue</span></span>|<span data-ttu-id="43037-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="43037-146">Boolean</span></span>|<span data-ttu-id="43037-147">如果指定此选项, 则用户必须指定注册表子项值和注册表子项名称。</span><span class="sxs-lookup"><span data-stu-id="43037-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="43037-148">列表框显示两列, 一个用于名称, 一个用于数据。</span><span class="sxs-lookup"><span data-stu-id="43037-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="43037-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="43037-149">The default value is false.</span></span>|
|<span data-ttu-id="43037-150">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="43037-150">valuePrefix</span></span>|<span data-ttu-id="43037-151">String</span><span class="sxs-lookup"><span data-stu-id="43037-151">String</span></span>|<span data-ttu-id="43037-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="43037-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43037-153">响应</span><span class="sxs-lookup"><span data-stu-id="43037-153">Response</span></span>
<span data-ttu-id="43037-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="43037-154">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43037-155">示例</span><span class="sxs-lookup"><span data-stu-id="43037-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="43037-156">请求</span><span class="sxs-lookup"><span data-stu-id="43037-156">Request</span></span>
<span data-ttu-id="43037-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43037-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a><span data-ttu-id="43037-158">响应</span><span class="sxs-lookup"><span data-stu-id="43037-158">Response</span></span>
<span data-ttu-id="43037-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43037-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```






