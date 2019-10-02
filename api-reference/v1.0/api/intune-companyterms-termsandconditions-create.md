---
title: 创建 termsAndConditions
description: 创建新的 termsAndConditions 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c655f712e9fbbf09342ac77f978de02b0ba5720
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357841"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="c1714-103">创建 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="c1714-103">Create termsAndConditions</span></span>

> <span data-ttu-id="c1714-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1714-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1714-105">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1714-105">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1714-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1714-106">Prerequisites</span></span>
<span data-ttu-id="c1714-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1714-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1714-109">Permission type</span></span>|<span data-ttu-id="c1714-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1714-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1714-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1714-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1714-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1714-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1714-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1714-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1714-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1714-114">Not supported.</span></span>|
|<span data-ttu-id="c1714-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1714-115">Application</span></span>|<span data-ttu-id="c1714-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1714-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1714-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1714-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="c1714-118">请求头</span><span class="sxs-lookup"><span data-stu-id="c1714-118">Request headers</span></span>
|<span data-ttu-id="c1714-119">标头</span><span class="sxs-lookup"><span data-stu-id="c1714-119">Header</span></span>|<span data-ttu-id="c1714-120">值</span><span class="sxs-lookup"><span data-stu-id="c1714-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1714-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1714-121">Authorization</span></span>|<span data-ttu-id="c1714-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1714-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1714-123">接受</span><span class="sxs-lookup"><span data-stu-id="c1714-123">Accept</span></span>|<span data-ttu-id="c1714-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1714-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1714-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1714-125">Request body</span></span>
<span data-ttu-id="c1714-126">在请求正文中，提供 termsAndConditions 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1714-126">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="c1714-127">下表显示创建 termsAndConditions 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1714-127">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="c1714-128">属性</span><span class="sxs-lookup"><span data-stu-id="c1714-128">Property</span></span>|<span data-ttu-id="c1714-129">类型</span><span class="sxs-lookup"><span data-stu-id="c1714-129">Type</span></span>|<span data-ttu-id="c1714-130">说明</span><span class="sxs-lookup"><span data-stu-id="c1714-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1714-131">id</span><span class="sxs-lookup"><span data-stu-id="c1714-131">id</span></span>|<span data-ttu-id="c1714-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c1714-132">String</span></span>|<span data-ttu-id="c1714-133">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c1714-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="c1714-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1714-134">createdDateTime</span></span>|<span data-ttu-id="c1714-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1714-135">DateTimeOffset</span></span>|<span data-ttu-id="c1714-136">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c1714-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="c1714-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1714-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c1714-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1714-138">DateTimeOffset</span></span>|<span data-ttu-id="c1714-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c1714-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c1714-140">displayName</span><span class="sxs-lookup"><span data-stu-id="c1714-140">displayName</span></span>|<span data-ttu-id="c1714-141">String</span><span class="sxs-lookup"><span data-stu-id="c1714-141">String</span></span>|<span data-ttu-id="c1714-142">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="c1714-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="c1714-143">说明</span><span class="sxs-lookup"><span data-stu-id="c1714-143">description</span></span>|<span data-ttu-id="c1714-144">字符串</span><span class="sxs-lookup"><span data-stu-id="c1714-144">String</span></span>|<span data-ttu-id="c1714-145">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="c1714-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="c1714-146">title</span><span class="sxs-lookup"><span data-stu-id="c1714-146">title</span></span>|<span data-ttu-id="c1714-147">String</span><span class="sxs-lookup"><span data-stu-id="c1714-147">String</span></span>|<span data-ttu-id="c1714-148">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="c1714-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="c1714-149">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="c1714-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="c1714-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="c1714-150">bodyText</span></span>|<span data-ttu-id="c1714-151">String</span><span class="sxs-lookup"><span data-stu-id="c1714-151">String</span></span>|<span data-ttu-id="c1714-152">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="c1714-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="c1714-153">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="c1714-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="c1714-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="c1714-154">acceptanceStatement</span></span>|<span data-ttu-id="c1714-155">String</span><span class="sxs-lookup"><span data-stu-id="c1714-155">String</span></span>|<span data-ttu-id="c1714-156">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="c1714-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="c1714-157">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="c1714-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="c1714-158">version</span><span class="sxs-lookup"><span data-stu-id="c1714-158">version</span></span>|<span data-ttu-id="c1714-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c1714-159">Int32</span></span>|<span data-ttu-id="c1714-160">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="c1714-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="c1714-161">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="c1714-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="c1714-162">响应</span><span class="sxs-lookup"><span data-stu-id="c1714-162">Response</span></span>
<span data-ttu-id="c1714-163">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1714-163">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1714-164">示例</span><span class="sxs-lookup"><span data-stu-id="c1714-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1714-165">请求</span><span class="sxs-lookup"><span data-stu-id="c1714-165">Request</span></span>
<span data-ttu-id="c1714-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1714-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1714-167">响应</span><span class="sxs-lookup"><span data-stu-id="c1714-167">Response</span></span>
<span data-ttu-id="c1714-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1714-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




