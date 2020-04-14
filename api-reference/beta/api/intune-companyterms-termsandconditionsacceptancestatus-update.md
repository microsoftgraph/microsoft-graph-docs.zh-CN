---
title: 更新 termsAndConditionsAcceptanceStatus
description: 更新 termsAndConditionsAcceptanceStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 23d368e6b7389c7a2e297fd9b5886b11ad66e3dd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436470"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="fa5e3-103">更新 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa5e3-103">Update termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="fa5e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa5e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa5e3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa5e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa5e3-107">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa5e3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa5e3-108">Prerequisites</span></span>
<span data-ttu-id="fa5e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa5e3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa5e3-111">Permission type</span></span>|<span data-ttu-id="fa5e3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa5e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa5e3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa5e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa5e3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa5e3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa5e3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa5e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa5e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-116">Not supported.</span></span>|
|<span data-ttu-id="fa5e3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa5e3-117">Application</span></span>|<span data-ttu-id="fa5e3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa5e3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa5e3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa5e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="fa5e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa5e3-120">Request headers</span></span>
|<span data-ttu-id="fa5e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="fa5e3-121">Header</span></span>|<span data-ttu-id="fa5e3-122">值</span><span class="sxs-lookup"><span data-stu-id="fa5e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa5e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa5e3-123">Authorization</span></span>|<span data-ttu-id="fa5e3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa5e3-125">接受</span><span class="sxs-lookup"><span data-stu-id="fa5e3-125">Accept</span></span>|<span data-ttu-id="fa5e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa5e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa5e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa5e3-127">Request body</span></span>
<span data-ttu-id="fa5e3-128">在请求正文中，提供 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="fa5e3-129">下表显示创建 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="fa5e3-130">属性</span><span class="sxs-lookup"><span data-stu-id="fa5e3-130">Property</span></span>|<span data-ttu-id="fa5e3-131">类型</span><span class="sxs-lookup"><span data-stu-id="fa5e3-131">Type</span></span>|<span data-ttu-id="fa5e3-132">说明</span><span class="sxs-lookup"><span data-stu-id="fa5e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa5e3-133">id</span><span class="sxs-lookup"><span data-stu-id="fa5e3-133">id</span></span>|<span data-ttu-id="fa5e3-134">String</span><span class="sxs-lookup"><span data-stu-id="fa5e3-134">String</span></span>|<span data-ttu-id="fa5e3-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fa5e3-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fa5e3-136">userDisplayName</span></span>|<span data-ttu-id="fa5e3-137">String</span><span class="sxs-lookup"><span data-stu-id="fa5e3-137">String</span></span>|<span data-ttu-id="fa5e3-138">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="fa5e3-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="fa5e3-139">acceptedVersion</span></span>|<span data-ttu-id="fa5e3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fa5e3-140">Int32</span></span>|<span data-ttu-id="fa5e3-141">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="fa5e3-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa5e3-142">acceptedDateTime</span></span>|<span data-ttu-id="fa5e3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa5e3-143">DateTimeOffset</span></span>|<span data-ttu-id="fa5e3-144">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-144">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="fa5e3-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fa5e3-145">userPrincipalName</span></span>|<span data-ttu-id="fa5e3-146">字符串</span><span class="sxs-lookup"><span data-stu-id="fa5e3-146">String</span></span>|<span data-ttu-id="fa5e3-147">接受术语的用户的 userPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-147">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="fa5e3-148">响应</span><span class="sxs-lookup"><span data-stu-id="fa5e3-148">Response</span></span>
<span data-ttu-id="fa5e3-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-149">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa5e3-150">示例</span><span class="sxs-lookup"><span data-stu-id="fa5e3-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa5e3-151">请求</span><span class="sxs-lookup"><span data-stu-id="fa5e3-151">Request</span></span>
<span data-ttu-id="fa5e3-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="fa5e3-153">响应</span><span class="sxs-lookup"><span data-stu-id="fa5e3-153">Response</span></span>
<span data-ttu-id="fa5e3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa5e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



