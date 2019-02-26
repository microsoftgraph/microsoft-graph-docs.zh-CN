---
title: 创建 telecomExpenseManagementPartner
description: 创建新的 telecomExpenseManagementPartner 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c83b26e0f9d9c2a881ca37a4a56c2cc37883120
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262326"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="901ea-103">创建 telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="901ea-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="901ea-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="901ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="901ea-105">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="901ea-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="901ea-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="901ea-106">Prerequisites</span></span>
<span data-ttu-id="901ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="901ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="901ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="901ea-109">Permission type</span></span>|<span data-ttu-id="901ea-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="901ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="901ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="901ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="901ea-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901ea-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="901ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="901ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="901ea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="901ea-114">Not supported.</span></span>|
|<span data-ttu-id="901ea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="901ea-115">Application</span></span>|<span data-ttu-id="901ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="901ea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="901ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="901ea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="901ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="901ea-118">Request headers</span></span>
|<span data-ttu-id="901ea-119">标头</span><span class="sxs-lookup"><span data-stu-id="901ea-119">Header</span></span>|<span data-ttu-id="901ea-120">值</span><span class="sxs-lookup"><span data-stu-id="901ea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="901ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="901ea-121">Authorization</span></span>|<span data-ttu-id="901ea-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="901ea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="901ea-123">Accept</span><span class="sxs-lookup"><span data-stu-id="901ea-123">Accept</span></span>|<span data-ttu-id="901ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="901ea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="901ea-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="901ea-125">Request body</span></span>
<span data-ttu-id="901ea-126">在请求正文中，提供 telecomExpenseManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="901ea-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="901ea-127">下表显示创建 telecomExpenseManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="901ea-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="901ea-128">属性</span><span class="sxs-lookup"><span data-stu-id="901ea-128">Property</span></span>|<span data-ttu-id="901ea-129">类型</span><span class="sxs-lookup"><span data-stu-id="901ea-129">Type</span></span>|<span data-ttu-id="901ea-130">说明</span><span class="sxs-lookup"><span data-stu-id="901ea-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="901ea-131">id</span><span class="sxs-lookup"><span data-stu-id="901ea-131">id</span></span>|<span data-ttu-id="901ea-132">String</span><span class="sxs-lookup"><span data-stu-id="901ea-132">String</span></span>|<span data-ttu-id="901ea-133">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="901ea-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="901ea-134">displayName</span><span class="sxs-lookup"><span data-stu-id="901ea-134">displayName</span></span>|<span data-ttu-id="901ea-135">String</span><span class="sxs-lookup"><span data-stu-id="901ea-135">String</span></span>|<span data-ttu-id="901ea-136">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="901ea-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="901ea-137">url</span><span class="sxs-lookup"><span data-stu-id="901ea-137">url</span></span>|<span data-ttu-id="901ea-138">String</span><span class="sxs-lookup"><span data-stu-id="901ea-138">String</span></span>|<span data-ttu-id="901ea-139">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="901ea-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="901ea-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="901ea-140">appAuthorized</span></span>|<span data-ttu-id="901ea-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="901ea-141">Boolean</span></span>|<span data-ttu-id="901ea-142">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="901ea-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="901ea-143">enabled</span><span class="sxs-lookup"><span data-stu-id="901ea-143">enabled</span></span>|<span data-ttu-id="901ea-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="901ea-144">Boolean</span></span>|<span data-ttu-id="901ea-145">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="901ea-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="901ea-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="901ea-146">lastConnectionDateTime</span></span>|<span data-ttu-id="901ea-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="901ea-147">DateTimeOffset</span></span>|<span data-ttu-id="901ea-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="901ea-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="901ea-149">响应</span><span class="sxs-lookup"><span data-stu-id="901ea-149">Response</span></span>
<span data-ttu-id="901ea-150">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="901ea-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="901ea-151">示例</span><span class="sxs-lookup"><span data-stu-id="901ea-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="901ea-152">请求</span><span class="sxs-lookup"><span data-stu-id="901ea-152">Request</span></span>
<span data-ttu-id="901ea-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="901ea-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="901ea-154">响应</span><span class="sxs-lookup"><span data-stu-id="901ea-154">Response</span></span>
<span data-ttu-id="901ea-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="901ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



