---
title: 更新 dataSharingConsent
description: 更新 dataSharingConsent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f89d81976eeea5cb4832aeb670c0bee26069487
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958016"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="8d47c-103">更新 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8d47c-103">Update dataSharingConsent</span></span>

> <span data-ttu-id="8d47c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d47c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d47c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d47c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d47c-106">更新[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8d47c-106">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d47c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d47c-107">Prerequisites</span></span>
<span data-ttu-id="8d47c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d47c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d47c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d47c-110">Permission type</span></span>|<span data-ttu-id="8d47c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8d47c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d47c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d47c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d47c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d47c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d47c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d47c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d47c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d47c-115">Not supported.</span></span>|
|<span data-ttu-id="8d47c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d47c-116">Application</span></span>|<span data-ttu-id="8d47c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d47c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d47c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d47c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="8d47c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d47c-119">Request headers</span></span>
|<span data-ttu-id="8d47c-120">标头</span><span class="sxs-lookup"><span data-stu-id="8d47c-120">Header</span></span>|<span data-ttu-id="8d47c-121">值</span><span class="sxs-lookup"><span data-stu-id="8d47c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d47c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d47c-122">Authorization</span></span>|<span data-ttu-id="8d47c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d47c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d47c-124">接受</span><span class="sxs-lookup"><span data-stu-id="8d47c-124">Accept</span></span>|<span data-ttu-id="8d47c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d47c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d47c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d47c-126">Request body</span></span>
<span data-ttu-id="8d47c-127">在请求正文中, 提供[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d47c-127">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="8d47c-128">下表显示创建[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8d47c-128">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="8d47c-129">属性</span><span class="sxs-lookup"><span data-stu-id="8d47c-129">Property</span></span>|<span data-ttu-id="8d47c-130">类型</span><span class="sxs-lookup"><span data-stu-id="8d47c-130">Type</span></span>|<span data-ttu-id="8d47c-131">说明</span><span class="sxs-lookup"><span data-stu-id="8d47c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d47c-132">id</span><span class="sxs-lookup"><span data-stu-id="8d47c-132">id</span></span>|<span data-ttu-id="8d47c-133">String</span><span class="sxs-lookup"><span data-stu-id="8d47c-133">String</span></span>|<span data-ttu-id="8d47c-134">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="8d47c-134">The data sharing consent Id</span></span>|
|<span data-ttu-id="8d47c-135">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8d47c-135">serviceDisplayName</span></span>|<span data-ttu-id="8d47c-136">String</span><span class="sxs-lookup"><span data-stu-id="8d47c-136">String</span></span>|<span data-ttu-id="8d47c-137">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="8d47c-137">The display name of the service work flow</span></span>|
|<span data-ttu-id="8d47c-138">termsUrl</span><span class="sxs-lookup"><span data-stu-id="8d47c-138">termsUrl</span></span>|<span data-ttu-id="8d47c-139">String</span><span class="sxs-lookup"><span data-stu-id="8d47c-139">String</span></span>|<span data-ttu-id="8d47c-140">数据共享同意的 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="8d47c-140">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="8d47c-141">granted</span><span class="sxs-lookup"><span data-stu-id="8d47c-141">granted</span></span>|<span data-ttu-id="8d47c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d47c-142">Boolean</span></span>|<span data-ttu-id="8d47c-143">"数据共享同意" 的 "已授予" 状态</span><span class="sxs-lookup"><span data-stu-id="8d47c-143">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="8d47c-144">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="8d47c-144">grantDateTime</span></span>|<span data-ttu-id="8d47c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d47c-145">DateTimeOffset</span></span>|<span data-ttu-id="8d47c-146">授予此帐户的时间许可</span><span class="sxs-lookup"><span data-stu-id="8d47c-146">The time consent was granted for this account</span></span>|
|<span data-ttu-id="8d47c-147">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="8d47c-147">grantedByUpn</span></span>|<span data-ttu-id="8d47c-148">String</span><span class="sxs-lookup"><span data-stu-id="8d47c-148">String</span></span>|<span data-ttu-id="8d47c-149">授予此帐户同意的用户的 Upn</span><span class="sxs-lookup"><span data-stu-id="8d47c-149">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="8d47c-150">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="8d47c-150">grantedByUserId</span></span>|<span data-ttu-id="8d47c-151">String</span><span class="sxs-lookup"><span data-stu-id="8d47c-151">String</span></span>|<span data-ttu-id="8d47c-152">授予此帐户同意的用户的用户 id</span><span class="sxs-lookup"><span data-stu-id="8d47c-152">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="8d47c-153">响应</span><span class="sxs-lookup"><span data-stu-id="8d47c-153">Response</span></span>
<span data-ttu-id="8d47c-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8d47c-154">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d47c-155">示例</span><span class="sxs-lookup"><span data-stu-id="8d47c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d47c-156">请求</span><span class="sxs-lookup"><span data-stu-id="8d47c-156">Request</span></span>
<span data-ttu-id="8d47c-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d47c-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d47c-158">响应</span><span class="sxs-lookup"><span data-stu-id="8d47c-158">Response</span></span>
<span data-ttu-id="8d47c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d47c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




