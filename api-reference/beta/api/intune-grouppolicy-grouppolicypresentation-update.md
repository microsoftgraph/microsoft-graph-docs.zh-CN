---
title: 更新 groupPolicyPresentation
description: 更新 groupPolicyPresentation 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 26f185d1474402f77f8dab09c500a1c11892f77b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431342"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="a60bc-103">更新 groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="a60bc-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="a60bc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a60bc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a60bc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a60bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a60bc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a60bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a60bc-107">更新[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a60bc-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a60bc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a60bc-108">Prerequisites</span></span>
<span data-ttu-id="a60bc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a60bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a60bc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a60bc-111">Permission type</span></span>|<span data-ttu-id="a60bc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a60bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a60bc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a60bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a60bc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a60bc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a60bc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a60bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a60bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a60bc-116">Not supported.</span></span>|
|<span data-ttu-id="a60bc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a60bc-117">Application</span></span>|<span data-ttu-id="a60bc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a60bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a60bc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a60bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="a60bc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a60bc-120">Request headers</span></span>
|<span data-ttu-id="a60bc-121">标头</span><span class="sxs-lookup"><span data-stu-id="a60bc-121">Header</span></span>|<span data-ttu-id="a60bc-122">值</span><span class="sxs-lookup"><span data-stu-id="a60bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a60bc-123">授权</span><span class="sxs-lookup"><span data-stu-id="a60bc-123">Authorization</span></span>|<span data-ttu-id="a60bc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a60bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a60bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a60bc-125">Accept</span></span>|<span data-ttu-id="a60bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a60bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a60bc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a60bc-127">Request body</span></span>
<span data-ttu-id="a60bc-128">在请求正文中，提供[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a60bc-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="a60bc-129">下表显示时创建[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a60bc-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="a60bc-130">属性</span><span class="sxs-lookup"><span data-stu-id="a60bc-130">Property</span></span>|<span data-ttu-id="a60bc-131">类型</span><span class="sxs-lookup"><span data-stu-id="a60bc-131">Type</span></span>|<span data-ttu-id="a60bc-132">说明</span><span class="sxs-lookup"><span data-stu-id="a60bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a60bc-133">标签</span><span class="sxs-lookup"><span data-stu-id="a60bc-133">label</span></span>|<span data-ttu-id="a60bc-134">String</span><span class="sxs-lookup"><span data-stu-id="a60bc-134">String</span></span>|<span data-ttu-id="a60bc-135">任何演示文稿实体的本地化的文本标签。</span><span class="sxs-lookup"><span data-stu-id="a60bc-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a60bc-136">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="a60bc-136">The default value is empty.</span></span>|
|<span data-ttu-id="a60bc-137">id</span><span class="sxs-lookup"><span data-stu-id="a60bc-137">id</span></span>|<span data-ttu-id="a60bc-138">String</span><span class="sxs-lookup"><span data-stu-id="a60bc-138">String</span></span>|<span data-ttu-id="a60bc-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a60bc-139">Key of the entity.</span></span>|
|<span data-ttu-id="a60bc-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a60bc-140">lastModifiedDateTime</span></span>|<span data-ttu-id="a60bc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a60bc-141">DateTimeOffset</span></span>|<span data-ttu-id="a60bc-142">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="a60bc-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a60bc-143">响应</span><span class="sxs-lookup"><span data-stu-id="a60bc-143">Response</span></span>
<span data-ttu-id="a60bc-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a60bc-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a60bc-145">示例</span><span class="sxs-lookup"><span data-stu-id="a60bc-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="a60bc-146">请求</span><span class="sxs-lookup"><span data-stu-id="a60bc-146">Request</span></span>
<span data-ttu-id="a60bc-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a60bc-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="a60bc-148">响应</span><span class="sxs-lookup"><span data-stu-id="a60bc-148">Response</span></span>
<span data-ttu-id="a60bc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a60bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




