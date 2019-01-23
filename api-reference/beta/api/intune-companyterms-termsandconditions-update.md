---
title: 更新 termsAndConditions
description: 更新 termsAndConditions 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3eca58812eb4032113e968ad054a7a11bf110b81
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409487"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="9a5f6-103">更新 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="9a5f6-103">Update termsAndConditions</span></span>

> <span data-ttu-id="9a5f6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a5f6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a5f6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a5f6-107">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-107">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a5f6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a5f6-108">Prerequisites</span></span>
<span data-ttu-id="9a5f6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a5f6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a5f6-111">Permission type</span></span>|<span data-ttu-id="9a5f6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a5f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a5f6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a5f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a5f6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a5f6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a5f6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a5f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a5f6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-116">Not supported.</span></span>|
|<span data-ttu-id="9a5f6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a5f6-117">Application</span></span>|<span data-ttu-id="9a5f6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a5f6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a5f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="9a5f6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a5f6-120">Request headers</span></span>
|<span data-ttu-id="9a5f6-121">标头</span><span class="sxs-lookup"><span data-stu-id="9a5f6-121">Header</span></span>|<span data-ttu-id="9a5f6-122">值</span><span class="sxs-lookup"><span data-stu-id="9a5f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a5f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a5f6-123">Authorization</span></span>|<span data-ttu-id="9a5f6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a5f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a5f6-125">Accept</span></span>|<span data-ttu-id="9a5f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a5f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a5f6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a5f6-127">Request body</span></span>
<span data-ttu-id="9a5f6-128">在请求正文中，提供 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-128">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="9a5f6-129">下表显示创建 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-129">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="9a5f6-130">属性</span><span class="sxs-lookup"><span data-stu-id="9a5f6-130">Property</span></span>|<span data-ttu-id="9a5f6-131">类型</span><span class="sxs-lookup"><span data-stu-id="9a5f6-131">Type</span></span>|<span data-ttu-id="9a5f6-132">说明</span><span class="sxs-lookup"><span data-stu-id="9a5f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a5f6-133">id</span><span class="sxs-lookup"><span data-stu-id="9a5f6-133">id</span></span>|<span data-ttu-id="9a5f6-134">String</span><span class="sxs-lookup"><span data-stu-id="9a5f6-134">String</span></span>|<span data-ttu-id="9a5f6-135">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="9a5f6-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a5f6-136">createdDateTime</span></span>|<span data-ttu-id="9a5f6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a5f6-137">DateTimeOffset</span></span>|<span data-ttu-id="9a5f6-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="9a5f6-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a5f6-139">modifiedDateTime</span></span>|<span data-ttu-id="9a5f6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a5f6-140">DateTimeOffset</span></span>|<span data-ttu-id="9a5f6-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9a5f6-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a5f6-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9a5f6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a5f6-143">DateTimeOffset</span></span>|<span data-ttu-id="9a5f6-144">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9a5f6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="9a5f6-145">displayName</span></span>|<span data-ttu-id="9a5f6-146">String</span><span class="sxs-lookup"><span data-stu-id="9a5f6-146">String</span></span>|<span data-ttu-id="9a5f6-147">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="9a5f6-148">说明</span><span class="sxs-lookup"><span data-stu-id="9a5f6-148">description</span></span>|<span data-ttu-id="9a5f6-149">String</span><span class="sxs-lookup"><span data-stu-id="9a5f6-149">String</span></span>|<span data-ttu-id="9a5f6-150">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="9a5f6-151">title</span><span class="sxs-lookup"><span data-stu-id="9a5f6-151">title</span></span>|<span data-ttu-id="9a5f6-152">String</span><span class="sxs-lookup"><span data-stu-id="9a5f6-152">String</span></span>|<span data-ttu-id="9a5f6-153">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="9a5f6-154">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9a5f6-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="9a5f6-155">bodyText</span></span>|<span data-ttu-id="9a5f6-156">String</span><span class="sxs-lookup"><span data-stu-id="9a5f6-156">String</span></span>|<span data-ttu-id="9a5f6-157">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="9a5f6-158">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9a5f6-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="9a5f6-159">acceptanceStatement</span></span>|<span data-ttu-id="9a5f6-160">String</span><span class="sxs-lookup"><span data-stu-id="9a5f6-160">String</span></span>|<span data-ttu-id="9a5f6-161">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="9a5f6-162">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9a5f6-163">version</span><span class="sxs-lookup"><span data-stu-id="9a5f6-163">version</span></span>|<span data-ttu-id="9a5f6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9a5f6-164">Int32</span></span>|<span data-ttu-id="9a5f6-165">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="9a5f6-166">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="9a5f6-167">响应</span><span class="sxs-lookup"><span data-stu-id="9a5f6-167">Response</span></span>
<span data-ttu-id="9a5f6-168">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-168">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a5f6-169">示例</span><span class="sxs-lookup"><span data-stu-id="9a5f6-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a5f6-170">请求</span><span class="sxs-lookup"><span data-stu-id="9a5f6-170">Request</span></span>
<span data-ttu-id="9a5f6-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a5f6-172">响应</span><span class="sxs-lookup"><span data-stu-id="9a5f6-172">Response</span></span>
<span data-ttu-id="9a5f6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a5f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




