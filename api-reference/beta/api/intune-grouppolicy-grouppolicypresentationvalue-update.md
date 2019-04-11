---
title: 更新 groupPolicyPresentationValue
description: 更新 groupPolicyPresentationValue 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e81726ea683b200c3e2a26071d834c7ab6b3428
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784054"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="b5b95-103">更新 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="b5b95-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="b5b95-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5b95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5b95-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5b95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5b95-106">更新[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5b95-106">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5b95-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5b95-107">Prerequisites</span></span>
<span data-ttu-id="b5b95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5b95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5b95-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5b95-110">Permission type</span></span>|<span data-ttu-id="b5b95-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5b95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5b95-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5b95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5b95-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b95-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b5b95-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5b95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5b95-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5b95-115">Not supported.</span></span>|
|<span data-ttu-id="b5b95-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5b95-116">Application</span></span>|<span data-ttu-id="b5b95-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5b95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5b95-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5b95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="b5b95-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5b95-119">Request headers</span></span>
|<span data-ttu-id="b5b95-120">标头</span><span class="sxs-lookup"><span data-stu-id="b5b95-120">Header</span></span>|<span data-ttu-id="b5b95-121">值</span><span class="sxs-lookup"><span data-stu-id="b5b95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5b95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5b95-122">Authorization</span></span>|<span data-ttu-id="b5b95-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5b95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5b95-124">接受</span><span class="sxs-lookup"><span data-stu-id="b5b95-124">Accept</span></span>|<span data-ttu-id="b5b95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5b95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5b95-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5b95-126">Request body</span></span>
<span data-ttu-id="b5b95-127">在请求正文中, 提供[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5b95-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="b5b95-128">下表显示创建[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5b95-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="b5b95-129">属性</span><span class="sxs-lookup"><span data-stu-id="b5b95-129">Property</span></span>|<span data-ttu-id="b5b95-130">类型</span><span class="sxs-lookup"><span data-stu-id="b5b95-130">Type</span></span>|<span data-ttu-id="b5b95-131">说明</span><span class="sxs-lookup"><span data-stu-id="b5b95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5b95-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5b95-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b5b95-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5b95-133">DateTimeOffset</span></span>|<span data-ttu-id="b5b95-134">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b5b95-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="b5b95-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5b95-135">createdDateTime</span></span>|<span data-ttu-id="b5b95-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5b95-136">DateTimeOffset</span></span>|<span data-ttu-id="b5b95-137">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b5b95-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="b5b95-138">id</span><span class="sxs-lookup"><span data-stu-id="b5b95-138">id</span></span>|<span data-ttu-id="b5b95-139">String</span><span class="sxs-lookup"><span data-stu-id="b5b95-139">String</span></span>|<span data-ttu-id="b5b95-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5b95-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b5b95-141">响应</span><span class="sxs-lookup"><span data-stu-id="b5b95-141">Response</span></span>
<span data-ttu-id="b5b95-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5b95-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5b95-143">示例</span><span class="sxs-lookup"><span data-stu-id="b5b95-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5b95-144">请求</span><span class="sxs-lookup"><span data-stu-id="b5b95-144">Request</span></span>
<span data-ttu-id="b5b95-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5b95-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="b5b95-146">响应</span><span class="sxs-lookup"><span data-stu-id="b5b95-146">Response</span></span>
<span data-ttu-id="b5b95-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5b95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```





