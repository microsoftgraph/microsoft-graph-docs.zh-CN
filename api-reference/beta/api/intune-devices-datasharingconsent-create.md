---
title: 创建 dataSharingConsent
description: 创建新的 dataSharingConsent 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 87e9044fc48f857aa64c75f7a9b5579d8ae7573a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154425"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="05eae-103">创建 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="05eae-103">Create dataSharingConsent</span></span>

<span data-ttu-id="05eae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05eae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05eae-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05eae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05eae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05eae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05eae-107">创建新的 [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05eae-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05eae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="05eae-108">Prerequisites</span></span>
<span data-ttu-id="05eae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05eae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05eae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="05eae-111">Permission type</span></span>|<span data-ttu-id="05eae-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05eae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05eae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05eae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05eae-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05eae-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="05eae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05eae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05eae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05eae-116">Not supported.</span></span>|
|<span data-ttu-id="05eae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="05eae-117">Application</span></span>|<span data-ttu-id="05eae-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05eae-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05eae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05eae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="05eae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05eae-120">Request headers</span></span>
|<span data-ttu-id="05eae-121">标头</span><span class="sxs-lookup"><span data-stu-id="05eae-121">Header</span></span>|<span data-ttu-id="05eae-122">值</span><span class="sxs-lookup"><span data-stu-id="05eae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05eae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05eae-123">Authorization</span></span>|<span data-ttu-id="05eae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05eae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05eae-125">接受</span><span class="sxs-lookup"><span data-stu-id="05eae-125">Accept</span></span>|<span data-ttu-id="05eae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05eae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05eae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05eae-127">Request body</span></span>
<span data-ttu-id="05eae-128">在请求正文中，提供 dataSharingConsent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05eae-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="05eae-129">下表显示创建 dataSharingConsent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="05eae-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="05eae-130">属性</span><span class="sxs-lookup"><span data-stu-id="05eae-130">Property</span></span>|<span data-ttu-id="05eae-131">类型</span><span class="sxs-lookup"><span data-stu-id="05eae-131">Type</span></span>|<span data-ttu-id="05eae-132">说明</span><span class="sxs-lookup"><span data-stu-id="05eae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05eae-133">id</span><span class="sxs-lookup"><span data-stu-id="05eae-133">id</span></span>|<span data-ttu-id="05eae-134">String</span><span class="sxs-lookup"><span data-stu-id="05eae-134">String</span></span>|<span data-ttu-id="05eae-135">数据共享许可 ID</span><span class="sxs-lookup"><span data-stu-id="05eae-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="05eae-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="05eae-136">serviceDisplayName</span></span>|<span data-ttu-id="05eae-137">String</span><span class="sxs-lookup"><span data-stu-id="05eae-137">String</span></span>|<span data-ttu-id="05eae-138">服务显示名称流</span><span class="sxs-lookup"><span data-stu-id="05eae-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="05eae-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="05eae-139">termsUrl</span></span>|<span data-ttu-id="05eae-140">String</span><span class="sxs-lookup"><span data-stu-id="05eae-140">String</span></span>|<span data-ttu-id="05eae-141">数据共享同意的 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="05eae-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="05eae-142">granted</span><span class="sxs-lookup"><span data-stu-id="05eae-142">granted</span></span>|<span data-ttu-id="05eae-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="05eae-143">Boolean</span></span>|<span data-ttu-id="05eae-144">数据共享同意的授予状态</span><span class="sxs-lookup"><span data-stu-id="05eae-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="05eae-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="05eae-145">grantDateTime</span></span>|<span data-ttu-id="05eae-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05eae-146">DateTimeOffset</span></span>|<span data-ttu-id="05eae-147">为此帐户授予许可的时间</span><span class="sxs-lookup"><span data-stu-id="05eae-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="05eae-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="05eae-148">grantedByUpn</span></span>|<span data-ttu-id="05eae-149">String</span><span class="sxs-lookup"><span data-stu-id="05eae-149">String</span></span>|<span data-ttu-id="05eae-150">授予此帐户同意的用户的 Upn</span><span class="sxs-lookup"><span data-stu-id="05eae-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="05eae-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="05eae-151">grantedByUserId</span></span>|<span data-ttu-id="05eae-152">String</span><span class="sxs-lookup"><span data-stu-id="05eae-152">String</span></span>|<span data-ttu-id="05eae-153">授予此帐户同意的用户的 UserId</span><span class="sxs-lookup"><span data-stu-id="05eae-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="05eae-154">响应</span><span class="sxs-lookup"><span data-stu-id="05eae-154">Response</span></span>
<span data-ttu-id="05eae-155">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05eae-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05eae-156">示例</span><span class="sxs-lookup"><span data-stu-id="05eae-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="05eae-157">请求</span><span class="sxs-lookup"><span data-stu-id="05eae-157">Request</span></span>
<span data-ttu-id="05eae-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05eae-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05eae-159">响应</span><span class="sxs-lookup"><span data-stu-id="05eae-159">Response</span></span>
<span data-ttu-id="05eae-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05eae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




