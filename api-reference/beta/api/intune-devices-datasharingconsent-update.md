---
title: 更新 dataSharingConsent
description: 更新 dataSharingConsent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d617546464b1333af2b535bbc1c17f61fa03386
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146543"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="4630e-103">更新 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="4630e-103">Update dataSharingConsent</span></span>

<span data-ttu-id="4630e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4630e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4630e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4630e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4630e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4630e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4630e-107">更新 [dataSharingConsent 对象](../resources/intune-devices-datasharingconsent.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4630e-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4630e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4630e-108">Prerequisites</span></span>
<span data-ttu-id="4630e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4630e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4630e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4630e-111">Permission type</span></span>|<span data-ttu-id="4630e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4630e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4630e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4630e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4630e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4630e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4630e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4630e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4630e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4630e-116">Not supported.</span></span>|
|<span data-ttu-id="4630e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4630e-117">Application</span></span>|<span data-ttu-id="4630e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4630e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4630e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4630e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="4630e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4630e-120">Request headers</span></span>
|<span data-ttu-id="4630e-121">标头</span><span class="sxs-lookup"><span data-stu-id="4630e-121">Header</span></span>|<span data-ttu-id="4630e-122">值</span><span class="sxs-lookup"><span data-stu-id="4630e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4630e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4630e-123">Authorization</span></span>|<span data-ttu-id="4630e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4630e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4630e-125">接受</span><span class="sxs-lookup"><span data-stu-id="4630e-125">Accept</span></span>|<span data-ttu-id="4630e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4630e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4630e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4630e-127">Request body</span></span>
<span data-ttu-id="4630e-128">在请求正文中，提供 [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4630e-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="4630e-129">下表显示创建 [dataSharingConsent 时所需的属性](../resources/intune-devices-datasharingconsent.md)。</span><span class="sxs-lookup"><span data-stu-id="4630e-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="4630e-130">属性</span><span class="sxs-lookup"><span data-stu-id="4630e-130">Property</span></span>|<span data-ttu-id="4630e-131">类型</span><span class="sxs-lookup"><span data-stu-id="4630e-131">Type</span></span>|<span data-ttu-id="4630e-132">说明</span><span class="sxs-lookup"><span data-stu-id="4630e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4630e-133">id</span><span class="sxs-lookup"><span data-stu-id="4630e-133">id</span></span>|<span data-ttu-id="4630e-134">String</span><span class="sxs-lookup"><span data-stu-id="4630e-134">String</span></span>|<span data-ttu-id="4630e-135">数据共享许可 ID</span><span class="sxs-lookup"><span data-stu-id="4630e-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="4630e-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4630e-136">serviceDisplayName</span></span>|<span data-ttu-id="4630e-137">String</span><span class="sxs-lookup"><span data-stu-id="4630e-137">String</span></span>|<span data-ttu-id="4630e-138">服务显示名称流</span><span class="sxs-lookup"><span data-stu-id="4630e-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="4630e-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="4630e-139">termsUrl</span></span>|<span data-ttu-id="4630e-140">String</span><span class="sxs-lookup"><span data-stu-id="4630e-140">String</span></span>|<span data-ttu-id="4630e-141">数据共享同意的 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="4630e-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="4630e-142">granted</span><span class="sxs-lookup"><span data-stu-id="4630e-142">granted</span></span>|<span data-ttu-id="4630e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4630e-143">Boolean</span></span>|<span data-ttu-id="4630e-144">数据共享同意的授予状态</span><span class="sxs-lookup"><span data-stu-id="4630e-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="4630e-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="4630e-145">grantDateTime</span></span>|<span data-ttu-id="4630e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4630e-146">DateTimeOffset</span></span>|<span data-ttu-id="4630e-147">为此帐户授予许可的时间</span><span class="sxs-lookup"><span data-stu-id="4630e-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="4630e-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="4630e-148">grantedByUpn</span></span>|<span data-ttu-id="4630e-149">String</span><span class="sxs-lookup"><span data-stu-id="4630e-149">String</span></span>|<span data-ttu-id="4630e-150">授予此帐户同意的用户的 Upn</span><span class="sxs-lookup"><span data-stu-id="4630e-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="4630e-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="4630e-151">grantedByUserId</span></span>|<span data-ttu-id="4630e-152">String</span><span class="sxs-lookup"><span data-stu-id="4630e-152">String</span></span>|<span data-ttu-id="4630e-153">授予此帐户同意的用户的 UserId</span><span class="sxs-lookup"><span data-stu-id="4630e-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="4630e-154">响应</span><span class="sxs-lookup"><span data-stu-id="4630e-154">Response</span></span>
<span data-ttu-id="4630e-155">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4630e-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4630e-156">示例</span><span class="sxs-lookup"><span data-stu-id="4630e-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="4630e-157">请求</span><span class="sxs-lookup"><span data-stu-id="4630e-157">Request</span></span>
<span data-ttu-id="4630e-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4630e-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4630e-159">响应</span><span class="sxs-lookup"><span data-stu-id="4630e-159">Response</span></span>
<span data-ttu-id="4630e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4630e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




