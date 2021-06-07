---
title: 创建 remoteAssistancePartner
description: 创建新的 remoteAssistancePartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a1da12ef0e782adfb1b80a15cb5a3bfad203ebf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759028"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="53825-103">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="53825-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="53825-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53825-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53825-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53825-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53825-106">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53825-106">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53825-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="53825-107">Prerequisites</span></span>
<span data-ttu-id="53825-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53825-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53825-110">Permission type</span></span>|<span data-ttu-id="53825-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53825-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53825-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53825-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53825-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53825-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53825-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53825-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53825-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53825-115">Not supported.</span></span>|
|<span data-ttu-id="53825-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53825-116">Application</span></span>|<span data-ttu-id="53825-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53825-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53825-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53825-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="53825-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53825-119">Request headers</span></span>
|<span data-ttu-id="53825-120">标头</span><span class="sxs-lookup"><span data-stu-id="53825-120">Header</span></span>|<span data-ttu-id="53825-121">值</span><span class="sxs-lookup"><span data-stu-id="53825-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53825-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53825-122">Authorization</span></span>|<span data-ttu-id="53825-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53825-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53825-124">接受</span><span class="sxs-lookup"><span data-stu-id="53825-124">Accept</span></span>|<span data-ttu-id="53825-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53825-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53825-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="53825-126">Request body</span></span>
<span data-ttu-id="53825-127">在请求正文中，提供 remoteAssistancePartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53825-127">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="53825-128">下表显示创建 remoteAssistancePartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53825-128">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="53825-129">属性</span><span class="sxs-lookup"><span data-stu-id="53825-129">Property</span></span>|<span data-ttu-id="53825-130">类型</span><span class="sxs-lookup"><span data-stu-id="53825-130">Type</span></span>|<span data-ttu-id="53825-131">说明</span><span class="sxs-lookup"><span data-stu-id="53825-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53825-132">id</span><span class="sxs-lookup"><span data-stu-id="53825-132">id</span></span>|<span data-ttu-id="53825-133">String</span><span class="sxs-lookup"><span data-stu-id="53825-133">String</span></span>|<span data-ttu-id="53825-134">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="53825-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="53825-135">displayName</span><span class="sxs-lookup"><span data-stu-id="53825-135">displayName</span></span>|<span data-ttu-id="53825-136">String</span><span class="sxs-lookup"><span data-stu-id="53825-136">String</span></span>|<span data-ttu-id="53825-137">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="53825-137">Display name of the partner.</span></span>|
|<span data-ttu-id="53825-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="53825-138">onboardingUrl</span></span>|<span data-ttu-id="53825-139">String</span><span class="sxs-lookup"><span data-stu-id="53825-139">String</span></span>|<span data-ttu-id="53825-140">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="53825-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="53825-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="53825-141">onboardingStatus</span></span>|[<span data-ttu-id="53825-142">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="53825-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="53825-143">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="53825-143">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="53825-144">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="53825-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="53825-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="53825-145">lastConnectionDateTime</span></span>|<span data-ttu-id="53825-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53825-146">DateTimeOffset</span></span>|<span data-ttu-id="53825-147">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="53825-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="53825-148">响应</span><span class="sxs-lookup"><span data-stu-id="53825-148">Response</span></span>
<span data-ttu-id="53825-149">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53825-149">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53825-150">示例</span><span class="sxs-lookup"><span data-stu-id="53825-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="53825-151">请求</span><span class="sxs-lookup"><span data-stu-id="53825-151">Request</span></span>
<span data-ttu-id="53825-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53825-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="53825-153">响应</span><span class="sxs-lookup"><span data-stu-id="53825-153">Response</span></span>
<span data-ttu-id="53825-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53825-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




