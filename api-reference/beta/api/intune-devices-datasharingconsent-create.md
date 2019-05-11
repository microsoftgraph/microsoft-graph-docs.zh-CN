---
title: 创建 dataSharingConsent
description: 创建新的 dataSharingConsent 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83928d0ee472d4c902ac7df75a17ab1cebe66ff3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33910176"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="f1d4e-103">创建 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="f1d4e-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="f1d4e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1d4e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1d4e-106">创建新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-106">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1d4e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1d4e-107">Prerequisites</span></span>
<span data-ttu-id="f1d4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d4e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1d4e-110">Permission type</span></span>|<span data-ttu-id="f1d4e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1d4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1d4e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1d4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1d4e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d4e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f1d4e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1d4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1d4e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-115">Not supported.</span></span>|
|<span data-ttu-id="f1d4e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1d4e-116">Application</span></span>|<span data-ttu-id="f1d4e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1d4e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1d4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="f1d4e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1d4e-119">Request headers</span></span>
|<span data-ttu-id="f1d4e-120">标头</span><span class="sxs-lookup"><span data-stu-id="f1d4e-120">Header</span></span>|<span data-ttu-id="f1d4e-121">值</span><span class="sxs-lookup"><span data-stu-id="f1d4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1d4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1d4e-122">Authorization</span></span>|<span data-ttu-id="f1d4e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1d4e-124">接受</span><span class="sxs-lookup"><span data-stu-id="f1d4e-124">Accept</span></span>|<span data-ttu-id="f1d4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1d4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d4e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1d4e-126">Request body</span></span>
<span data-ttu-id="f1d4e-127">在请求正文中, 提供 dataSharingConsent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-127">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="f1d4e-128">下表显示创建 dataSharingConsent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-128">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="f1d4e-129">属性</span><span class="sxs-lookup"><span data-stu-id="f1d4e-129">Property</span></span>|<span data-ttu-id="f1d4e-130">类型</span><span class="sxs-lookup"><span data-stu-id="f1d4e-130">Type</span></span>|<span data-ttu-id="f1d4e-131">说明</span><span class="sxs-lookup"><span data-stu-id="f1d4e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d4e-132">id</span><span class="sxs-lookup"><span data-stu-id="f1d4e-132">id</span></span>|<span data-ttu-id="f1d4e-133">String</span><span class="sxs-lookup"><span data-stu-id="f1d4e-133">String</span></span>|<span data-ttu-id="f1d4e-134">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="f1d4e-134">The data sharing consent Id</span></span>|
|<span data-ttu-id="f1d4e-135">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1d4e-135">serviceDisplayName</span></span>|<span data-ttu-id="f1d4e-136">String</span><span class="sxs-lookup"><span data-stu-id="f1d4e-136">String</span></span>|<span data-ttu-id="f1d4e-137">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="f1d4e-137">The display name of the service work flow</span></span>|
|<span data-ttu-id="f1d4e-138">termsUrl</span><span class="sxs-lookup"><span data-stu-id="f1d4e-138">termsUrl</span></span>|<span data-ttu-id="f1d4e-139">String</span><span class="sxs-lookup"><span data-stu-id="f1d4e-139">String</span></span>|<span data-ttu-id="f1d4e-140">数据共享同意的 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="f1d4e-140">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="f1d4e-141">granted</span><span class="sxs-lookup"><span data-stu-id="f1d4e-141">granted</span></span>|<span data-ttu-id="f1d4e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d4e-142">Boolean</span></span>|<span data-ttu-id="f1d4e-143">"数据共享同意" 的 "已授予" 状态</span><span class="sxs-lookup"><span data-stu-id="f1d4e-143">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="f1d4e-144">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d4e-144">grantDateTime</span></span>|<span data-ttu-id="f1d4e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d4e-145">DateTimeOffset</span></span>|<span data-ttu-id="f1d4e-146">授予此帐户的时间许可</span><span class="sxs-lookup"><span data-stu-id="f1d4e-146">The time consent was granted for this account</span></span>|
|<span data-ttu-id="f1d4e-147">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="f1d4e-147">grantedByUpn</span></span>|<span data-ttu-id="f1d4e-148">String</span><span class="sxs-lookup"><span data-stu-id="f1d4e-148">String</span></span>|<span data-ttu-id="f1d4e-149">授予此帐户同意的用户的 Upn</span><span class="sxs-lookup"><span data-stu-id="f1d4e-149">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="f1d4e-150">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="f1d4e-150">grantedByUserId</span></span>|<span data-ttu-id="f1d4e-151">String</span><span class="sxs-lookup"><span data-stu-id="f1d4e-151">String</span></span>|<span data-ttu-id="f1d4e-152">授予此帐户同意的用户的用户 Id</span><span class="sxs-lookup"><span data-stu-id="f1d4e-152">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="f1d4e-153">响应</span><span class="sxs-lookup"><span data-stu-id="f1d4e-153">Response</span></span>
<span data-ttu-id="f1d4e-154">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-154">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1d4e-155">示例</span><span class="sxs-lookup"><span data-stu-id="f1d4e-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1d4e-156">请求</span><span class="sxs-lookup"><span data-stu-id="f1d4e-156">Request</span></span>
<span data-ttu-id="f1d4e-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
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

### <a name="response"></a><span data-ttu-id="f1d4e-158">响应</span><span class="sxs-lookup"><span data-stu-id="f1d4e-158">Response</span></span>
<span data-ttu-id="f1d4e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1d4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




