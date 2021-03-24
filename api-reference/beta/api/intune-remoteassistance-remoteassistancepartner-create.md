---
title: 创建 remoteAssistancePartner
description: 创建新的 remoteAssistancePartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f8ca45d9cc8efc61a67708ca3595f1b4856e393
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134457"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="6ca06-103">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="6ca06-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="6ca06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ca06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ca06-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ca06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ca06-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ca06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ca06-107">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ca06-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ca06-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ca06-108">Prerequisites</span></span>
<span data-ttu-id="6ca06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ca06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ca06-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ca06-111">Permission type</span></span>|<span data-ttu-id="6ca06-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ca06-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ca06-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ca06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ca06-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ca06-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6ca06-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ca06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ca06-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ca06-116">Not supported.</span></span>|
|<span data-ttu-id="6ca06-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ca06-117">Application</span></span>|<span data-ttu-id="6ca06-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ca06-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ca06-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ca06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="6ca06-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ca06-120">Request headers</span></span>
|<span data-ttu-id="6ca06-121">标头</span><span class="sxs-lookup"><span data-stu-id="6ca06-121">Header</span></span>|<span data-ttu-id="6ca06-122">值</span><span class="sxs-lookup"><span data-stu-id="6ca06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ca06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ca06-123">Authorization</span></span>|<span data-ttu-id="6ca06-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ca06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ca06-125">接受</span><span class="sxs-lookup"><span data-stu-id="6ca06-125">Accept</span></span>|<span data-ttu-id="6ca06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ca06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ca06-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ca06-127">Request body</span></span>
<span data-ttu-id="6ca06-128">在请求正文中，提供 remoteAssistancePartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ca06-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="6ca06-129">下表显示创建 remoteAssistancePartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6ca06-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="6ca06-130">属性</span><span class="sxs-lookup"><span data-stu-id="6ca06-130">Property</span></span>|<span data-ttu-id="6ca06-131">类型</span><span class="sxs-lookup"><span data-stu-id="6ca06-131">Type</span></span>|<span data-ttu-id="6ca06-132">说明</span><span class="sxs-lookup"><span data-stu-id="6ca06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ca06-133">id</span><span class="sxs-lookup"><span data-stu-id="6ca06-133">id</span></span>|<span data-ttu-id="6ca06-134">String</span><span class="sxs-lookup"><span data-stu-id="6ca06-134">String</span></span>|<span data-ttu-id="6ca06-135">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6ca06-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="6ca06-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6ca06-136">displayName</span></span>|<span data-ttu-id="6ca06-137">String</span><span class="sxs-lookup"><span data-stu-id="6ca06-137">String</span></span>|<span data-ttu-id="6ca06-138">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ca06-138">Display name of the partner.</span></span>|
|<span data-ttu-id="6ca06-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="6ca06-139">onboardingUrl</span></span>|<span data-ttu-id="6ca06-140">String</span><span class="sxs-lookup"><span data-stu-id="6ca06-140">String</span></span>|<span data-ttu-id="6ca06-141">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="6ca06-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="6ca06-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="6ca06-142">onboardingStatus</span></span>|[<span data-ttu-id="6ca06-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="6ca06-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="6ca06-144">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="6ca06-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="6ca06-145">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="6ca06-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="6ca06-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="6ca06-146">lastConnectionDateTime</span></span>|<span data-ttu-id="6ca06-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ca06-147">DateTimeOffset</span></span>|<span data-ttu-id="6ca06-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="6ca06-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|
|<span data-ttu-id="6ca06-149">onboardingRequestExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="6ca06-149">onboardingRequestExpiryDateTime</span></span>|<span data-ttu-id="6ca06-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ca06-150">DateTimeOffset</span></span>|<span data-ttu-id="6ca06-151">当 OnboardingStatus 载入时，这是载入请求到期的日期时间。</span><span class="sxs-lookup"><span data-stu-id="6ca06-151">When the OnboardingStatus is Onboarding, This is the date time when the onboarding request expires.</span></span>|



## <a name="response"></a><span data-ttu-id="6ca06-152">响应</span><span class="sxs-lookup"><span data-stu-id="6ca06-152">Response</span></span>
<span data-ttu-id="6ca06-153">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ca06-153">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ca06-154">示例</span><span class="sxs-lookup"><span data-stu-id="6ca06-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ca06-155">请求</span><span class="sxs-lookup"><span data-stu-id="6ca06-155">Request</span></span>
<span data-ttu-id="6ca06-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ca06-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ca06-157">响应</span><span class="sxs-lookup"><span data-stu-id="6ca06-157">Response</span></span>
<span data-ttu-id="6ca06-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ca06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




