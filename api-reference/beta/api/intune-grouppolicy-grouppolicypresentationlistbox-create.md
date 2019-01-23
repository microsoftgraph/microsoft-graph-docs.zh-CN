---
title: 创建 groupPolicyPresentationListBox
description: 创建新的 groupPolicyPresentationListBox 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d080fe046af88939d4c505f3848d1a7f2b1f67d3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429371"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="faa3a-103">创建 groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="faa3a-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="faa3a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="faa3a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faa3a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="faa3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faa3a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="faa3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa3a-107">创建新的[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="faa3a-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faa3a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="faa3a-108">Prerequisites</span></span>
<span data-ttu-id="faa3a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="faa3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="faa3a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="faa3a-111">Permission type</span></span>|<span data-ttu-id="faa3a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="faa3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faa3a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="faa3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="faa3a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa3a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="faa3a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="faa3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faa3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="faa3a-116">Not supported.</span></span>|
|<span data-ttu-id="faa3a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="faa3a-117">Application</span></span>|<span data-ttu-id="faa3a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="faa3a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faa3a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="faa3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="faa3a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="faa3a-120">Request headers</span></span>
|<span data-ttu-id="faa3a-121">标头</span><span class="sxs-lookup"><span data-stu-id="faa3a-121">Header</span></span>|<span data-ttu-id="faa3a-122">值</span><span class="sxs-lookup"><span data-stu-id="faa3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faa3a-123">授权</span><span class="sxs-lookup"><span data-stu-id="faa3a-123">Authorization</span></span>|<span data-ttu-id="faa3a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="faa3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faa3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="faa3a-125">Accept</span></span>|<span data-ttu-id="faa3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="faa3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faa3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="faa3a-127">Request body</span></span>
<span data-ttu-id="faa3a-128">在请求正文中，提供 groupPolicyPresentationListBox 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faa3a-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="faa3a-129">下表显示时创建 groupPolicyPresentationListBox 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="faa3a-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="faa3a-130">属性</span><span class="sxs-lookup"><span data-stu-id="faa3a-130">Property</span></span>|<span data-ttu-id="faa3a-131">类型</span><span class="sxs-lookup"><span data-stu-id="faa3a-131">Type</span></span>|<span data-ttu-id="faa3a-132">说明</span><span class="sxs-lookup"><span data-stu-id="faa3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa3a-133">标签</span><span class="sxs-lookup"><span data-stu-id="faa3a-133">label</span></span>|<span data-ttu-id="faa3a-134">String</span><span class="sxs-lookup"><span data-stu-id="faa3a-134">String</span></span>|<span data-ttu-id="faa3a-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="faa3a-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="faa3a-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="faa3a-136">The default value is empty.</span></span> <span data-ttu-id="faa3a-137">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="faa3a-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="faa3a-138">id</span><span class="sxs-lookup"><span data-stu-id="faa3a-138">id</span></span>|<span data-ttu-id="faa3a-139">String</span><span class="sxs-lookup"><span data-stu-id="faa3a-139">String</span></span>|<span data-ttu-id="faa3a-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="faa3a-140">Key of the entity.</span></span> <span data-ttu-id="faa3a-141">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="faa3a-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="faa3a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faa3a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="faa3a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faa3a-143">DateTimeOffset</span></span>|<span data-ttu-id="faa3a-144">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="faa3a-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="faa3a-145">继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="faa3a-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="faa3a-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="faa3a-146">explicitValue</span></span>|<span data-ttu-id="faa3a-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa3a-147">Boolean</span></span>|<span data-ttu-id="faa3a-148">如果此选项将指定 true 用户必须指定该注册表子项值和注册表子项名称。</span><span class="sxs-lookup"><span data-stu-id="faa3a-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="faa3a-149">列表框中显示两列、 名称和数据。</span><span class="sxs-lookup"><span data-stu-id="faa3a-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="faa3a-150">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="faa3a-150">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="faa3a-151">响应</span><span class="sxs-lookup"><span data-stu-id="faa3a-151">Response</span></span>
<span data-ttu-id="faa3a-152">如果成功，此方法返回`201 Created`响应代码和响应正文中的[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)对象。</span><span class="sxs-lookup"><span data-stu-id="faa3a-152">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faa3a-153">示例</span><span class="sxs-lookup"><span data-stu-id="faa3a-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="faa3a-154">请求</span><span class="sxs-lookup"><span data-stu-id="faa3a-154">Request</span></span>
<span data-ttu-id="faa3a-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="faa3a-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="faa3a-156">响应</span><span class="sxs-lookup"><span data-stu-id="faa3a-156">Response</span></span>
<span data-ttu-id="faa3a-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="faa3a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```




