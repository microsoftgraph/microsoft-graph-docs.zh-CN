---
title: 更新 remoteAssistancePartner
description: 更新 remoteAssistancePartner 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6184bbed2e40dbb7477817d77385209f3d8dd245
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459293"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="3eccb-103">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="3eccb-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="3eccb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3eccb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3eccb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3eccb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3eccb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3eccb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eccb-107">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3eccb-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eccb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3eccb-108">Prerequisites</span></span>
<span data-ttu-id="3eccb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3eccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eccb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3eccb-111">Permission type</span></span>|<span data-ttu-id="3eccb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3eccb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eccb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3eccb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3eccb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eccb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3eccb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3eccb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eccb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3eccb-116">Not supported.</span></span>|
|<span data-ttu-id="3eccb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3eccb-117">Application</span></span>|<span data-ttu-id="3eccb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eccb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eccb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3eccb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="3eccb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3eccb-120">Request headers</span></span>
|<span data-ttu-id="3eccb-121">标头</span><span class="sxs-lookup"><span data-stu-id="3eccb-121">Header</span></span>|<span data-ttu-id="3eccb-122">值</span><span class="sxs-lookup"><span data-stu-id="3eccb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eccb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eccb-123">Authorization</span></span>|<span data-ttu-id="3eccb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3eccb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eccb-125">接受</span><span class="sxs-lookup"><span data-stu-id="3eccb-125">Accept</span></span>|<span data-ttu-id="3eccb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3eccb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eccb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3eccb-127">Request body</span></span>
<span data-ttu-id="3eccb-128">在请求正文中，提供 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3eccb-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="3eccb-129">下表显示创建 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3eccb-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="3eccb-130">属性</span><span class="sxs-lookup"><span data-stu-id="3eccb-130">Property</span></span>|<span data-ttu-id="3eccb-131">类型</span><span class="sxs-lookup"><span data-stu-id="3eccb-131">Type</span></span>|<span data-ttu-id="3eccb-132">说明</span><span class="sxs-lookup"><span data-stu-id="3eccb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eccb-133">id</span><span class="sxs-lookup"><span data-stu-id="3eccb-133">id</span></span>|<span data-ttu-id="3eccb-134">String</span><span class="sxs-lookup"><span data-stu-id="3eccb-134">String</span></span>|<span data-ttu-id="3eccb-135">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3eccb-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="3eccb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3eccb-136">displayName</span></span>|<span data-ttu-id="3eccb-137">字符串</span><span class="sxs-lookup"><span data-stu-id="3eccb-137">String</span></span>|<span data-ttu-id="3eccb-138">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3eccb-138">Display name of the partner.</span></span>|
|<span data-ttu-id="3eccb-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="3eccb-139">onboardingUrl</span></span>|<span data-ttu-id="3eccb-140">String</span><span class="sxs-lookup"><span data-stu-id="3eccb-140">String</span></span>|<span data-ttu-id="3eccb-141">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="3eccb-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="3eccb-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="3eccb-142">onboardingStatus</span></span>|[<span data-ttu-id="3eccb-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="3eccb-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="3eccb-144">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="3eccb-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="3eccb-145">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="3eccb-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="3eccb-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="3eccb-146">lastConnectionDateTime</span></span>|<span data-ttu-id="3eccb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eccb-147">DateTimeOffset</span></span>|<span data-ttu-id="3eccb-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="3eccb-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="3eccb-149">响应</span><span class="sxs-lookup"><span data-stu-id="3eccb-149">Response</span></span>
<span data-ttu-id="3eccb-150">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3eccb-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eccb-151">示例</span><span class="sxs-lookup"><span data-stu-id="3eccb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eccb-152">请求</span><span class="sxs-lookup"><span data-stu-id="3eccb-152">Request</span></span>
<span data-ttu-id="3eccb-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3eccb-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3eccb-154">响应</span><span class="sxs-lookup"><span data-stu-id="3eccb-154">Response</span></span>
<span data-ttu-id="3eccb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3eccb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```





