---
title: 更新 remoteAssistancePartner
description: 更新 remoteAssistancePartner 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1af8672541c0bc23e7f5af0df51964e8858cbf55
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756805"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="ad8b5-103">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ad8b5-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="ad8b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad8b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad8b5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad8b5-106">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-106">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad8b5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ad8b5-107">Prerequisites</span></span>
<span data-ttu-id="ad8b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad8b5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad8b5-110">Permission type</span></span>|<span data-ttu-id="ad8b5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad8b5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad8b5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad8b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad8b5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8b5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ad8b5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad8b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad8b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-115">Not supported.</span></span>|
|<span data-ttu-id="ad8b5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad8b5-116">Application</span></span>|<span data-ttu-id="ad8b5-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8b5-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad8b5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad8b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="ad8b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad8b5-119">Request headers</span></span>
|<span data-ttu-id="ad8b5-120">标头</span><span class="sxs-lookup"><span data-stu-id="ad8b5-120">Header</span></span>|<span data-ttu-id="ad8b5-121">值</span><span class="sxs-lookup"><span data-stu-id="ad8b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad8b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad8b5-122">Authorization</span></span>|<span data-ttu-id="ad8b5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad8b5-124">接受</span><span class="sxs-lookup"><span data-stu-id="ad8b5-124">Accept</span></span>|<span data-ttu-id="ad8b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad8b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad8b5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad8b5-126">Request body</span></span>
<span data-ttu-id="ad8b5-127">在请求正文中，提供 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-127">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="ad8b5-128">下表显示创建 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-128">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="ad8b5-129">属性</span><span class="sxs-lookup"><span data-stu-id="ad8b5-129">Property</span></span>|<span data-ttu-id="ad8b5-130">类型</span><span class="sxs-lookup"><span data-stu-id="ad8b5-130">Type</span></span>|<span data-ttu-id="ad8b5-131">说明</span><span class="sxs-lookup"><span data-stu-id="ad8b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad8b5-132">id</span><span class="sxs-lookup"><span data-stu-id="ad8b5-132">id</span></span>|<span data-ttu-id="ad8b5-133">String</span><span class="sxs-lookup"><span data-stu-id="ad8b5-133">String</span></span>|<span data-ttu-id="ad8b5-134">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="ad8b5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ad8b5-135">displayName</span></span>|<span data-ttu-id="ad8b5-136">String</span><span class="sxs-lookup"><span data-stu-id="ad8b5-136">String</span></span>|<span data-ttu-id="ad8b5-137">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-137">Display name of the partner.</span></span>|
|<span data-ttu-id="ad8b5-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="ad8b5-138">onboardingUrl</span></span>|<span data-ttu-id="ad8b5-139">String</span><span class="sxs-lookup"><span data-stu-id="ad8b5-139">String</span></span>|<span data-ttu-id="ad8b5-140">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="ad8b5-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="ad8b5-141">onboardingStatus</span></span>|[<span data-ttu-id="ad8b5-142">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="ad8b5-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="ad8b5-143">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-143">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="ad8b5-144">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="ad8b5-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ad8b5-145">lastConnectionDateTime</span></span>|<span data-ttu-id="ad8b5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad8b5-146">DateTimeOffset</span></span>|<span data-ttu-id="ad8b5-147">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="ad8b5-148">响应</span><span class="sxs-lookup"><span data-stu-id="ad8b5-148">Response</span></span>
<span data-ttu-id="ad8b5-149">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-149">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad8b5-150">示例</span><span class="sxs-lookup"><span data-stu-id="ad8b5-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad8b5-151">请求</span><span class="sxs-lookup"><span data-stu-id="ad8b5-151">Request</span></span>
<span data-ttu-id="ad8b5-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad8b5-153">响应</span><span class="sxs-lookup"><span data-stu-id="ad8b5-153">Response</span></span>
<span data-ttu-id="ad8b5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad8b5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




