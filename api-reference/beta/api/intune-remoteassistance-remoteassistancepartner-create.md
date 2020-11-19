---
title: 创建 remoteAssistancePartner
description: 创建新的 remoteAssistancePartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d140b49e0052350c897840ff6a61453430c309f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304320"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="da2da-103">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="da2da-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="da2da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da2da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da2da-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da2da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da2da-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da2da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da2da-107">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da2da-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da2da-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da2da-108">Prerequisites</span></span>
<span data-ttu-id="da2da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da2da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da2da-111">Permission type</span></span>|<span data-ttu-id="da2da-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da2da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da2da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da2da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da2da-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2da-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="da2da-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da2da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da2da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da2da-116">Not supported.</span></span>|
|<span data-ttu-id="da2da-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da2da-117">Application</span></span>|<span data-ttu-id="da2da-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2da-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da2da-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da2da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="da2da-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da2da-120">Request headers</span></span>
|<span data-ttu-id="da2da-121">标头</span><span class="sxs-lookup"><span data-stu-id="da2da-121">Header</span></span>|<span data-ttu-id="da2da-122">值</span><span class="sxs-lookup"><span data-stu-id="da2da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da2da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2da-123">Authorization</span></span>|<span data-ttu-id="da2da-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da2da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da2da-125">接受</span><span class="sxs-lookup"><span data-stu-id="da2da-125">Accept</span></span>|<span data-ttu-id="da2da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da2da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da2da-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da2da-127">Request body</span></span>
<span data-ttu-id="da2da-128">在请求正文中，提供 remoteAssistancePartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da2da-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="da2da-129">下表显示创建 remoteAssistancePartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da2da-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="da2da-130">属性</span><span class="sxs-lookup"><span data-stu-id="da2da-130">Property</span></span>|<span data-ttu-id="da2da-131">类型</span><span class="sxs-lookup"><span data-stu-id="da2da-131">Type</span></span>|<span data-ttu-id="da2da-132">说明</span><span class="sxs-lookup"><span data-stu-id="da2da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2da-133">id</span><span class="sxs-lookup"><span data-stu-id="da2da-133">id</span></span>|<span data-ttu-id="da2da-134">字符串</span><span class="sxs-lookup"><span data-stu-id="da2da-134">String</span></span>|<span data-ttu-id="da2da-135">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="da2da-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="da2da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="da2da-136">displayName</span></span>|<span data-ttu-id="da2da-137">字符串</span><span class="sxs-lookup"><span data-stu-id="da2da-137">String</span></span>|<span data-ttu-id="da2da-138">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="da2da-138">Display name of the partner.</span></span>|
|<span data-ttu-id="da2da-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="da2da-139">onboardingUrl</span></span>|<span data-ttu-id="da2da-140">String</span><span class="sxs-lookup"><span data-stu-id="da2da-140">String</span></span>|<span data-ttu-id="da2da-141">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="da2da-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="da2da-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="da2da-142">onboardingStatus</span></span>|[<span data-ttu-id="da2da-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="da2da-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="da2da-144">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="da2da-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="da2da-145">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="da2da-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="da2da-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="da2da-146">lastConnectionDateTime</span></span>|<span data-ttu-id="da2da-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da2da-147">DateTimeOffset</span></span>|<span data-ttu-id="da2da-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="da2da-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|
|<span data-ttu-id="da2da-149">onboardingRequestExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="da2da-149">onboardingRequestExpiryDateTime</span></span>|<span data-ttu-id="da2da-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da2da-150">DateTimeOffset</span></span>|<span data-ttu-id="da2da-151">在载入 OnboardingStatus 时，这是启动请求过期的日期时间。</span><span class="sxs-lookup"><span data-stu-id="da2da-151">When the OnboardingStatus is Onboarding, This is the date time when the onboarding request expires.</span></span>|



## <a name="response"></a><span data-ttu-id="da2da-152">响应</span><span class="sxs-lookup"><span data-stu-id="da2da-152">Response</span></span>
<span data-ttu-id="da2da-153">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da2da-153">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da2da-154">示例</span><span class="sxs-lookup"><span data-stu-id="da2da-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="da2da-155">请求</span><span class="sxs-lookup"><span data-stu-id="da2da-155">Request</span></span>
<span data-ttu-id="da2da-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da2da-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 341

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "onboardingRequestExpiryDateTime": "2017-01-01T00:02:07.7573274-08:00"
}
```

### <a name="response"></a><span data-ttu-id="da2da-157">响应</span><span class="sxs-lookup"><span data-stu-id="da2da-157">Response</span></span>
<span data-ttu-id="da2da-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da2da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 390

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "onboardingRequestExpiryDateTime": "2017-01-01T00:02:07.7573274-08:00"
}
```




