---
title: 更新 remoteAssistancePartner
description: 更新 remoteAssistancePartner 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40a21ce7c0e5cf8ad525dfa44ffc8a6657c7cf13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512137"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="c552e-103">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="c552e-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="c552e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c552e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c552e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c552e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c552e-106">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c552e-106">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c552e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c552e-107">Prerequisites</span></span>
<span data-ttu-id="c552e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c552e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c552e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c552e-110">Permission type</span></span>|<span data-ttu-id="c552e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c552e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c552e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c552e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c552e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c552e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c552e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c552e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c552e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c552e-115">Not supported.</span></span>|
|<span data-ttu-id="c552e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c552e-116">Application</span></span>|<span data-ttu-id="c552e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c552e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c552e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c552e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="c552e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c552e-119">Request headers</span></span>
|<span data-ttu-id="c552e-120">标头</span><span class="sxs-lookup"><span data-stu-id="c552e-120">Header</span></span>|<span data-ttu-id="c552e-121">值</span><span class="sxs-lookup"><span data-stu-id="c552e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c552e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c552e-122">Authorization</span></span>|<span data-ttu-id="c552e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c552e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c552e-124">接受</span><span class="sxs-lookup"><span data-stu-id="c552e-124">Accept</span></span>|<span data-ttu-id="c552e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c552e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c552e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c552e-126">Request body</span></span>
<span data-ttu-id="c552e-127">在请求正文中，提供 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c552e-127">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="c552e-128">下表显示创建 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c552e-128">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="c552e-129">属性</span><span class="sxs-lookup"><span data-stu-id="c552e-129">Property</span></span>|<span data-ttu-id="c552e-130">类型</span><span class="sxs-lookup"><span data-stu-id="c552e-130">Type</span></span>|<span data-ttu-id="c552e-131">说明</span><span class="sxs-lookup"><span data-stu-id="c552e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c552e-132">id</span><span class="sxs-lookup"><span data-stu-id="c552e-132">id</span></span>|<span data-ttu-id="c552e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c552e-133">String</span></span>|<span data-ttu-id="c552e-134">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c552e-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="c552e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c552e-135">displayName</span></span>|<span data-ttu-id="c552e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="c552e-136">String</span></span>|<span data-ttu-id="c552e-137">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c552e-137">Display name of the partner.</span></span>|
|<span data-ttu-id="c552e-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="c552e-138">onboardingUrl</span></span>|<span data-ttu-id="c552e-139">String</span><span class="sxs-lookup"><span data-stu-id="c552e-139">String</span></span>|<span data-ttu-id="c552e-140">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="c552e-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="c552e-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c552e-141">onboardingStatus</span></span>|[<span data-ttu-id="c552e-142">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c552e-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="c552e-143">待定.</span><span class="sxs-lookup"><span data-stu-id="c552e-143">TBD.</span></span> <span data-ttu-id="c552e-144">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="c552e-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="c552e-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c552e-145">lastConnectionDateTime</span></span>|<span data-ttu-id="c552e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c552e-146">DateTimeOffset</span></span>|<span data-ttu-id="c552e-147">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c552e-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c552e-148">响应</span><span class="sxs-lookup"><span data-stu-id="c552e-148">Response</span></span>
<span data-ttu-id="c552e-149">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c552e-149">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c552e-150">示例</span><span class="sxs-lookup"><span data-stu-id="c552e-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c552e-151">请求</span><span class="sxs-lookup"><span data-stu-id="c552e-151">Request</span></span>
<span data-ttu-id="c552e-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c552e-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c552e-153">响应</span><span class="sxs-lookup"><span data-stu-id="c552e-153">Response</span></span>
<span data-ttu-id="c552e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c552e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




