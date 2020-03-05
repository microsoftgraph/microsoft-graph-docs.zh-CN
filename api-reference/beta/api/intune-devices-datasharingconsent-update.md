---
title: 更新 dataSharingConsent
description: 更新 dataSharingConsent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8a856ce266380796344e178279a0629ddac2488
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469900"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="b5310-103">更新 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="b5310-103">Update dataSharingConsent</span></span>

<span data-ttu-id="b5310-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b5310-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5310-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5310-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5310-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5310-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5310-107">更新[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5310-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5310-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5310-108">Prerequisites</span></span>
<span data-ttu-id="b5310-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5310-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5310-111">Permission type</span></span>|<span data-ttu-id="b5310-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5310-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5310-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5310-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5310-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5310-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b5310-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5310-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5310-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5310-116">Not supported.</span></span>|
|<span data-ttu-id="b5310-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5310-117">Application</span></span>|<span data-ttu-id="b5310-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5310-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5310-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5310-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="b5310-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5310-120">Request headers</span></span>
|<span data-ttu-id="b5310-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5310-121">Header</span></span>|<span data-ttu-id="b5310-122">值</span><span class="sxs-lookup"><span data-stu-id="b5310-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5310-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5310-123">Authorization</span></span>|<span data-ttu-id="b5310-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5310-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5310-125">接受</span><span class="sxs-lookup"><span data-stu-id="b5310-125">Accept</span></span>|<span data-ttu-id="b5310-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5310-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5310-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5310-127">Request body</span></span>
<span data-ttu-id="b5310-128">在请求正文中，提供[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5310-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="b5310-129">下表显示创建[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5310-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="b5310-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5310-130">Property</span></span>|<span data-ttu-id="b5310-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5310-131">Type</span></span>|<span data-ttu-id="b5310-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5310-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5310-133">id</span><span class="sxs-lookup"><span data-stu-id="b5310-133">id</span></span>|<span data-ttu-id="b5310-134">String</span><span class="sxs-lookup"><span data-stu-id="b5310-134">String</span></span>|<span data-ttu-id="b5310-135">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="b5310-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="b5310-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b5310-136">serviceDisplayName</span></span>|<span data-ttu-id="b5310-137">String</span><span class="sxs-lookup"><span data-stu-id="b5310-137">String</span></span>|<span data-ttu-id="b5310-138">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="b5310-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="b5310-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="b5310-139">termsUrl</span></span>|<span data-ttu-id="b5310-140">String</span><span class="sxs-lookup"><span data-stu-id="b5310-140">String</span></span>|<span data-ttu-id="b5310-141">数据共享同意的 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="b5310-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="b5310-142">granted</span><span class="sxs-lookup"><span data-stu-id="b5310-142">granted</span></span>|<span data-ttu-id="b5310-143">布尔</span><span class="sxs-lookup"><span data-stu-id="b5310-143">Boolean</span></span>|<span data-ttu-id="b5310-144">"数据共享同意" 的 "已授予" 状态</span><span class="sxs-lookup"><span data-stu-id="b5310-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="b5310-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="b5310-145">grantDateTime</span></span>|<span data-ttu-id="b5310-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5310-146">DateTimeOffset</span></span>|<span data-ttu-id="b5310-147">授予此帐户的时间许可</span><span class="sxs-lookup"><span data-stu-id="b5310-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="b5310-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="b5310-148">grantedByUpn</span></span>|<span data-ttu-id="b5310-149">String</span><span class="sxs-lookup"><span data-stu-id="b5310-149">String</span></span>|<span data-ttu-id="b5310-150">授予此帐户同意的用户的 Upn</span><span class="sxs-lookup"><span data-stu-id="b5310-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="b5310-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="b5310-151">grantedByUserId</span></span>|<span data-ttu-id="b5310-152">String</span><span class="sxs-lookup"><span data-stu-id="b5310-152">String</span></span>|<span data-ttu-id="b5310-153">授予此帐户同意的用户的用户 Id</span><span class="sxs-lookup"><span data-stu-id="b5310-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="b5310-154">响应</span><span class="sxs-lookup"><span data-stu-id="b5310-154">Response</span></span>
<span data-ttu-id="b5310-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5310-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5310-156">示例</span><span class="sxs-lookup"><span data-stu-id="b5310-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5310-157">请求</span><span class="sxs-lookup"><span data-stu-id="b5310-157">Request</span></span>
<span data-ttu-id="b5310-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5310-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a><span data-ttu-id="b5310-159">响应</span><span class="sxs-lookup"><span data-stu-id="b5310-159">Response</span></span>
<span data-ttu-id="b5310-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5310-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "333387f7-87f7-3333-f787-3333f7873333",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```





