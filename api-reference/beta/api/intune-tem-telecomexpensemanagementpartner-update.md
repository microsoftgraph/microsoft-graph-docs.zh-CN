---
title: 更新 telecomExpenseManagementPartner
description: 更新 telecomExpenseManagementPartner 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6b757c86fe3ddca1c7a86caa7c44888973a651f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123411"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="edc49-103">更新 telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="edc49-103">Update telecomExpenseManagementPartner</span></span>

<span data-ttu-id="edc49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edc49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edc49-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edc49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edc49-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edc49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edc49-107">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="edc49-107">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edc49-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="edc49-108">Prerequisites</span></span>
<span data-ttu-id="edc49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edc49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edc49-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="edc49-111">Permission type</span></span>|<span data-ttu-id="edc49-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edc49-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edc49-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edc49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edc49-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc49-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="edc49-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edc49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edc49-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc49-116">Not supported.</span></span>|
|<span data-ttu-id="edc49-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="edc49-117">Application</span></span>|<span data-ttu-id="edc49-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc49-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edc49-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edc49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="edc49-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="edc49-120">Request headers</span></span>
|<span data-ttu-id="edc49-121">标头</span><span class="sxs-lookup"><span data-stu-id="edc49-121">Header</span></span>|<span data-ttu-id="edc49-122">值</span><span class="sxs-lookup"><span data-stu-id="edc49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edc49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edc49-123">Authorization</span></span>|<span data-ttu-id="edc49-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="edc49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edc49-125">接受</span><span class="sxs-lookup"><span data-stu-id="edc49-125">Accept</span></span>|<span data-ttu-id="edc49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edc49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edc49-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="edc49-127">Request body</span></span>
<span data-ttu-id="edc49-128">在请求正文中，提供 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc49-128">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="edc49-129">下表显示创建 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="edc49-129">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="edc49-130">属性</span><span class="sxs-lookup"><span data-stu-id="edc49-130">Property</span></span>|<span data-ttu-id="edc49-131">类型</span><span class="sxs-lookup"><span data-stu-id="edc49-131">Type</span></span>|<span data-ttu-id="edc49-132">说明</span><span class="sxs-lookup"><span data-stu-id="edc49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc49-133">id</span><span class="sxs-lookup"><span data-stu-id="edc49-133">id</span></span>|<span data-ttu-id="edc49-134">String</span><span class="sxs-lookup"><span data-stu-id="edc49-134">String</span></span>|<span data-ttu-id="edc49-135">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="edc49-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="edc49-136">displayName</span><span class="sxs-lookup"><span data-stu-id="edc49-136">displayName</span></span>|<span data-ttu-id="edc49-137">String</span><span class="sxs-lookup"><span data-stu-id="edc49-137">String</span></span>|<span data-ttu-id="edc49-138">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="edc49-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="edc49-139">url</span><span class="sxs-lookup"><span data-stu-id="edc49-139">url</span></span>|<span data-ttu-id="edc49-140">String</span><span class="sxs-lookup"><span data-stu-id="edc49-140">String</span></span>|<span data-ttu-id="edc49-141">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="edc49-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="edc49-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="edc49-142">appAuthorized</span></span>|<span data-ttu-id="edc49-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="edc49-143">Boolean</span></span>|<span data-ttu-id="edc49-144">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="edc49-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="edc49-145">enabled</span><span class="sxs-lookup"><span data-stu-id="edc49-145">enabled</span></span>|<span data-ttu-id="edc49-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="edc49-146">Boolean</span></span>|<span data-ttu-id="edc49-147">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="edc49-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="edc49-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="edc49-148">lastConnectionDateTime</span></span>|<span data-ttu-id="edc49-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edc49-149">DateTimeOffset</span></span>|<span data-ttu-id="edc49-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="edc49-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="edc49-151">响应</span><span class="sxs-lookup"><span data-stu-id="edc49-151">Response</span></span>
<span data-ttu-id="edc49-152">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edc49-152">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edc49-153">示例</span><span class="sxs-lookup"><span data-stu-id="edc49-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="edc49-154">请求</span><span class="sxs-lookup"><span data-stu-id="edc49-154">Request</span></span>
<span data-ttu-id="edc49-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="edc49-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="edc49-156">响应</span><span class="sxs-lookup"><span data-stu-id="edc49-156">Response</span></span>
<span data-ttu-id="edc49-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="edc49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




