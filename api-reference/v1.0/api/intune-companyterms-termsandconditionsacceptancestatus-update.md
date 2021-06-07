---
title: 更新 termsAndConditionsAcceptanceStatus
description: 更新 termsAndConditionsAcceptanceStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4acda8ce8c89ec73fbe6808ba2a6242eb27acde7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756720"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="3b9ef-103">更新 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="3b9ef-103">Update termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="3b9ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b9ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b9ef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b9ef-106">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b9ef-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b9ef-107">Prerequisites</span></span>
<span data-ttu-id="3b9ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b9ef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b9ef-110">Permission type</span></span>|<span data-ttu-id="3b9ef-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b9ef-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b9ef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b9ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b9ef-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b9ef-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3b9ef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b9ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b9ef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-115">Not supported.</span></span>|
|<span data-ttu-id="3b9ef-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b9ef-116">Application</span></span>|<span data-ttu-id="3b9ef-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b9ef-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b9ef-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b9ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="3b9ef-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b9ef-119">Request headers</span></span>
|<span data-ttu-id="3b9ef-120">标头</span><span class="sxs-lookup"><span data-stu-id="3b9ef-120">Header</span></span>|<span data-ttu-id="3b9ef-121">值</span><span class="sxs-lookup"><span data-stu-id="3b9ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b9ef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b9ef-122">Authorization</span></span>|<span data-ttu-id="3b9ef-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b9ef-124">接受</span><span class="sxs-lookup"><span data-stu-id="3b9ef-124">Accept</span></span>|<span data-ttu-id="3b9ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b9ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b9ef-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b9ef-126">Request body</span></span>
<span data-ttu-id="3b9ef-127">在请求正文中，提供 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="3b9ef-128">下表显示创建 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="3b9ef-129">属性</span><span class="sxs-lookup"><span data-stu-id="3b9ef-129">Property</span></span>|<span data-ttu-id="3b9ef-130">类型</span><span class="sxs-lookup"><span data-stu-id="3b9ef-130">Type</span></span>|<span data-ttu-id="3b9ef-131">说明</span><span class="sxs-lookup"><span data-stu-id="3b9ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b9ef-132">id</span><span class="sxs-lookup"><span data-stu-id="3b9ef-132">id</span></span>|<span data-ttu-id="3b9ef-133">String</span><span class="sxs-lookup"><span data-stu-id="3b9ef-133">String</span></span>|<span data-ttu-id="3b9ef-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="3b9ef-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3b9ef-135">userDisplayName</span></span>|<span data-ttu-id="3b9ef-136">String</span><span class="sxs-lookup"><span data-stu-id="3b9ef-136">String</span></span>|<span data-ttu-id="3b9ef-137">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="3b9ef-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="3b9ef-138">acceptedVersion</span></span>|<span data-ttu-id="3b9ef-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3b9ef-139">Int32</span></span>|<span data-ttu-id="3b9ef-140">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="3b9ef-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b9ef-141">acceptedDateTime</span></span>|<span data-ttu-id="3b9ef-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b9ef-142">DateTimeOffset</span></span>|<span data-ttu-id="3b9ef-143">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="3b9ef-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b9ef-144">userPrincipalName</span></span>|<span data-ttu-id="3b9ef-145">String</span><span class="sxs-lookup"><span data-stu-id="3b9ef-145">String</span></span>|<span data-ttu-id="3b9ef-146">接受术语的用户的 userPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-146">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="3b9ef-147">响应</span><span class="sxs-lookup"><span data-stu-id="3b9ef-147">Response</span></span>
<span data-ttu-id="3b9ef-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-148">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b9ef-149">示例</span><span class="sxs-lookup"><span data-stu-id="3b9ef-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b9ef-150">请求</span><span class="sxs-lookup"><span data-stu-id="3b9ef-150">Request</span></span>
<span data-ttu-id="3b9ef-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
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

### <a name="response"></a><span data-ttu-id="3b9ef-152">响应</span><span class="sxs-lookup"><span data-stu-id="3b9ef-152">Response</span></span>
<span data-ttu-id="3b9ef-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b9ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




