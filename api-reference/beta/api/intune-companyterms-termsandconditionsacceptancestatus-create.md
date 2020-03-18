---
title: 创建 termsAndConditionsAcceptanceStatus
description: 创建新的 termsAndConditionsAcceptanceStatus 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 755fd3e3c518ca0b30f660bdd7275e09f5ab9ce4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760142"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="4387a-103">创建 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="4387a-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="4387a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4387a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4387a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4387a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4387a-106">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4387a-106">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4387a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4387a-107">Prerequisites</span></span>
<span data-ttu-id="4387a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4387a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4387a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4387a-110">Permission type</span></span>|<span data-ttu-id="4387a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4387a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4387a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4387a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4387a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4387a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4387a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4387a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4387a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4387a-115">Not supported.</span></span>|
|<span data-ttu-id="4387a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4387a-116">Application</span></span>|<span data-ttu-id="4387a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4387a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4387a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4387a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4387a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4387a-119">Request headers</span></span>
|<span data-ttu-id="4387a-120">标头</span><span class="sxs-lookup"><span data-stu-id="4387a-120">Header</span></span>|<span data-ttu-id="4387a-121">值</span><span class="sxs-lookup"><span data-stu-id="4387a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4387a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4387a-122">Authorization</span></span>|<span data-ttu-id="4387a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4387a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4387a-124">接受</span><span class="sxs-lookup"><span data-stu-id="4387a-124">Accept</span></span>|<span data-ttu-id="4387a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4387a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4387a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4387a-126">Request body</span></span>
<span data-ttu-id="4387a-127">在请求正文中，提供 termsAndConditionsAcceptanceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4387a-127">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="4387a-128">下表显示创建 termsAndConditionsAcceptanceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4387a-128">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="4387a-129">属性</span><span class="sxs-lookup"><span data-stu-id="4387a-129">Property</span></span>|<span data-ttu-id="4387a-130">类型</span><span class="sxs-lookup"><span data-stu-id="4387a-130">Type</span></span>|<span data-ttu-id="4387a-131">说明</span><span class="sxs-lookup"><span data-stu-id="4387a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4387a-132">id</span><span class="sxs-lookup"><span data-stu-id="4387a-132">id</span></span>|<span data-ttu-id="4387a-133">String</span><span class="sxs-lookup"><span data-stu-id="4387a-133">String</span></span>|<span data-ttu-id="4387a-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4387a-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="4387a-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4387a-135">userDisplayName</span></span>|<span data-ttu-id="4387a-136">String</span><span class="sxs-lookup"><span data-stu-id="4387a-136">String</span></span>|<span data-ttu-id="4387a-137">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4387a-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="4387a-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="4387a-138">acceptedVersion</span></span>|<span data-ttu-id="4387a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4387a-139">Int32</span></span>|<span data-ttu-id="4387a-140">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="4387a-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="4387a-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="4387a-141">acceptedDateTime</span></span>|<span data-ttu-id="4387a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4387a-142">DateTimeOffset</span></span>|<span data-ttu-id="4387a-143">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4387a-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="4387a-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4387a-144">userPrincipalName</span></span>|<span data-ttu-id="4387a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="4387a-145">String</span></span>|<span data-ttu-id="4387a-146">接受术语的用户的 userPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4387a-146">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="4387a-147">响应</span><span class="sxs-lookup"><span data-stu-id="4387a-147">Response</span></span>
<span data-ttu-id="4387a-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4387a-148">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4387a-149">示例</span><span class="sxs-lookup"><span data-stu-id="4387a-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="4387a-150">请求</span><span class="sxs-lookup"><span data-stu-id="4387a-150">Request</span></span>
<span data-ttu-id="4387a-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4387a-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
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

### <a name="response"></a><span data-ttu-id="4387a-152">响应</span><span class="sxs-lookup"><span data-stu-id="4387a-152">Response</span></span>
<span data-ttu-id="4387a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4387a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




