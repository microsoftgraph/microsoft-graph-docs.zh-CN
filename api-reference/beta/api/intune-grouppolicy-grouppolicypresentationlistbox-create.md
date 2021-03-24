---
title: 创建 groupPolicyPresentationListBox
description: 创建新的 groupPolicyPresentationListBox 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 561a591e61ef5d6872f2eec63c24964b7827ce43
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135388"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="99c1a-103">创建 groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="99c1a-103">Create groupPolicyPresentationListBox</span></span>

<span data-ttu-id="99c1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99c1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99c1a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99c1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99c1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99c1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c1a-107">创建新的 [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99c1a-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99c1a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="99c1a-108">Prerequisites</span></span>
<span data-ttu-id="99c1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99c1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c1a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99c1a-111">Permission type</span></span>|<span data-ttu-id="99c1a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99c1a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99c1a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99c1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99c1a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c1a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99c1a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99c1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99c1a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99c1a-116">Not supported.</span></span>|
|<span data-ttu-id="99c1a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="99c1a-117">Application</span></span>|<span data-ttu-id="99c1a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c1a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99c1a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99c1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="99c1a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99c1a-120">Request headers</span></span>
|<span data-ttu-id="99c1a-121">标头</span><span class="sxs-lookup"><span data-stu-id="99c1a-121">Header</span></span>|<span data-ttu-id="99c1a-122">值</span><span class="sxs-lookup"><span data-stu-id="99c1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99c1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99c1a-123">Authorization</span></span>|<span data-ttu-id="99c1a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99c1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99c1a-125">接受</span><span class="sxs-lookup"><span data-stu-id="99c1a-125">Accept</span></span>|<span data-ttu-id="99c1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99c1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c1a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="99c1a-127">Request body</span></span>
<span data-ttu-id="99c1a-128">在请求正文中，提供 groupPolicyPresentationListBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99c1a-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="99c1a-129">下表显示创建 groupPolicyPresentationListBox 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="99c1a-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="99c1a-130">属性</span><span class="sxs-lookup"><span data-stu-id="99c1a-130">Property</span></span>|<span data-ttu-id="99c1a-131">类型</span><span class="sxs-lookup"><span data-stu-id="99c1a-131">Type</span></span>|<span data-ttu-id="99c1a-132">说明</span><span class="sxs-lookup"><span data-stu-id="99c1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c1a-133">label</span><span class="sxs-lookup"><span data-stu-id="99c1a-133">label</span></span>|<span data-ttu-id="99c1a-134">String</span><span class="sxs-lookup"><span data-stu-id="99c1a-134">String</span></span>|<span data-ttu-id="99c1a-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="99c1a-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="99c1a-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="99c1a-136">The default value is empty.</span></span> <span data-ttu-id="99c1a-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="99c1a-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="99c1a-138">id</span><span class="sxs-lookup"><span data-stu-id="99c1a-138">id</span></span>|<span data-ttu-id="99c1a-139">String</span><span class="sxs-lookup"><span data-stu-id="99c1a-139">String</span></span>|<span data-ttu-id="99c1a-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="99c1a-140">Key of the entity.</span></span> <span data-ttu-id="99c1a-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="99c1a-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="99c1a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99c1a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="99c1a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99c1a-143">DateTimeOffset</span></span>|<span data-ttu-id="99c1a-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="99c1a-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="99c1a-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="99c1a-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="99c1a-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="99c1a-146">explicitValue</span></span>|<span data-ttu-id="99c1a-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="99c1a-147">Boolean</span></span>|<span data-ttu-id="99c1a-148">如果指定此选项，则用户必须指定注册表子项值和注册表子项名称。</span><span class="sxs-lookup"><span data-stu-id="99c1a-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="99c1a-149">列表框显示两列，一列用于名称，另一列用于数据。</span><span class="sxs-lookup"><span data-stu-id="99c1a-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="99c1a-150">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="99c1a-150">The default value is false.</span></span>|
|<span data-ttu-id="99c1a-151">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="99c1a-151">valuePrefix</span></span>|<span data-ttu-id="99c1a-152">String</span><span class="sxs-lookup"><span data-stu-id="99c1a-152">String</span></span>|<span data-ttu-id="99c1a-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99c1a-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="99c1a-154">响应</span><span class="sxs-lookup"><span data-stu-id="99c1a-154">Response</span></span>
<span data-ttu-id="99c1a-155">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99c1a-155">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99c1a-156">示例</span><span class="sxs-lookup"><span data-stu-id="99c1a-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="99c1a-157">请求</span><span class="sxs-lookup"><span data-stu-id="99c1a-157">Request</span></span>
<span data-ttu-id="99c1a-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99c1a-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99c1a-159">响应</span><span class="sxs-lookup"><span data-stu-id="99c1a-159">Response</span></span>
<span data-ttu-id="99c1a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99c1a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




