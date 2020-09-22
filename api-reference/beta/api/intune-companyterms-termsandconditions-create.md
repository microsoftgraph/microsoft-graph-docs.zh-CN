---
title: 创建 termsAndConditions
description: 创建新的 termsAndConditions 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34f7adbaf7476dc71a9251ae5e17fb8d7030b201
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975092"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="08740-103">创建 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="08740-103">Create termsAndConditions</span></span>

<span data-ttu-id="08740-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08740-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08740-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08740-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08740-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08740-107">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08740-107">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08740-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="08740-108">Prerequisites</span></span>
<span data-ttu-id="08740-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08740-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08740-111">Permission type</span></span>|<span data-ttu-id="08740-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08740-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08740-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08740-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08740-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08740-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08740-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08740-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08740-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08740-116">Not supported.</span></span>|
|<span data-ttu-id="08740-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08740-117">Application</span></span>|<span data-ttu-id="08740-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08740-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08740-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08740-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="08740-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08740-120">Request headers</span></span>
|<span data-ttu-id="08740-121">标头</span><span class="sxs-lookup"><span data-stu-id="08740-121">Header</span></span>|<span data-ttu-id="08740-122">值</span><span class="sxs-lookup"><span data-stu-id="08740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08740-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08740-123">Authorization</span></span>|<span data-ttu-id="08740-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08740-125">接受</span><span class="sxs-lookup"><span data-stu-id="08740-125">Accept</span></span>|<span data-ttu-id="08740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08740-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08740-127">Request body</span></span>
<span data-ttu-id="08740-128">在请求正文中，提供 termsAndConditions 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08740-128">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="08740-129">下表显示创建 termsAndConditions 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08740-129">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="08740-130">属性</span><span class="sxs-lookup"><span data-stu-id="08740-130">Property</span></span>|<span data-ttu-id="08740-131">类型</span><span class="sxs-lookup"><span data-stu-id="08740-131">Type</span></span>|<span data-ttu-id="08740-132">说明</span><span class="sxs-lookup"><span data-stu-id="08740-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08740-133">id</span><span class="sxs-lookup"><span data-stu-id="08740-133">id</span></span>|<span data-ttu-id="08740-134">String</span><span class="sxs-lookup"><span data-stu-id="08740-134">String</span></span>|<span data-ttu-id="08740-135">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="08740-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="08740-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08740-136">createdDateTime</span></span>|<span data-ttu-id="08740-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08740-137">DateTimeOffset</span></span>|<span data-ttu-id="08740-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="08740-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="08740-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08740-139">modifiedDateTime</span></span>|<span data-ttu-id="08740-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08740-140">DateTimeOffset</span></span>|<span data-ttu-id="08740-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="08740-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="08740-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08740-142">lastModifiedDateTime</span></span>|<span data-ttu-id="08740-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08740-143">DateTimeOffset</span></span>|<span data-ttu-id="08740-144">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="08740-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="08740-145">displayName</span><span class="sxs-lookup"><span data-stu-id="08740-145">displayName</span></span>|<span data-ttu-id="08740-146">String</span><span class="sxs-lookup"><span data-stu-id="08740-146">String</span></span>|<span data-ttu-id="08740-147">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="08740-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="08740-148">description</span><span class="sxs-lookup"><span data-stu-id="08740-148">description</span></span>|<span data-ttu-id="08740-149">String</span><span class="sxs-lookup"><span data-stu-id="08740-149">String</span></span>|<span data-ttu-id="08740-150">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="08740-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="08740-151">title</span><span class="sxs-lookup"><span data-stu-id="08740-151">title</span></span>|<span data-ttu-id="08740-152">String</span><span class="sxs-lookup"><span data-stu-id="08740-152">String</span></span>|<span data-ttu-id="08740-153">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="08740-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="08740-154">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="08740-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="08740-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="08740-155">bodyText</span></span>|<span data-ttu-id="08740-156">String</span><span class="sxs-lookup"><span data-stu-id="08740-156">String</span></span>|<span data-ttu-id="08740-157">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="08740-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="08740-158">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="08740-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="08740-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="08740-159">acceptanceStatement</span></span>|<span data-ttu-id="08740-160">String</span><span class="sxs-lookup"><span data-stu-id="08740-160">String</span></span>|<span data-ttu-id="08740-161">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="08740-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="08740-162">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="08740-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="08740-163">version</span><span class="sxs-lookup"><span data-stu-id="08740-163">version</span></span>|<span data-ttu-id="08740-164">Int32</span><span class="sxs-lookup"><span data-stu-id="08740-164">Int32</span></span>|<span data-ttu-id="08740-165">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="08740-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="08740-166">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="08740-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="08740-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08740-167">roleScopeTagIds</span></span>|<span data-ttu-id="08740-168">String collection</span><span class="sxs-lookup"><span data-stu-id="08740-168">String collection</span></span>|<span data-ttu-id="08740-169">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="08740-169">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="08740-170">响应</span><span class="sxs-lookup"><span data-stu-id="08740-170">Response</span></span>
<span data-ttu-id="08740-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08740-171">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08740-172">示例</span><span class="sxs-lookup"><span data-stu-id="08740-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="08740-173">请求</span><span class="sxs-lookup"><span data-stu-id="08740-173">Request</span></span>
<span data-ttu-id="08740-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08740-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08740-175">响应</span><span class="sxs-lookup"><span data-stu-id="08740-175">Response</span></span>
<span data-ttu-id="08740-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08740-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






