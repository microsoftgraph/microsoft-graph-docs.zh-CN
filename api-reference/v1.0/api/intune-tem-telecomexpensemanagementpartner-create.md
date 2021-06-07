---
title: 创建 telecomExpenseManagementPartner
description: 创建新的 telecomExpenseManagementPartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: deada7598a04b1d1de96eb586d7429a613411f32
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757870"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="dc327-103">创建 telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="dc327-103">Create telecomExpenseManagementPartner</span></span>

<span data-ttu-id="dc327-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc327-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc327-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc327-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc327-106">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc327-106">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc327-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dc327-107">Prerequisites</span></span>
<span data-ttu-id="dc327-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc327-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc327-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc327-110">Permission type</span></span>|<span data-ttu-id="dc327-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc327-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc327-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc327-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc327-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc327-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc327-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc327-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc327-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc327-115">Not supported.</span></span>|
|<span data-ttu-id="dc327-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc327-116">Application</span></span>|<span data-ttu-id="dc327-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc327-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc327-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc327-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="dc327-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc327-119">Request headers</span></span>
|<span data-ttu-id="dc327-120">标头</span><span class="sxs-lookup"><span data-stu-id="dc327-120">Header</span></span>|<span data-ttu-id="dc327-121">值</span><span class="sxs-lookup"><span data-stu-id="dc327-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc327-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc327-122">Authorization</span></span>|<span data-ttu-id="dc327-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dc327-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc327-124">接受</span><span class="sxs-lookup"><span data-stu-id="dc327-124">Accept</span></span>|<span data-ttu-id="dc327-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc327-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc327-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc327-126">Request body</span></span>
<span data-ttu-id="dc327-127">在请求正文中，提供 telecomExpenseManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc327-127">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="dc327-128">下表显示创建 telecomExpenseManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dc327-128">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="dc327-129">属性</span><span class="sxs-lookup"><span data-stu-id="dc327-129">Property</span></span>|<span data-ttu-id="dc327-130">类型</span><span class="sxs-lookup"><span data-stu-id="dc327-130">Type</span></span>|<span data-ttu-id="dc327-131">说明</span><span class="sxs-lookup"><span data-stu-id="dc327-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc327-132">id</span><span class="sxs-lookup"><span data-stu-id="dc327-132">id</span></span>|<span data-ttu-id="dc327-133">String</span><span class="sxs-lookup"><span data-stu-id="dc327-133">String</span></span>|<span data-ttu-id="dc327-134">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dc327-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="dc327-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dc327-135">displayName</span></span>|<span data-ttu-id="dc327-136">String</span><span class="sxs-lookup"><span data-stu-id="dc327-136">String</span></span>|<span data-ttu-id="dc327-137">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dc327-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="dc327-138">url</span><span class="sxs-lookup"><span data-stu-id="dc327-138">url</span></span>|<span data-ttu-id="dc327-139">String</span><span class="sxs-lookup"><span data-stu-id="dc327-139">String</span></span>|<span data-ttu-id="dc327-140">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="dc327-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="dc327-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="dc327-141">appAuthorized</span></span>|<span data-ttu-id="dc327-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc327-142">Boolean</span></span>|<span data-ttu-id="dc327-143">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="dc327-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="dc327-144">enabled</span><span class="sxs-lookup"><span data-stu-id="dc327-144">enabled</span></span>|<span data-ttu-id="dc327-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc327-145">Boolean</span></span>|<span data-ttu-id="dc327-146">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="dc327-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="dc327-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="dc327-147">lastConnectionDateTime</span></span>|<span data-ttu-id="dc327-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc327-148">DateTimeOffset</span></span>|<span data-ttu-id="dc327-149">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="dc327-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="dc327-150">响应</span><span class="sxs-lookup"><span data-stu-id="dc327-150">Response</span></span>
<span data-ttu-id="dc327-151">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc327-151">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc327-152">示例</span><span class="sxs-lookup"><span data-stu-id="dc327-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc327-153">请求</span><span class="sxs-lookup"><span data-stu-id="dc327-153">Request</span></span>
<span data-ttu-id="dc327-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc327-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="dc327-155">响应</span><span class="sxs-lookup"><span data-stu-id="dc327-155">Response</span></span>
<span data-ttu-id="dc327-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc327-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




