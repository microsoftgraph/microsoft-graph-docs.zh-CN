---
title: 更新 dataSharingConsent
description: 更新 dataSharingConsent 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 143e2c655adac2403f49bb92afff2aca30a3653f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421114"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="f88cf-103">更新 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="f88cf-103">Update dataSharingConsent</span></span>

> <span data-ttu-id="f88cf-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f88cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f88cf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f88cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f88cf-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f88cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f88cf-107">更新[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f88cf-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f88cf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f88cf-108">Prerequisites</span></span>
<span data-ttu-id="f88cf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f88cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f88cf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f88cf-111">Permission type</span></span>|<span data-ttu-id="f88cf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f88cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f88cf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f88cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f88cf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f88cf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f88cf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f88cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f88cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f88cf-116">Not supported.</span></span>|
|<span data-ttu-id="f88cf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f88cf-117">Application</span></span>|<span data-ttu-id="f88cf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f88cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f88cf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f88cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="f88cf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f88cf-120">Request headers</span></span>
|<span data-ttu-id="f88cf-121">标头</span><span class="sxs-lookup"><span data-stu-id="f88cf-121">Header</span></span>|<span data-ttu-id="f88cf-122">值</span><span class="sxs-lookup"><span data-stu-id="f88cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f88cf-123">授权</span><span class="sxs-lookup"><span data-stu-id="f88cf-123">Authorization</span></span>|<span data-ttu-id="f88cf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f88cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f88cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f88cf-125">Accept</span></span>|<span data-ttu-id="f88cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f88cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f88cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f88cf-127">Request body</span></span>
<span data-ttu-id="f88cf-128">在请求正文中，提供[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f88cf-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="f88cf-129">下表显示时创建[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f88cf-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="f88cf-130">属性</span><span class="sxs-lookup"><span data-stu-id="f88cf-130">Property</span></span>|<span data-ttu-id="f88cf-131">类型</span><span class="sxs-lookup"><span data-stu-id="f88cf-131">Type</span></span>|<span data-ttu-id="f88cf-132">说明</span><span class="sxs-lookup"><span data-stu-id="f88cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f88cf-133">id</span><span class="sxs-lookup"><span data-stu-id="f88cf-133">id</span></span>|<span data-ttu-id="f88cf-134">String</span><span class="sxs-lookup"><span data-stu-id="f88cf-134">String</span></span>|<span data-ttu-id="f88cf-135">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="f88cf-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="f88cf-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f88cf-136">serviceDisplayName</span></span>|<span data-ttu-id="f88cf-137">String</span><span class="sxs-lookup"><span data-stu-id="f88cf-137">String</span></span>|<span data-ttu-id="f88cf-138">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="f88cf-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="f88cf-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="f88cf-139">termsUrl</span></span>|<span data-ttu-id="f88cf-140">String</span><span class="sxs-lookup"><span data-stu-id="f88cf-140">String</span></span>|<span data-ttu-id="f88cf-141">数据共享同意 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="f88cf-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="f88cf-142">granted</span><span class="sxs-lookup"><span data-stu-id="f88cf-142">granted</span></span>|<span data-ttu-id="f88cf-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f88cf-143">Boolean</span></span>|<span data-ttu-id="f88cf-144">数据共享同意向其授予的状态</span><span class="sxs-lookup"><span data-stu-id="f88cf-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="f88cf-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="f88cf-145">grantDateTime</span></span>|<span data-ttu-id="f88cf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f88cf-146">DateTimeOffset</span></span>|<span data-ttu-id="f88cf-147">此帐户授予时间同意</span><span class="sxs-lookup"><span data-stu-id="f88cf-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="f88cf-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="f88cf-148">grantedByUpn</span></span>|<span data-ttu-id="f88cf-149">String</span><span class="sxs-lookup"><span data-stu-id="f88cf-149">String</span></span>|<span data-ttu-id="f88cf-150">用户授予许可，为此帐户的 Upn</span><span class="sxs-lookup"><span data-stu-id="f88cf-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="f88cf-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="f88cf-151">grantedByUserId</span></span>|<span data-ttu-id="f88cf-152">String</span><span class="sxs-lookup"><span data-stu-id="f88cf-152">String</span></span>|<span data-ttu-id="f88cf-153">授予许可，为此帐户的用户的用户 Id</span><span class="sxs-lookup"><span data-stu-id="f88cf-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="f88cf-154">响应</span><span class="sxs-lookup"><span data-stu-id="f88cf-154">Response</span></span>
<span data-ttu-id="f88cf-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f88cf-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f88cf-156">示例</span><span class="sxs-lookup"><span data-stu-id="f88cf-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f88cf-157">请求</span><span class="sxs-lookup"><span data-stu-id="f88cf-157">Request</span></span>
<span data-ttu-id="f88cf-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f88cf-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f88cf-159">响应</span><span class="sxs-lookup"><span data-stu-id="f88cf-159">Response</span></span>
<span data-ttu-id="f88cf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f88cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




