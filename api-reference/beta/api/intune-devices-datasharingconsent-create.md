---
title: 创建 dataSharingConsent
description: 创建新的 dataSharingConsent 对象。
author: tfitzmac
ms.openlocfilehash: 07d76bbd92d2741571683bb7614b3336c10d9058
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349670"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="7b787-103">创建 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="7b787-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="7b787-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b787-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b787-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b787-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b787-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7b787-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b787-107">创建新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b787-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b787-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b787-108">Prerequisites</span></span>
<span data-ttu-id="7b787-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7b787-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b787-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b787-111">Permission type</span></span>|<span data-ttu-id="7b787-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b787-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b787-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b787-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b787-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b787-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7b787-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b787-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b787-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b787-116">Not supported.</span></span>|
|<span data-ttu-id="7b787-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b787-117">Application</span></span>|<span data-ttu-id="7b787-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b787-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b787-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b787-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="7b787-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b787-120">Request headers</span></span>
|<span data-ttu-id="7b787-121">标头</span><span class="sxs-lookup"><span data-stu-id="7b787-121">Header</span></span>|<span data-ttu-id="7b787-122">值</span><span class="sxs-lookup"><span data-stu-id="7b787-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b787-123">授权</span><span class="sxs-lookup"><span data-stu-id="7b787-123">Authorization</span></span>|<span data-ttu-id="7b787-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b787-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b787-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b787-125">Accept</span></span>|<span data-ttu-id="7b787-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b787-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b787-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b787-127">Request body</span></span>
<span data-ttu-id="7b787-128">在请求正文中，提供 dataSharingConsent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b787-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="7b787-129">下表显示时创建 dataSharingConsent 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7b787-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="7b787-130">属性</span><span class="sxs-lookup"><span data-stu-id="7b787-130">Property</span></span>|<span data-ttu-id="7b787-131">类型</span><span class="sxs-lookup"><span data-stu-id="7b787-131">Type</span></span>|<span data-ttu-id="7b787-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b787-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b787-133">id</span><span class="sxs-lookup"><span data-stu-id="7b787-133">id</span></span>|<span data-ttu-id="7b787-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7b787-134">String</span></span>|<span data-ttu-id="7b787-135">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="7b787-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="7b787-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b787-136">serviceDisplayName</span></span>|<span data-ttu-id="7b787-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7b787-137">String</span></span>|<span data-ttu-id="7b787-138">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="7b787-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="7b787-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="7b787-139">termsUrl</span></span>|<span data-ttu-id="7b787-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7b787-140">String</span></span>|<span data-ttu-id="7b787-141">数据共享同意 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="7b787-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="7b787-142">授予</span><span class="sxs-lookup"><span data-stu-id="7b787-142">granted</span></span>|<span data-ttu-id="7b787-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b787-143">Boolean</span></span>|<span data-ttu-id="7b787-144">数据共享同意向其授予的状态</span><span class="sxs-lookup"><span data-stu-id="7b787-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="7b787-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="7b787-145">grantDateTime</span></span>|<span data-ttu-id="7b787-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b787-146">DateTimeOffset</span></span>|<span data-ttu-id="7b787-147">此帐户授予时间同意</span><span class="sxs-lookup"><span data-stu-id="7b787-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="7b787-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="7b787-148">grantedByUpn</span></span>|<span data-ttu-id="7b787-149">字符串</span><span class="sxs-lookup"><span data-stu-id="7b787-149">String</span></span>|<span data-ttu-id="7b787-150">用户授予许可，为此帐户的 Upn</span><span class="sxs-lookup"><span data-stu-id="7b787-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="7b787-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="7b787-151">grantedByUserId</span></span>|<span data-ttu-id="7b787-152">字符串</span><span class="sxs-lookup"><span data-stu-id="7b787-152">String</span></span>|<span data-ttu-id="7b787-153">授予许可，为此帐户的用户的用户 Id</span><span class="sxs-lookup"><span data-stu-id="7b787-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="7b787-154">响应</span><span class="sxs-lookup"><span data-stu-id="7b787-154">Response</span></span>
<span data-ttu-id="7b787-155">如果成功，此方法返回`201 Created`响应代码和响应正文中的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b787-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b787-156">示例</span><span class="sxs-lookup"><span data-stu-id="7b787-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b787-157">请求</span><span class="sxs-lookup"><span data-stu-id="7b787-157">Request</span></span>
<span data-ttu-id="7b787-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b787-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b787-159">响应</span><span class="sxs-lookup"><span data-stu-id="7b787-159">Response</span></span>
<span data-ttu-id="7b787-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b787-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





