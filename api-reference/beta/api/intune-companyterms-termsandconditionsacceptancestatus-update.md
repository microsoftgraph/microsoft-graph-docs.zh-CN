---
title: 更新 termsAndConditionsAcceptanceStatus
description: 更新 termsAndConditionsAcceptanceStatus 对象的属性。
ms.openlocfilehash: 46e7c69be6dc0ac410162b491b51c6f81a65fce5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048048"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="bc831-103">更新 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="bc831-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="bc831-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc831-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc831-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc831-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc831-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bc831-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc831-107">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc831-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc831-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc831-108">Prerequisites</span></span>
<span data-ttu-id="bc831-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bc831-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc831-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc831-111">Permission type</span></span>|<span data-ttu-id="bc831-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc831-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc831-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc831-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc831-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc831-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bc831-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc831-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc831-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc831-116">Not supported.</span></span>|
|<span data-ttu-id="bc831-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc831-117">Application</span></span>|<span data-ttu-id="bc831-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc831-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc831-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc831-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="bc831-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc831-120">Request headers</span></span>
|<span data-ttu-id="bc831-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc831-121">Header</span></span>|<span data-ttu-id="bc831-122">值</span><span class="sxs-lookup"><span data-stu-id="bc831-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc831-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc831-123">Authorization</span></span>|<span data-ttu-id="bc831-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc831-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc831-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc831-125">Accept</span></span>|<span data-ttu-id="bc831-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc831-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc831-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc831-127">Request body</span></span>
<span data-ttu-id="bc831-128">在请求正文中，提供 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc831-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="bc831-129">下表显示创建 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bc831-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="bc831-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc831-130">Property</span></span>|<span data-ttu-id="bc831-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc831-131">Type</span></span>|<span data-ttu-id="bc831-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc831-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc831-133">id</span><span class="sxs-lookup"><span data-stu-id="bc831-133">id</span></span>|<span data-ttu-id="bc831-134">String</span><span class="sxs-lookup"><span data-stu-id="bc831-134">String</span></span>|<span data-ttu-id="bc831-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bc831-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="bc831-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bc831-136">userDisplayName</span></span>|<span data-ttu-id="bc831-137">String</span><span class="sxs-lookup"><span data-stu-id="bc831-137">String</span></span>|<span data-ttu-id="bc831-138">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bc831-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="bc831-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="bc831-139">acceptedVersion</span></span>|<span data-ttu-id="bc831-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bc831-140">Int32</span></span>|<span data-ttu-id="bc831-141">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="bc831-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="bc831-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc831-142">acceptedDateTime</span></span>|<span data-ttu-id="bc831-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc831-143">DateTimeOffset</span></span>|<span data-ttu-id="bc831-144">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc831-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="bc831-145">响应</span><span class="sxs-lookup"><span data-stu-id="bc831-145">Response</span></span>
<span data-ttu-id="bc831-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc831-146">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc831-147">示例</span><span class="sxs-lookup"><span data-stu-id="bc831-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc831-148">请求</span><span class="sxs-lookup"><span data-stu-id="bc831-148">Request</span></span>
<span data-ttu-id="bc831-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc831-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 138

{
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bc831-150">响应</span><span class="sxs-lookup"><span data-stu-id="bc831-150">Response</span></span>
<span data-ttu-id="bc831-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc831-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





