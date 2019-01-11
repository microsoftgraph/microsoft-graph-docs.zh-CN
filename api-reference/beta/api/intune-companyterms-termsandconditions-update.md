---
title: 更新 termsAndConditions
description: 更新 termsAndConditions 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7617e58dcae72f4f69c08c5f4dfa8c373df8edd1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852808"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="6f50a-103">更新 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6f50a-103">Update termsAndConditions</span></span>

> <span data-ttu-id="6f50a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6f50a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f50a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f50a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f50a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f50a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f50a-107">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6f50a-107">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f50a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f50a-108">Prerequisites</span></span>
<span data-ttu-id="6f50a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6f50a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f50a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f50a-111">Permission type</span></span>|<span data-ttu-id="6f50a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f50a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f50a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f50a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f50a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f50a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f50a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f50a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f50a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f50a-116">Not supported.</span></span>|
|<span data-ttu-id="6f50a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f50a-117">Application</span></span>|<span data-ttu-id="6f50a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f50a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f50a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f50a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="6f50a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f50a-120">Request headers</span></span>
|<span data-ttu-id="6f50a-121">标头</span><span class="sxs-lookup"><span data-stu-id="6f50a-121">Header</span></span>|<span data-ttu-id="6f50a-122">值</span><span class="sxs-lookup"><span data-stu-id="6f50a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f50a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f50a-123">Authorization</span></span>|<span data-ttu-id="6f50a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f50a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f50a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f50a-125">Accept</span></span>|<span data-ttu-id="6f50a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f50a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f50a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f50a-127">Request body</span></span>
<span data-ttu-id="6f50a-128">在请求正文中，提供 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f50a-128">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="6f50a-129">下表显示创建 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6f50a-129">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="6f50a-130">属性</span><span class="sxs-lookup"><span data-stu-id="6f50a-130">Property</span></span>|<span data-ttu-id="6f50a-131">类型</span><span class="sxs-lookup"><span data-stu-id="6f50a-131">Type</span></span>|<span data-ttu-id="6f50a-132">说明</span><span class="sxs-lookup"><span data-stu-id="6f50a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f50a-133">id</span><span class="sxs-lookup"><span data-stu-id="6f50a-133">id</span></span>|<span data-ttu-id="6f50a-134">String</span><span class="sxs-lookup"><span data-stu-id="6f50a-134">String</span></span>|<span data-ttu-id="6f50a-135">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6f50a-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="6f50a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f50a-136">createdDateTime</span></span>|<span data-ttu-id="6f50a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f50a-137">DateTimeOffset</span></span>|<span data-ttu-id="6f50a-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6f50a-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="6f50a-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f50a-139">modifiedDateTime</span></span>|<span data-ttu-id="6f50a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f50a-140">DateTimeOffset</span></span>|<span data-ttu-id="6f50a-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6f50a-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6f50a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f50a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="6f50a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f50a-143">DateTimeOffset</span></span>|<span data-ttu-id="6f50a-144">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6f50a-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6f50a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6f50a-145">displayName</span></span>|<span data-ttu-id="6f50a-146">String</span><span class="sxs-lookup"><span data-stu-id="6f50a-146">String</span></span>|<span data-ttu-id="6f50a-147">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="6f50a-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="6f50a-148">说明</span><span class="sxs-lookup"><span data-stu-id="6f50a-148">description</span></span>|<span data-ttu-id="6f50a-149">String</span><span class="sxs-lookup"><span data-stu-id="6f50a-149">String</span></span>|<span data-ttu-id="6f50a-150">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="6f50a-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="6f50a-151">title</span><span class="sxs-lookup"><span data-stu-id="6f50a-151">title</span></span>|<span data-ttu-id="6f50a-152">String</span><span class="sxs-lookup"><span data-stu-id="6f50a-152">String</span></span>|<span data-ttu-id="6f50a-153">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="6f50a-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="6f50a-154">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6f50a-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6f50a-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="6f50a-155">bodyText</span></span>|<span data-ttu-id="6f50a-156">String</span><span class="sxs-lookup"><span data-stu-id="6f50a-156">String</span></span>|<span data-ttu-id="6f50a-157">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="6f50a-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="6f50a-158">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6f50a-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6f50a-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="6f50a-159">acceptanceStatement</span></span>|<span data-ttu-id="6f50a-160">String</span><span class="sxs-lookup"><span data-stu-id="6f50a-160">String</span></span>|<span data-ttu-id="6f50a-161">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="6f50a-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="6f50a-162">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6f50a-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6f50a-163">version</span><span class="sxs-lookup"><span data-stu-id="6f50a-163">version</span></span>|<span data-ttu-id="6f50a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6f50a-164">Int32</span></span>|<span data-ttu-id="6f50a-165">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="6f50a-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="6f50a-166">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="6f50a-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6f50a-167">响应</span><span class="sxs-lookup"><span data-stu-id="6f50a-167">Response</span></span>
<span data-ttu-id="6f50a-168">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f50a-168">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f50a-169">示例</span><span class="sxs-lookup"><span data-stu-id="6f50a-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f50a-170">请求</span><span class="sxs-lookup"><span data-stu-id="6f50a-170">Request</span></span>
<span data-ttu-id="6f50a-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f50a-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 280

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="6f50a-172">响应</span><span class="sxs-lookup"><span data-stu-id="6f50a-172">Response</span></span>
<span data-ttu-id="6f50a-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f50a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





