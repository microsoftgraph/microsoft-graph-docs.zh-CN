---
title: 更新 groupPolicyPresentationListBox
description: 更新 groupPolicyPresentationListBox 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 71b67c8d6c18f94e42fade17500d681e915230e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153298"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="725d5-103">更新 groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="725d5-103">Update groupPolicyPresentationListBox</span></span>

<span data-ttu-id="725d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="725d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="725d5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="725d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="725d5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="725d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="725d5-107">更新 [groupPolicyPresentationListBox 对象](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="725d5-107">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="725d5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="725d5-108">Prerequisites</span></span>
<span data-ttu-id="725d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="725d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="725d5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="725d5-111">Permission type</span></span>|<span data-ttu-id="725d5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="725d5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="725d5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="725d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="725d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="725d5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="725d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="725d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="725d5-116">Not supported.</span></span>|
|<span data-ttu-id="725d5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="725d5-117">Application</span></span>|<span data-ttu-id="725d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="725d5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="725d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="725d5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="725d5-120">Request headers</span></span>
|<span data-ttu-id="725d5-121">标头</span><span class="sxs-lookup"><span data-stu-id="725d5-121">Header</span></span>|<span data-ttu-id="725d5-122">值</span><span class="sxs-lookup"><span data-stu-id="725d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="725d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="725d5-123">Authorization</span></span>|<span data-ttu-id="725d5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="725d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="725d5-125">接受</span><span class="sxs-lookup"><span data-stu-id="725d5-125">Accept</span></span>|<span data-ttu-id="725d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="725d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="725d5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="725d5-127">Request body</span></span>
<span data-ttu-id="725d5-128">在请求正文中，提供 [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="725d5-128">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="725d5-129">下表显示创建 [groupPolicyPresentationListBox 时所需的属性](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)。</span><span class="sxs-lookup"><span data-stu-id="725d5-129">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="725d5-130">属性</span><span class="sxs-lookup"><span data-stu-id="725d5-130">Property</span></span>|<span data-ttu-id="725d5-131">类型</span><span class="sxs-lookup"><span data-stu-id="725d5-131">Type</span></span>|<span data-ttu-id="725d5-132">说明</span><span class="sxs-lookup"><span data-stu-id="725d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="725d5-133">label</span><span class="sxs-lookup"><span data-stu-id="725d5-133">label</span></span>|<span data-ttu-id="725d5-134">String</span><span class="sxs-lookup"><span data-stu-id="725d5-134">String</span></span>|<span data-ttu-id="725d5-135">任何演示文稿实体的本地化文本标签。</span><span class="sxs-lookup"><span data-stu-id="725d5-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="725d5-136">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="725d5-136">The default value is empty.</span></span> <span data-ttu-id="725d5-137">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="725d5-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="725d5-138">id</span><span class="sxs-lookup"><span data-stu-id="725d5-138">id</span></span>|<span data-ttu-id="725d5-139">String</span><span class="sxs-lookup"><span data-stu-id="725d5-139">String</span></span>|<span data-ttu-id="725d5-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="725d5-140">Key of the entity.</span></span> <span data-ttu-id="725d5-141">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="725d5-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="725d5-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="725d5-142">lastModifiedDateTime</span></span>|<span data-ttu-id="725d5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="725d5-143">DateTimeOffset</span></span>|<span data-ttu-id="725d5-144">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="725d5-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="725d5-145">继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="725d5-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="725d5-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="725d5-146">explicitValue</span></span>|<span data-ttu-id="725d5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="725d5-147">Boolean</span></span>|<span data-ttu-id="725d5-148">如果指定此选项，则用户必须指定注册表子项值和注册表子项名称。</span><span class="sxs-lookup"><span data-stu-id="725d5-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="725d5-149">列表框显示两列，一列用于名称，另一列用于数据。</span><span class="sxs-lookup"><span data-stu-id="725d5-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="725d5-150">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="725d5-150">The default value is false.</span></span>|
|<span data-ttu-id="725d5-151">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="725d5-151">valuePrefix</span></span>|<span data-ttu-id="725d5-152">String</span><span class="sxs-lookup"><span data-stu-id="725d5-152">String</span></span>|<span data-ttu-id="725d5-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="725d5-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="725d5-154">响应</span><span class="sxs-lookup"><span data-stu-id="725d5-154">Response</span></span>
<span data-ttu-id="725d5-155">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="725d5-155">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="725d5-156">示例</span><span class="sxs-lookup"><span data-stu-id="725d5-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="725d5-157">请求</span><span class="sxs-lookup"><span data-stu-id="725d5-157">Request</span></span>
<span data-ttu-id="725d5-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="725d5-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="725d5-159">响应</span><span class="sxs-lookup"><span data-stu-id="725d5-159">Response</span></span>
<span data-ttu-id="725d5-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="725d5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




