---
title: 更新 telecomExpenseManagementPartner
description: 更新 telecomExpenseManagementPartner 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a642e05ce730f1ebfb23a9b9c634555dd73b726f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511906"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="d4249-103">更新 telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="d4249-103">Update telecomExpenseManagementPartner</span></span>

<span data-ttu-id="d4249-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4249-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4249-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4249-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4249-106">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d4249-106">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4249-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4249-107">Prerequisites</span></span>
<span data-ttu-id="d4249-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4249-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4249-110">Permission type</span></span>|<span data-ttu-id="d4249-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d4249-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4249-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4249-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4249-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4249-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4249-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4249-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4249-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4249-115">Not supported.</span></span>|
|<span data-ttu-id="d4249-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4249-116">Application</span></span>|<span data-ttu-id="d4249-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4249-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4249-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4249-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="d4249-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4249-119">Request headers</span></span>
|<span data-ttu-id="d4249-120">标头</span><span class="sxs-lookup"><span data-stu-id="d4249-120">Header</span></span>|<span data-ttu-id="d4249-121">值</span><span class="sxs-lookup"><span data-stu-id="d4249-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4249-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4249-122">Authorization</span></span>|<span data-ttu-id="d4249-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4249-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4249-124">接受</span><span class="sxs-lookup"><span data-stu-id="d4249-124">Accept</span></span>|<span data-ttu-id="d4249-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4249-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4249-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4249-126">Request body</span></span>
<span data-ttu-id="d4249-127">在请求正文中，提供 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4249-127">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="d4249-128">下表显示创建 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4249-128">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="d4249-129">属性</span><span class="sxs-lookup"><span data-stu-id="d4249-129">Property</span></span>|<span data-ttu-id="d4249-130">类型</span><span class="sxs-lookup"><span data-stu-id="d4249-130">Type</span></span>|<span data-ttu-id="d4249-131">说明</span><span class="sxs-lookup"><span data-stu-id="d4249-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4249-132">id</span><span class="sxs-lookup"><span data-stu-id="d4249-132">id</span></span>|<span data-ttu-id="d4249-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d4249-133">String</span></span>|<span data-ttu-id="d4249-134">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d4249-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="d4249-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d4249-135">displayName</span></span>|<span data-ttu-id="d4249-136">字符串</span><span class="sxs-lookup"><span data-stu-id="d4249-136">String</span></span>|<span data-ttu-id="d4249-137">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d4249-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="d4249-138">url</span><span class="sxs-lookup"><span data-stu-id="d4249-138">url</span></span>|<span data-ttu-id="d4249-139">String</span><span class="sxs-lookup"><span data-stu-id="d4249-139">String</span></span>|<span data-ttu-id="d4249-140">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="d4249-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="d4249-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="d4249-141">appAuthorized</span></span>|<span data-ttu-id="d4249-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4249-142">Boolean</span></span>|<span data-ttu-id="d4249-143">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="d4249-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="d4249-144">enabled</span><span class="sxs-lookup"><span data-stu-id="d4249-144">enabled</span></span>|<span data-ttu-id="d4249-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4249-145">Boolean</span></span>|<span data-ttu-id="d4249-146">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="d4249-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="d4249-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d4249-147">lastConnectionDateTime</span></span>|<span data-ttu-id="d4249-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4249-148">DateTimeOffset</span></span>|<span data-ttu-id="d4249-149">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="d4249-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="d4249-150">响应</span><span class="sxs-lookup"><span data-stu-id="d4249-150">Response</span></span>
<span data-ttu-id="d4249-151">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4249-151">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4249-152">示例</span><span class="sxs-lookup"><span data-stu-id="d4249-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4249-153">请求</span><span class="sxs-lookup"><span data-stu-id="d4249-153">Request</span></span>
<span data-ttu-id="d4249-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4249-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d4249-155">响应</span><span class="sxs-lookup"><span data-stu-id="d4249-155">Response</span></span>
<span data-ttu-id="d4249-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4249-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




