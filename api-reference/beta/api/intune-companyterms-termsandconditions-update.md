---
title: 更新 termsAndConditions
description: 更新 termsAndConditions 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5019102fbc3914a009544f44f1698084602456b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958633"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="54134-103">更新 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="54134-103">Update termsAndConditions</span></span>

> <span data-ttu-id="54134-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54134-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54134-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54134-106">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="54134-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54134-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="54134-107">Prerequisites</span></span>
<span data-ttu-id="54134-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54134-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="54134-110">Permission type</span></span>|<span data-ttu-id="54134-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="54134-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54134-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54134-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54134-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54134-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54134-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54134-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54134-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="54134-115">Not supported.</span></span>|
|<span data-ttu-id="54134-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="54134-116">Application</span></span>|<span data-ttu-id="54134-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="54134-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54134-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54134-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="54134-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54134-119">Request headers</span></span>
|<span data-ttu-id="54134-120">标头</span><span class="sxs-lookup"><span data-stu-id="54134-120">Header</span></span>|<span data-ttu-id="54134-121">值</span><span class="sxs-lookup"><span data-stu-id="54134-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54134-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54134-122">Authorization</span></span>|<span data-ttu-id="54134-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54134-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54134-124">接受</span><span class="sxs-lookup"><span data-stu-id="54134-124">Accept</span></span>|<span data-ttu-id="54134-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54134-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54134-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="54134-126">Request body</span></span>
<span data-ttu-id="54134-127">在请求正文中，提供 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54134-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="54134-128">下表显示创建 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="54134-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="54134-129">属性</span><span class="sxs-lookup"><span data-stu-id="54134-129">Property</span></span>|<span data-ttu-id="54134-130">类型</span><span class="sxs-lookup"><span data-stu-id="54134-130">Type</span></span>|<span data-ttu-id="54134-131">说明</span><span class="sxs-lookup"><span data-stu-id="54134-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54134-132">id</span><span class="sxs-lookup"><span data-stu-id="54134-132">id</span></span>|<span data-ttu-id="54134-133">字符串</span><span class="sxs-lookup"><span data-stu-id="54134-133">String</span></span>|<span data-ttu-id="54134-134">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="54134-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="54134-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54134-135">createdDateTime</span></span>|<span data-ttu-id="54134-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54134-136">DateTimeOffset</span></span>|<span data-ttu-id="54134-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="54134-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="54134-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54134-138">modifiedDateTime</span></span>|<span data-ttu-id="54134-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54134-139">DateTimeOffset</span></span>|<span data-ttu-id="54134-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="54134-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="54134-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54134-141">lastModifiedDateTime</span></span>|<span data-ttu-id="54134-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54134-142">DateTimeOffset</span></span>|<span data-ttu-id="54134-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="54134-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="54134-144">displayName</span><span class="sxs-lookup"><span data-stu-id="54134-144">displayName</span></span>|<span data-ttu-id="54134-145">String</span><span class="sxs-lookup"><span data-stu-id="54134-145">String</span></span>|<span data-ttu-id="54134-146">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="54134-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="54134-147">说明</span><span class="sxs-lookup"><span data-stu-id="54134-147">description</span></span>|<span data-ttu-id="54134-148">字符串</span><span class="sxs-lookup"><span data-stu-id="54134-148">String</span></span>|<span data-ttu-id="54134-149">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="54134-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="54134-150">title</span><span class="sxs-lookup"><span data-stu-id="54134-150">title</span></span>|<span data-ttu-id="54134-151">String</span><span class="sxs-lookup"><span data-stu-id="54134-151">String</span></span>|<span data-ttu-id="54134-152">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="54134-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="54134-153">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="54134-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="54134-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="54134-154">bodyText</span></span>|<span data-ttu-id="54134-155">String</span><span class="sxs-lookup"><span data-stu-id="54134-155">String</span></span>|<span data-ttu-id="54134-156">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="54134-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="54134-157">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="54134-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="54134-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="54134-158">acceptanceStatement</span></span>|<span data-ttu-id="54134-159">String</span><span class="sxs-lookup"><span data-stu-id="54134-159">String</span></span>|<span data-ttu-id="54134-160">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="54134-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="54134-161">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="54134-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="54134-162">version</span><span class="sxs-lookup"><span data-stu-id="54134-162">version</span></span>|<span data-ttu-id="54134-163">Int32</span><span class="sxs-lookup"><span data-stu-id="54134-163">Int32</span></span>|<span data-ttu-id="54134-164">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="54134-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="54134-165">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="54134-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="54134-166">响应</span><span class="sxs-lookup"><span data-stu-id="54134-166">Response</span></span>
<span data-ttu-id="54134-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54134-167">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54134-168">示例</span><span class="sxs-lookup"><span data-stu-id="54134-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="54134-169">请求</span><span class="sxs-lookup"><span data-stu-id="54134-169">Request</span></span>
<span data-ttu-id="54134-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54134-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="54134-171">响应</span><span class="sxs-lookup"><span data-stu-id="54134-171">Response</span></span>
<span data-ttu-id="54134-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54134-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

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
  "version": 7
}
```





