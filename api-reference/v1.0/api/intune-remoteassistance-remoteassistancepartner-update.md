---
title: 更新 remoteAssistancePartner
description: 更新 remoteAssistancePartner 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16b7c3f9d3125ca688f08faa22772c4335e02a8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871398"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="cd220-103">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="cd220-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="cd220-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cd220-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd220-105">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cd220-105">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd220-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd220-106">Prerequisites</span></span>
<span data-ttu-id="cd220-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cd220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd220-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd220-109">Permission type</span></span>|<span data-ttu-id="cd220-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd220-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd220-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd220-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd220-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd220-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd220-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd220-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd220-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd220-114">Not supported.</span></span>|
|<span data-ttu-id="cd220-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd220-115">Application</span></span>|<span data-ttu-id="cd220-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd220-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd220-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd220-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="cd220-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd220-118">Request headers</span></span>
|<span data-ttu-id="cd220-119">标头</span><span class="sxs-lookup"><span data-stu-id="cd220-119">Header</span></span>|<span data-ttu-id="cd220-120">值</span><span class="sxs-lookup"><span data-stu-id="cd220-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd220-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd220-121">Authorization</span></span>|<span data-ttu-id="cd220-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd220-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd220-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cd220-123">Accept</span></span>|<span data-ttu-id="cd220-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cd220-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd220-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd220-125">Request body</span></span>
<span data-ttu-id="cd220-126">在请求正文中，提供 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd220-126">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="cd220-127">下表显示创建 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cd220-127">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="cd220-128">属性</span><span class="sxs-lookup"><span data-stu-id="cd220-128">Property</span></span>|<span data-ttu-id="cd220-129">类型</span><span class="sxs-lookup"><span data-stu-id="cd220-129">Type</span></span>|<span data-ttu-id="cd220-130">说明</span><span class="sxs-lookup"><span data-stu-id="cd220-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd220-131">id</span><span class="sxs-lookup"><span data-stu-id="cd220-131">id</span></span>|<span data-ttu-id="cd220-132">String</span><span class="sxs-lookup"><span data-stu-id="cd220-132">String</span></span>|<span data-ttu-id="cd220-133">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cd220-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="cd220-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cd220-134">displayName</span></span>|<span data-ttu-id="cd220-135">String</span><span class="sxs-lookup"><span data-stu-id="cd220-135">String</span></span>|<span data-ttu-id="cd220-136">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cd220-136">Display name of the partner.</span></span>|
|<span data-ttu-id="cd220-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="cd220-137">onboardingUrl</span></span>|<span data-ttu-id="cd220-138">String</span><span class="sxs-lookup"><span data-stu-id="cd220-138">String</span></span>|<span data-ttu-id="cd220-139">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="cd220-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="cd220-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="cd220-140">onboardingStatus</span></span>|[<span data-ttu-id="cd220-141">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="cd220-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="cd220-142">TBD。</span><span class="sxs-lookup"><span data-stu-id="cd220-142">TBD.</span></span> <span data-ttu-id="cd220-143">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="cd220-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="cd220-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="cd220-144">lastConnectionDateTime</span></span>|<span data-ttu-id="cd220-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd220-145">DateTimeOffset</span></span>|<span data-ttu-id="cd220-146">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="cd220-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="cd220-147">响应</span><span class="sxs-lookup"><span data-stu-id="cd220-147">Response</span></span>
<span data-ttu-id="cd220-148">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd220-148">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd220-149">示例</span><span class="sxs-lookup"><span data-stu-id="cd220-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd220-150">请求</span><span class="sxs-lookup"><span data-stu-id="cd220-150">Request</span></span>
<span data-ttu-id="cd220-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd220-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
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

### <a name="response"></a><span data-ttu-id="cd220-152">响应</span><span class="sxs-lookup"><span data-stu-id="cd220-152">Response</span></span>
<span data-ttu-id="cd220-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd220-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



