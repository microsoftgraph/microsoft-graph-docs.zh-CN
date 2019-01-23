---
title: 创建 dataSharingConsent
description: 创建新的 dataSharingConsent 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 686f8e5ddb56c53224d467bc6ac31cfdb5b6858c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406946"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="d4ba1-103">创建 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d4ba1-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="d4ba1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4ba1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4ba1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4ba1-107">创建新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4ba1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4ba1-108">Prerequisites</span></span>
<span data-ttu-id="d4ba1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d4ba1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4ba1-111">Permission type</span></span>|<span data-ttu-id="d4ba1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d4ba1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4ba1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4ba1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4ba1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4ba1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4ba1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4ba1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4ba1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-116">Not supported.</span></span>|
|<span data-ttu-id="d4ba1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4ba1-117">Application</span></span>|<span data-ttu-id="d4ba1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4ba1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4ba1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="d4ba1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4ba1-120">Request headers</span></span>
|<span data-ttu-id="d4ba1-121">标头</span><span class="sxs-lookup"><span data-stu-id="d4ba1-121">Header</span></span>|<span data-ttu-id="d4ba1-122">值</span><span class="sxs-lookup"><span data-stu-id="d4ba1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4ba1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4ba1-123">Authorization</span></span>|<span data-ttu-id="d4ba1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4ba1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4ba1-125">Accept</span></span>|<span data-ttu-id="d4ba1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4ba1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4ba1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4ba1-127">Request body</span></span>
<span data-ttu-id="d4ba1-128">在请求正文中，提供 dataSharingConsent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="d4ba1-129">下表显示时创建 dataSharingConsent 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="d4ba1-130">属性</span><span class="sxs-lookup"><span data-stu-id="d4ba1-130">Property</span></span>|<span data-ttu-id="d4ba1-131">类型</span><span class="sxs-lookup"><span data-stu-id="d4ba1-131">Type</span></span>|<span data-ttu-id="d4ba1-132">说明</span><span class="sxs-lookup"><span data-stu-id="d4ba1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4ba1-133">id</span><span class="sxs-lookup"><span data-stu-id="d4ba1-133">id</span></span>|<span data-ttu-id="d4ba1-134">String</span><span class="sxs-lookup"><span data-stu-id="d4ba1-134">String</span></span>|<span data-ttu-id="d4ba1-135">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="d4ba1-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="d4ba1-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d4ba1-136">serviceDisplayName</span></span>|<span data-ttu-id="d4ba1-137">String</span><span class="sxs-lookup"><span data-stu-id="d4ba1-137">String</span></span>|<span data-ttu-id="d4ba1-138">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="d4ba1-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="d4ba1-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="d4ba1-139">termsUrl</span></span>|<span data-ttu-id="d4ba1-140">String</span><span class="sxs-lookup"><span data-stu-id="d4ba1-140">String</span></span>|<span data-ttu-id="d4ba1-141">数据共享同意 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="d4ba1-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="d4ba1-142">granted</span><span class="sxs-lookup"><span data-stu-id="d4ba1-142">granted</span></span>|<span data-ttu-id="d4ba1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ba1-143">Boolean</span></span>|<span data-ttu-id="d4ba1-144">数据共享同意向其授予的状态</span><span class="sxs-lookup"><span data-stu-id="d4ba1-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="d4ba1-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ba1-145">grantDateTime</span></span>|<span data-ttu-id="d4ba1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ba1-146">DateTimeOffset</span></span>|<span data-ttu-id="d4ba1-147">此帐户授予时间同意</span><span class="sxs-lookup"><span data-stu-id="d4ba1-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="d4ba1-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="d4ba1-148">grantedByUpn</span></span>|<span data-ttu-id="d4ba1-149">String</span><span class="sxs-lookup"><span data-stu-id="d4ba1-149">String</span></span>|<span data-ttu-id="d4ba1-150">用户授予许可，为此帐户的 Upn</span><span class="sxs-lookup"><span data-stu-id="d4ba1-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="d4ba1-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="d4ba1-151">grantedByUserId</span></span>|<span data-ttu-id="d4ba1-152">String</span><span class="sxs-lookup"><span data-stu-id="d4ba1-152">String</span></span>|<span data-ttu-id="d4ba1-153">授予许可，为此帐户的用户的用户 Id</span><span class="sxs-lookup"><span data-stu-id="d4ba1-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="d4ba1-154">响应</span><span class="sxs-lookup"><span data-stu-id="d4ba1-154">Response</span></span>
<span data-ttu-id="d4ba1-155">如果成功，此方法返回`201 Created`响应代码和响应正文中的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4ba1-156">示例</span><span class="sxs-lookup"><span data-stu-id="d4ba1-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4ba1-157">请求</span><span class="sxs-lookup"><span data-stu-id="d4ba1-157">Request</span></span>
<span data-ttu-id="d4ba1-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4ba1-159">响应</span><span class="sxs-lookup"><span data-stu-id="d4ba1-159">Response</span></span>
<span data-ttu-id="d4ba1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4ba1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




