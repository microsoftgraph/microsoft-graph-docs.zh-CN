---
title: 创建 remoteAssistancePartner
description: 创建新的 remoteAssistancePartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c218d01a2c8c3b60a6de75a677f722d0a49c05e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698384"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="35624-103">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="35624-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="35624-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35624-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35624-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35624-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35624-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35624-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35624-107">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35624-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35624-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="35624-108">Prerequisites</span></span>
<span data-ttu-id="35624-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35624-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="35624-111">Permission type</span></span>|<span data-ttu-id="35624-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35624-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35624-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35624-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35624-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35624-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="35624-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35624-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35624-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="35624-116">Not supported.</span></span>|
|<span data-ttu-id="35624-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="35624-117">Application</span></span>|<span data-ttu-id="35624-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35624-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35624-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35624-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="35624-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="35624-120">Request headers</span></span>
|<span data-ttu-id="35624-121">标头</span><span class="sxs-lookup"><span data-stu-id="35624-121">Header</span></span>|<span data-ttu-id="35624-122">值</span><span class="sxs-lookup"><span data-stu-id="35624-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35624-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35624-123">Authorization</span></span>|<span data-ttu-id="35624-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35624-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35624-125">接受</span><span class="sxs-lookup"><span data-stu-id="35624-125">Accept</span></span>|<span data-ttu-id="35624-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35624-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35624-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="35624-127">Request body</span></span>
<span data-ttu-id="35624-128">在请求正文中，提供 remoteAssistancePartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35624-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="35624-129">下表显示创建 remoteAssistancePartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35624-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="35624-130">属性</span><span class="sxs-lookup"><span data-stu-id="35624-130">Property</span></span>|<span data-ttu-id="35624-131">类型</span><span class="sxs-lookup"><span data-stu-id="35624-131">Type</span></span>|<span data-ttu-id="35624-132">说明</span><span class="sxs-lookup"><span data-stu-id="35624-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35624-133">id</span><span class="sxs-lookup"><span data-stu-id="35624-133">id</span></span>|<span data-ttu-id="35624-134">String</span><span class="sxs-lookup"><span data-stu-id="35624-134">String</span></span>|<span data-ttu-id="35624-135">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="35624-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="35624-136">displayName</span><span class="sxs-lookup"><span data-stu-id="35624-136">displayName</span></span>|<span data-ttu-id="35624-137">String</span><span class="sxs-lookup"><span data-stu-id="35624-137">String</span></span>|<span data-ttu-id="35624-138">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="35624-138">Display name of the partner.</span></span>|
|<span data-ttu-id="35624-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="35624-139">onboardingUrl</span></span>|<span data-ttu-id="35624-140">String</span><span class="sxs-lookup"><span data-stu-id="35624-140">String</span></span>|<span data-ttu-id="35624-141">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="35624-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="35624-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="35624-142">onboardingStatus</span></span>|[<span data-ttu-id="35624-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="35624-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="35624-144">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="35624-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="35624-145">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="35624-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="35624-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="35624-146">lastConnectionDateTime</span></span>|<span data-ttu-id="35624-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35624-147">DateTimeOffset</span></span>|<span data-ttu-id="35624-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="35624-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|
|<span data-ttu-id="35624-149">onboardingRequestExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="35624-149">onboardingRequestExpiryDateTime</span></span>|<span data-ttu-id="35624-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35624-150">DateTimeOffset</span></span>|<span data-ttu-id="35624-151">在载入 OnboardingStatus 时，这是启动请求过期的日期时间。</span><span class="sxs-lookup"><span data-stu-id="35624-151">When the OnboardingStatus is Onboarding, This is the date time when the onboarding request expires.</span></span>|



## <a name="response"></a><span data-ttu-id="35624-152">响应</span><span class="sxs-lookup"><span data-stu-id="35624-152">Response</span></span>
<span data-ttu-id="35624-153">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35624-153">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35624-154">示例</span><span class="sxs-lookup"><span data-stu-id="35624-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="35624-155">请求</span><span class="sxs-lookup"><span data-stu-id="35624-155">Request</span></span>
<span data-ttu-id="35624-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35624-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35624-157">响应</span><span class="sxs-lookup"><span data-stu-id="35624-157">Response</span></span>
<span data-ttu-id="35624-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35624-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





