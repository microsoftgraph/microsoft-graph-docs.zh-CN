---
title: 更新 termsAndConditionsAcceptanceStatus
description: 更新 termsAndConditionsAcceptanceStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6cbb67f852a89322cae6455b13d97b80872bbf9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960704"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="13531-103">更新 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="13531-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="13531-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13531-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13531-105">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13531-105">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13531-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="13531-106">Prerequisites</span></span>
<span data-ttu-id="13531-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13531-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="13531-109">Permission type</span></span>|<span data-ttu-id="13531-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="13531-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13531-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13531-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13531-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13531-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="13531-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13531-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13531-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="13531-114">Not supported.</span></span>|
|<span data-ttu-id="13531-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="13531-115">Application</span></span>|<span data-ttu-id="13531-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="13531-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13531-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13531-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="13531-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="13531-118">Request headers</span></span>
|<span data-ttu-id="13531-119">标头</span><span class="sxs-lookup"><span data-stu-id="13531-119">Header</span></span>|<span data-ttu-id="13531-120">值</span><span class="sxs-lookup"><span data-stu-id="13531-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13531-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="13531-121">Authorization</span></span>|<span data-ttu-id="13531-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="13531-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13531-123">接受</span><span class="sxs-lookup"><span data-stu-id="13531-123">Accept</span></span>|<span data-ttu-id="13531-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13531-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13531-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="13531-125">Request body</span></span>
<span data-ttu-id="13531-126">在请求正文中，提供 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13531-126">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="13531-127">下表显示创建 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="13531-127">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="13531-128">属性</span><span class="sxs-lookup"><span data-stu-id="13531-128">Property</span></span>|<span data-ttu-id="13531-129">类型</span><span class="sxs-lookup"><span data-stu-id="13531-129">Type</span></span>|<span data-ttu-id="13531-130">说明</span><span class="sxs-lookup"><span data-stu-id="13531-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13531-131">id</span><span class="sxs-lookup"><span data-stu-id="13531-131">id</span></span>|<span data-ttu-id="13531-132">String</span><span class="sxs-lookup"><span data-stu-id="13531-132">String</span></span>|<span data-ttu-id="13531-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="13531-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="13531-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="13531-134">userDisplayName</span></span>|<span data-ttu-id="13531-135">String</span><span class="sxs-lookup"><span data-stu-id="13531-135">String</span></span>|<span data-ttu-id="13531-136">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="13531-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="13531-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="13531-137">acceptedVersion</span></span>|<span data-ttu-id="13531-138">Int32</span><span class="sxs-lookup"><span data-stu-id="13531-138">Int32</span></span>|<span data-ttu-id="13531-139">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="13531-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="13531-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="13531-140">acceptedDateTime</span></span>|<span data-ttu-id="13531-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13531-141">DateTimeOffset</span></span>|<span data-ttu-id="13531-142">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="13531-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="13531-143">响应</span><span class="sxs-lookup"><span data-stu-id="13531-143">Response</span></span>
<span data-ttu-id="13531-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13531-144">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13531-145">示例</span><span class="sxs-lookup"><span data-stu-id="13531-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="13531-146">请求</span><span class="sxs-lookup"><span data-stu-id="13531-146">Request</span></span>
<span data-ttu-id="13531-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13531-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="13531-148">响应</span><span class="sxs-lookup"><span data-stu-id="13531-148">Response</span></span>
<span data-ttu-id="13531-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13531-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



