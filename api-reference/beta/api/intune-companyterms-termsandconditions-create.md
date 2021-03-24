---
title: 创建 termsAndConditions
description: 创建新的 termsAndConditions 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69b42125cf8f107ad94a3ab56438b7cba3d9dd50
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133666"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="1ce17-103">创建 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1ce17-103">Create termsAndConditions</span></span>

<span data-ttu-id="1ce17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ce17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ce17-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ce17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ce17-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ce17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ce17-107">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ce17-107">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ce17-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ce17-108">Prerequisites</span></span>
<span data-ttu-id="1ce17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ce17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ce17-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ce17-111">Permission type</span></span>|<span data-ttu-id="1ce17-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ce17-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ce17-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ce17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ce17-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ce17-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1ce17-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ce17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ce17-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ce17-116">Not supported.</span></span>|
|<span data-ttu-id="1ce17-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ce17-117">Application</span></span>|<span data-ttu-id="1ce17-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ce17-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ce17-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ce17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="1ce17-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ce17-120">Request headers</span></span>
|<span data-ttu-id="1ce17-121">标头</span><span class="sxs-lookup"><span data-stu-id="1ce17-121">Header</span></span>|<span data-ttu-id="1ce17-122">值</span><span class="sxs-lookup"><span data-stu-id="1ce17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ce17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ce17-123">Authorization</span></span>|<span data-ttu-id="1ce17-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ce17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ce17-125">接受</span><span class="sxs-lookup"><span data-stu-id="1ce17-125">Accept</span></span>|<span data-ttu-id="1ce17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ce17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ce17-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ce17-127">Request body</span></span>
<span data-ttu-id="1ce17-128">在请求正文中，提供 termsAndConditions 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ce17-128">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="1ce17-129">下表显示创建 termsAndConditions 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ce17-129">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="1ce17-130">属性</span><span class="sxs-lookup"><span data-stu-id="1ce17-130">Property</span></span>|<span data-ttu-id="1ce17-131">类型</span><span class="sxs-lookup"><span data-stu-id="1ce17-131">Type</span></span>|<span data-ttu-id="1ce17-132">说明</span><span class="sxs-lookup"><span data-stu-id="1ce17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce17-133">id</span><span class="sxs-lookup"><span data-stu-id="1ce17-133">id</span></span>|<span data-ttu-id="1ce17-134">String</span><span class="sxs-lookup"><span data-stu-id="1ce17-134">String</span></span>|<span data-ttu-id="1ce17-135">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1ce17-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="1ce17-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ce17-136">createdDateTime</span></span>|<span data-ttu-id="1ce17-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce17-137">DateTimeOffset</span></span>|<span data-ttu-id="1ce17-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1ce17-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="1ce17-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ce17-139">modifiedDateTime</span></span>|<span data-ttu-id="1ce17-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce17-140">DateTimeOffset</span></span>|<span data-ttu-id="1ce17-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1ce17-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1ce17-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ce17-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1ce17-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce17-143">DateTimeOffset</span></span>|<span data-ttu-id="1ce17-144">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1ce17-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1ce17-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1ce17-145">displayName</span></span>|<span data-ttu-id="1ce17-146">String</span><span class="sxs-lookup"><span data-stu-id="1ce17-146">String</span></span>|<span data-ttu-id="1ce17-147">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="1ce17-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="1ce17-148">说明</span><span class="sxs-lookup"><span data-stu-id="1ce17-148">description</span></span>|<span data-ttu-id="1ce17-149">String</span><span class="sxs-lookup"><span data-stu-id="1ce17-149">String</span></span>|<span data-ttu-id="1ce17-150">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="1ce17-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="1ce17-151">title</span><span class="sxs-lookup"><span data-stu-id="1ce17-151">title</span></span>|<span data-ttu-id="1ce17-152">String</span><span class="sxs-lookup"><span data-stu-id="1ce17-152">String</span></span>|<span data-ttu-id="1ce17-153">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="1ce17-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="1ce17-154">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="1ce17-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1ce17-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="1ce17-155">bodyText</span></span>|<span data-ttu-id="1ce17-156">String</span><span class="sxs-lookup"><span data-stu-id="1ce17-156">String</span></span>|<span data-ttu-id="1ce17-157">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="1ce17-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="1ce17-158">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="1ce17-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1ce17-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="1ce17-159">acceptanceStatement</span></span>|<span data-ttu-id="1ce17-160">String</span><span class="sxs-lookup"><span data-stu-id="1ce17-160">String</span></span>|<span data-ttu-id="1ce17-161">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="1ce17-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="1ce17-162">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="1ce17-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1ce17-163">version</span><span class="sxs-lookup"><span data-stu-id="1ce17-163">version</span></span>|<span data-ttu-id="1ce17-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1ce17-164">Int32</span></span>|<span data-ttu-id="1ce17-165">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="1ce17-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="1ce17-166">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="1ce17-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="1ce17-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ce17-167">roleScopeTagIds</span></span>|<span data-ttu-id="1ce17-168">String collection</span><span class="sxs-lookup"><span data-stu-id="1ce17-168">String collection</span></span>|<span data-ttu-id="1ce17-169">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1ce17-169">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="1ce17-170">响应</span><span class="sxs-lookup"><span data-stu-id="1ce17-170">Response</span></span>
<span data-ttu-id="1ce17-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ce17-171">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ce17-172">示例</span><span class="sxs-lookup"><span data-stu-id="1ce17-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ce17-173">请求</span><span class="sxs-lookup"><span data-stu-id="1ce17-173">Request</span></span>
<span data-ttu-id="1ce17-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ce17-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1ce17-175">响应</span><span class="sxs-lookup"><span data-stu-id="1ce17-175">Response</span></span>
<span data-ttu-id="1ce17-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ce17-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




