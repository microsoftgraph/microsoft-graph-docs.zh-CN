---
title: 更新 termsAndConditions
description: 更新 termsAndConditions 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a866b17861c3c11047607f4af6691fc810648142
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760149"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="23561-103">更新 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="23561-103">Update termsAndConditions</span></span>

> <span data-ttu-id="23561-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23561-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23561-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23561-106">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23561-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23561-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="23561-107">Prerequisites</span></span>
<span data-ttu-id="23561-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23561-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="23561-110">Permission type</span></span>|<span data-ttu-id="23561-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="23561-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23561-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23561-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23561-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23561-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23561-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23561-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23561-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="23561-115">Not supported.</span></span>|
|<span data-ttu-id="23561-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="23561-116">Application</span></span>|<span data-ttu-id="23561-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23561-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23561-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23561-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="23561-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="23561-119">Request headers</span></span>
|<span data-ttu-id="23561-120">标头</span><span class="sxs-lookup"><span data-stu-id="23561-120">Header</span></span>|<span data-ttu-id="23561-121">值</span><span class="sxs-lookup"><span data-stu-id="23561-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23561-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="23561-122">Authorization</span></span>|<span data-ttu-id="23561-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="23561-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23561-124">接受</span><span class="sxs-lookup"><span data-stu-id="23561-124">Accept</span></span>|<span data-ttu-id="23561-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23561-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23561-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="23561-126">Request body</span></span>
<span data-ttu-id="23561-127">在请求正文中，提供 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23561-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="23561-128">下表显示创建 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="23561-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="23561-129">属性</span><span class="sxs-lookup"><span data-stu-id="23561-129">Property</span></span>|<span data-ttu-id="23561-130">类型</span><span class="sxs-lookup"><span data-stu-id="23561-130">Type</span></span>|<span data-ttu-id="23561-131">说明</span><span class="sxs-lookup"><span data-stu-id="23561-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23561-132">id</span><span class="sxs-lookup"><span data-stu-id="23561-132">id</span></span>|<span data-ttu-id="23561-133">字符串</span><span class="sxs-lookup"><span data-stu-id="23561-133">String</span></span>|<span data-ttu-id="23561-134">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="23561-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="23561-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23561-135">createdDateTime</span></span>|<span data-ttu-id="23561-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23561-136">DateTimeOffset</span></span>|<span data-ttu-id="23561-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="23561-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="23561-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23561-138">modifiedDateTime</span></span>|<span data-ttu-id="23561-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23561-139">DateTimeOffset</span></span>|<span data-ttu-id="23561-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="23561-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="23561-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23561-141">lastModifiedDateTime</span></span>|<span data-ttu-id="23561-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23561-142">DateTimeOffset</span></span>|<span data-ttu-id="23561-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="23561-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="23561-144">displayName</span><span class="sxs-lookup"><span data-stu-id="23561-144">displayName</span></span>|<span data-ttu-id="23561-145">String</span><span class="sxs-lookup"><span data-stu-id="23561-145">String</span></span>|<span data-ttu-id="23561-146">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="23561-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="23561-147">说明</span><span class="sxs-lookup"><span data-stu-id="23561-147">description</span></span>|<span data-ttu-id="23561-148">字符串</span><span class="sxs-lookup"><span data-stu-id="23561-148">String</span></span>|<span data-ttu-id="23561-149">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="23561-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="23561-150">title</span><span class="sxs-lookup"><span data-stu-id="23561-150">title</span></span>|<span data-ttu-id="23561-151">String</span><span class="sxs-lookup"><span data-stu-id="23561-151">String</span></span>|<span data-ttu-id="23561-152">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="23561-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="23561-153">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="23561-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="23561-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="23561-154">bodyText</span></span>|<span data-ttu-id="23561-155">String</span><span class="sxs-lookup"><span data-stu-id="23561-155">String</span></span>|<span data-ttu-id="23561-156">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="23561-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="23561-157">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="23561-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="23561-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="23561-158">acceptanceStatement</span></span>|<span data-ttu-id="23561-159">String</span><span class="sxs-lookup"><span data-stu-id="23561-159">String</span></span>|<span data-ttu-id="23561-160">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="23561-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="23561-161">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="23561-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="23561-162">version</span><span class="sxs-lookup"><span data-stu-id="23561-162">version</span></span>|<span data-ttu-id="23561-163">Int32</span><span class="sxs-lookup"><span data-stu-id="23561-163">Int32</span></span>|<span data-ttu-id="23561-164">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="23561-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="23561-165">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="23561-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="23561-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23561-166">roleScopeTagIds</span></span>|<span data-ttu-id="23561-167">String collection</span><span class="sxs-lookup"><span data-stu-id="23561-167">String collection</span></span>|<span data-ttu-id="23561-168">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="23561-168">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="23561-169">响应</span><span class="sxs-lookup"><span data-stu-id="23561-169">Response</span></span>
<span data-ttu-id="23561-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23561-170">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23561-171">示例</span><span class="sxs-lookup"><span data-stu-id="23561-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="23561-172">请求</span><span class="sxs-lookup"><span data-stu-id="23561-172">Request</span></span>
<span data-ttu-id="23561-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23561-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
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

### <a name="response"></a><span data-ttu-id="23561-174">响应</span><span class="sxs-lookup"><span data-stu-id="23561-174">Response</span></span>
<span data-ttu-id="23561-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23561-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




