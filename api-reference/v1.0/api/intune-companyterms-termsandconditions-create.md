---
title: 创建 termsAndConditions
description: 创建新的 termsAndConditions 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a278dc8cd621ae66e65e56eab081ab89de565d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442160"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="6177b-103">创建 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6177b-103">Create termsAndConditions</span></span>

<span data-ttu-id="6177b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6177b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6177b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6177b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6177b-106">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6177b-106">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6177b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6177b-107">Prerequisites</span></span>
<span data-ttu-id="6177b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6177b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6177b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6177b-110">Permission type</span></span>|<span data-ttu-id="6177b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6177b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6177b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6177b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6177b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6177b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6177b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6177b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6177b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6177b-115">Not supported.</span></span>|
|<span data-ttu-id="6177b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6177b-116">Application</span></span>|<span data-ttu-id="6177b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6177b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6177b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6177b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="6177b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6177b-119">Request headers</span></span>
|<span data-ttu-id="6177b-120">标头</span><span class="sxs-lookup"><span data-stu-id="6177b-120">Header</span></span>|<span data-ttu-id="6177b-121">值</span><span class="sxs-lookup"><span data-stu-id="6177b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6177b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6177b-122">Authorization</span></span>|<span data-ttu-id="6177b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6177b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6177b-124">接受</span><span class="sxs-lookup"><span data-stu-id="6177b-124">Accept</span></span>|<span data-ttu-id="6177b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6177b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6177b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6177b-126">Request body</span></span>
<span data-ttu-id="6177b-127">在请求正文中，提供 termsAndConditions 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6177b-127">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="6177b-128">下表显示创建 termsAndConditions 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6177b-128">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="6177b-129">属性</span><span class="sxs-lookup"><span data-stu-id="6177b-129">Property</span></span>|<span data-ttu-id="6177b-130">类型</span><span class="sxs-lookup"><span data-stu-id="6177b-130">Type</span></span>|<span data-ttu-id="6177b-131">说明</span><span class="sxs-lookup"><span data-stu-id="6177b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6177b-132">id</span><span class="sxs-lookup"><span data-stu-id="6177b-132">id</span></span>|<span data-ttu-id="6177b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6177b-133">String</span></span>|<span data-ttu-id="6177b-134">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6177b-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="6177b-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6177b-135">createdDateTime</span></span>|<span data-ttu-id="6177b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6177b-136">DateTimeOffset</span></span>|<span data-ttu-id="6177b-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6177b-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="6177b-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6177b-138">lastModifiedDateTime</span></span>|<span data-ttu-id="6177b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6177b-139">DateTimeOffset</span></span>|<span data-ttu-id="6177b-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6177b-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6177b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6177b-141">displayName</span></span>|<span data-ttu-id="6177b-142">String</span><span class="sxs-lookup"><span data-stu-id="6177b-142">String</span></span>|<span data-ttu-id="6177b-143">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="6177b-143">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="6177b-144">description</span><span class="sxs-lookup"><span data-stu-id="6177b-144">description</span></span>|<span data-ttu-id="6177b-145">字符串</span><span class="sxs-lookup"><span data-stu-id="6177b-145">String</span></span>|<span data-ttu-id="6177b-146">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="6177b-146">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="6177b-147">title</span><span class="sxs-lookup"><span data-stu-id="6177b-147">title</span></span>|<span data-ttu-id="6177b-148">String</span><span class="sxs-lookup"><span data-stu-id="6177b-148">String</span></span>|<span data-ttu-id="6177b-149">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="6177b-149">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="6177b-150">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6177b-150">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6177b-151">bodyText</span><span class="sxs-lookup"><span data-stu-id="6177b-151">bodyText</span></span>|<span data-ttu-id="6177b-152">String</span><span class="sxs-lookup"><span data-stu-id="6177b-152">String</span></span>|<span data-ttu-id="6177b-153">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="6177b-153">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="6177b-154">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6177b-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6177b-155">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="6177b-155">acceptanceStatement</span></span>|<span data-ttu-id="6177b-156">String</span><span class="sxs-lookup"><span data-stu-id="6177b-156">String</span></span>|<span data-ttu-id="6177b-157">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="6177b-157">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="6177b-158">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6177b-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6177b-159">version</span><span class="sxs-lookup"><span data-stu-id="6177b-159">version</span></span>|<span data-ttu-id="6177b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6177b-160">Int32</span></span>|<span data-ttu-id="6177b-161">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="6177b-161">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="6177b-162">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="6177b-162">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6177b-163">响应</span><span class="sxs-lookup"><span data-stu-id="6177b-163">Response</span></span>
<span data-ttu-id="6177b-164">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6177b-164">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6177b-165">示例</span><span class="sxs-lookup"><span data-stu-id="6177b-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="6177b-166">请求</span><span class="sxs-lookup"><span data-stu-id="6177b-166">Request</span></span>
<span data-ttu-id="6177b-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6177b-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
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

### <a name="response"></a><span data-ttu-id="6177b-168">响应</span><span class="sxs-lookup"><span data-stu-id="6177b-168">Response</span></span>
<span data-ttu-id="6177b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6177b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






