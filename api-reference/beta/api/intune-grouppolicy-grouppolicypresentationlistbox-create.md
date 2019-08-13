---
title: 创建 groupPolicyPresentationListBox
description: 创建新的 groupPolicyPresentationListBox 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c895b9d1e935d9e490d4685f3ea9a8669ae679aa
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357801"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="f33d9-103">创建 groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="f33d9-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="f33d9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f33d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f33d9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f33d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f33d9-106">创建新的[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f33d9-106">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f33d9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f33d9-107">Prerequisites</span></span>
<span data-ttu-id="f33d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f33d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f33d9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f33d9-110">Permission type</span></span>|<span data-ttu-id="f33d9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f33d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f33d9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f33d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f33d9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f33d9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f33d9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f33d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f33d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f33d9-115">Not supported.</span></span>|
|<span data-ttu-id="f33d9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f33d9-116">Application</span></span>|<span data-ttu-id="f33d9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f33d9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f33d9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f33d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="f33d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f33d9-119">Request headers</span></span>
|<span data-ttu-id="f33d9-120">标头</span><span class="sxs-lookup"><span data-stu-id="f33d9-120">Header</span></span>|<span data-ttu-id="f33d9-121">值</span><span class="sxs-lookup"><span data-stu-id="f33d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f33d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f33d9-122">Authorization</span></span>|<span data-ttu-id="f33d9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f33d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f33d9-124">接受</span><span class="sxs-lookup"><span data-stu-id="f33d9-124">Accept</span></span>|<span data-ttu-id="f33d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f33d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f33d9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f33d9-126">Request body</span></span>
<span data-ttu-id="f33d9-127">在请求正文中, 提供 groupPolicyPresentationListBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f33d9-127">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="f33d9-128">下表显示创建 groupPolicyPresentationListBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f33d9-128">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="f33d9-129">属性</span><span class="sxs-lookup"><span data-stu-id="f33d9-129">Property</span></span>|<span data-ttu-id="f33d9-130">类型</span><span class="sxs-lookup"><span data-stu-id="f33d9-130">Type</span></span>|<span data-ttu-id="f33d9-131">说明</span><span class="sxs-lookup"><span data-stu-id="f33d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f33d9-132">label</span><span class="sxs-lookup"><span data-stu-id="f33d9-132">label</span></span>|<span data-ttu-id="f33d9-133">String</span><span class="sxs-lookup"><span data-stu-id="f33d9-133">String</span></span>|<span data-ttu-id="f33d9-134">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="f33d9-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f33d9-135">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="f33d9-135">The default value is empty.</span></span> <span data-ttu-id="f33d9-136">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f33d9-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f33d9-137">id</span><span class="sxs-lookup"><span data-stu-id="f33d9-137">id</span></span>|<span data-ttu-id="f33d9-138">String</span><span class="sxs-lookup"><span data-stu-id="f33d9-138">String</span></span>|<span data-ttu-id="f33d9-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f33d9-139">Key of the entity.</span></span> <span data-ttu-id="f33d9-140">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f33d9-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f33d9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f33d9-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f33d9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f33d9-142">DateTimeOffset</span></span>|<span data-ttu-id="f33d9-143">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f33d9-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="f33d9-144">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f33d9-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f33d9-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="f33d9-145">explicitValue</span></span>|<span data-ttu-id="f33d9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f33d9-146">Boolean</span></span>|<span data-ttu-id="f33d9-147">如果指定此选项, 则用户必须指定注册表子项值和注册表子项名称。</span><span class="sxs-lookup"><span data-stu-id="f33d9-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="f33d9-148">列表框显示两列, 一个用于名称, 一个用于数据。</span><span class="sxs-lookup"><span data-stu-id="f33d9-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="f33d9-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="f33d9-149">The default value is false.</span></span>|
|<span data-ttu-id="f33d9-150">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="f33d9-150">valuePrefix</span></span>|<span data-ttu-id="f33d9-151">String</span><span class="sxs-lookup"><span data-stu-id="f33d9-151">String</span></span>|<span data-ttu-id="f33d9-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f33d9-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f33d9-153">响应</span><span class="sxs-lookup"><span data-stu-id="f33d9-153">Response</span></span>
<span data-ttu-id="f33d9-154">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f33d9-154">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f33d9-155">示例</span><span class="sxs-lookup"><span data-stu-id="f33d9-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="f33d9-156">请求</span><span class="sxs-lookup"><span data-stu-id="f33d9-156">Request</span></span>
<span data-ttu-id="f33d9-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f33d9-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a><span data-ttu-id="f33d9-158">响应</span><span class="sxs-lookup"><span data-stu-id="f33d9-158">Response</span></span>
<span data-ttu-id="f33d9-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f33d9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






