---
title: 更新 termsAndConditions
description: 更新 termsAndConditions 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fc8442c1e15b515380d98d3ba91248c4fe277a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923416"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="ba931-103">更新 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ba931-103">Update termsAndConditions</span></span>

> <span data-ttu-id="ba931-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ba931-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba931-105">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ba931-105">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba931-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ba931-106">Prerequisites</span></span>
<span data-ttu-id="ba931-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ba931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba931-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba931-109">Permission type</span></span>|<span data-ttu-id="ba931-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ba931-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba931-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba931-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba931-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba931-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ba931-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba931-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba931-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba931-114">Not supported.</span></span>|
|<span data-ttu-id="ba931-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba931-115">Application</span></span>|<span data-ttu-id="ba931-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba931-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba931-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba931-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="ba931-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba931-118">Request headers</span></span>
|<span data-ttu-id="ba931-119">标头</span><span class="sxs-lookup"><span data-stu-id="ba931-119">Header</span></span>|<span data-ttu-id="ba931-120">值</span><span class="sxs-lookup"><span data-stu-id="ba931-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba931-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba931-121">Authorization</span></span>|<span data-ttu-id="ba931-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ba931-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba931-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ba931-123">Accept</span></span>|<span data-ttu-id="ba931-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ba931-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba931-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba931-125">Request body</span></span>
<span data-ttu-id="ba931-126">在请求正文中，提供 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba931-126">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="ba931-127">下表显示创建 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ba931-127">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="ba931-128">属性</span><span class="sxs-lookup"><span data-stu-id="ba931-128">Property</span></span>|<span data-ttu-id="ba931-129">类型</span><span class="sxs-lookup"><span data-stu-id="ba931-129">Type</span></span>|<span data-ttu-id="ba931-130">说明</span><span class="sxs-lookup"><span data-stu-id="ba931-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba931-131">id</span><span class="sxs-lookup"><span data-stu-id="ba931-131">id</span></span>|<span data-ttu-id="ba931-132">String</span><span class="sxs-lookup"><span data-stu-id="ba931-132">String</span></span>|<span data-ttu-id="ba931-133">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ba931-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="ba931-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba931-134">createdDateTime</span></span>|<span data-ttu-id="ba931-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba931-135">DateTimeOffset</span></span>|<span data-ttu-id="ba931-136">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ba931-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="ba931-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba931-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ba931-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba931-138">DateTimeOffset</span></span>|<span data-ttu-id="ba931-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ba931-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ba931-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ba931-140">displayName</span></span>|<span data-ttu-id="ba931-141">String</span><span class="sxs-lookup"><span data-stu-id="ba931-141">String</span></span>|<span data-ttu-id="ba931-142">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="ba931-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="ba931-143">说明</span><span class="sxs-lookup"><span data-stu-id="ba931-143">description</span></span>|<span data-ttu-id="ba931-144">String</span><span class="sxs-lookup"><span data-stu-id="ba931-144">String</span></span>|<span data-ttu-id="ba931-145">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="ba931-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="ba931-146">title</span><span class="sxs-lookup"><span data-stu-id="ba931-146">title</span></span>|<span data-ttu-id="ba931-147">String</span><span class="sxs-lookup"><span data-stu-id="ba931-147">String</span></span>|<span data-ttu-id="ba931-148">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="ba931-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="ba931-149">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="ba931-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ba931-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="ba931-150">bodyText</span></span>|<span data-ttu-id="ba931-151">String</span><span class="sxs-lookup"><span data-stu-id="ba931-151">String</span></span>|<span data-ttu-id="ba931-152">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="ba931-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="ba931-153">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="ba931-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ba931-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="ba931-154">acceptanceStatement</span></span>|<span data-ttu-id="ba931-155">String</span><span class="sxs-lookup"><span data-stu-id="ba931-155">String</span></span>|<span data-ttu-id="ba931-156">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="ba931-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="ba931-157">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="ba931-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ba931-158">version</span><span class="sxs-lookup"><span data-stu-id="ba931-158">version</span></span>|<span data-ttu-id="ba931-159">Int32</span><span class="sxs-lookup"><span data-stu-id="ba931-159">Int32</span></span>|<span data-ttu-id="ba931-160">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="ba931-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="ba931-161">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="ba931-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="ba931-162">响应</span><span class="sxs-lookup"><span data-stu-id="ba931-162">Response</span></span>
<span data-ttu-id="ba931-163">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba931-163">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba931-164">示例</span><span class="sxs-lookup"><span data-stu-id="ba931-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba931-165">请求</span><span class="sxs-lookup"><span data-stu-id="ba931-165">Request</span></span>
<span data-ttu-id="ba931-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba931-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
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

### <a name="response"></a><span data-ttu-id="ba931-167">响应</span><span class="sxs-lookup"><span data-stu-id="ba931-167">Response</span></span>
<span data-ttu-id="ba931-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba931-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



