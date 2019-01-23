---
title: 创建 telecomExpenseManagementPartner
description: 创建新的 telecomExpenseManagementPartner 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d39e3b81700b95134ea2d243f6dd8920e61f48b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395844"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="3d975-103">创建 telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3d975-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="3d975-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3d975-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d975-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3d975-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d975-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d975-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d975-107">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d975-107">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d975-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d975-108">Prerequisites</span></span>
<span data-ttu-id="3d975-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3d975-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d975-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d975-111">Permission type</span></span>|<span data-ttu-id="3d975-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d975-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d975-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d975-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d975-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d975-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d975-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d975-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d975-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d975-116">Not supported.</span></span>|
|<span data-ttu-id="3d975-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d975-117">Application</span></span>|<span data-ttu-id="3d975-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d975-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d975-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d975-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="3d975-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d975-120">Request headers</span></span>
|<span data-ttu-id="3d975-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d975-121">Header</span></span>|<span data-ttu-id="3d975-122">值</span><span class="sxs-lookup"><span data-stu-id="3d975-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d975-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d975-123">Authorization</span></span>|<span data-ttu-id="3d975-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d975-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d975-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d975-125">Accept</span></span>|<span data-ttu-id="3d975-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d975-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d975-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d975-127">Request body</span></span>
<span data-ttu-id="3d975-128">在请求正文中，提供 telecomExpenseManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d975-128">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="3d975-129">下表显示创建 telecomExpenseManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d975-129">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="3d975-130">属性</span><span class="sxs-lookup"><span data-stu-id="3d975-130">Property</span></span>|<span data-ttu-id="3d975-131">类型</span><span class="sxs-lookup"><span data-stu-id="3d975-131">Type</span></span>|<span data-ttu-id="3d975-132">说明</span><span class="sxs-lookup"><span data-stu-id="3d975-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d975-133">id</span><span class="sxs-lookup"><span data-stu-id="3d975-133">id</span></span>|<span data-ttu-id="3d975-134">String</span><span class="sxs-lookup"><span data-stu-id="3d975-134">String</span></span>|<span data-ttu-id="3d975-135">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3d975-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="3d975-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3d975-136">displayName</span></span>|<span data-ttu-id="3d975-137">String</span><span class="sxs-lookup"><span data-stu-id="3d975-137">String</span></span>|<span data-ttu-id="3d975-138">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3d975-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="3d975-139">url</span><span class="sxs-lookup"><span data-stu-id="3d975-139">url</span></span>|<span data-ttu-id="3d975-140">String</span><span class="sxs-lookup"><span data-stu-id="3d975-140">String</span></span>|<span data-ttu-id="3d975-141">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="3d975-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="3d975-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="3d975-142">appAuthorized</span></span>|<span data-ttu-id="3d975-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d975-143">Boolean</span></span>|<span data-ttu-id="3d975-144">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="3d975-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="3d975-145">enabled</span><span class="sxs-lookup"><span data-stu-id="3d975-145">enabled</span></span>|<span data-ttu-id="3d975-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d975-146">Boolean</span></span>|<span data-ttu-id="3d975-147">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="3d975-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="3d975-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="3d975-148">lastConnectionDateTime</span></span>|<span data-ttu-id="3d975-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d975-149">DateTimeOffset</span></span>|<span data-ttu-id="3d975-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="3d975-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="3d975-151">响应</span><span class="sxs-lookup"><span data-stu-id="3d975-151">Response</span></span>
<span data-ttu-id="3d975-152">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d975-152">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d975-153">示例</span><span class="sxs-lookup"><span data-stu-id="3d975-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d975-154">请求</span><span class="sxs-lookup"><span data-stu-id="3d975-154">Request</span></span>
<span data-ttu-id="3d975-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d975-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="3d975-156">响应</span><span class="sxs-lookup"><span data-stu-id="3d975-156">Response</span></span>
<span data-ttu-id="3d975-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d975-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




