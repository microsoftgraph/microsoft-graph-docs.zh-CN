---
title: 创建 remoteAssistancePartner
description: 创建新的 remoteAssistancePartner 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a10aade12fcfdbcb1a9b74722c480d52c98aefc1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194822"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="f10bd-103">创建 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="f10bd-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="f10bd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f10bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f10bd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f10bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f10bd-106">创建新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f10bd-106">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f10bd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f10bd-107">Prerequisites</span></span>
<span data-ttu-id="f10bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f10bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f10bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f10bd-110">Permission type</span></span>|<span data-ttu-id="f10bd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f10bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f10bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f10bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f10bd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10bd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f10bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f10bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f10bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f10bd-115">Not supported.</span></span>|
|<span data-ttu-id="f10bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f10bd-116">Application</span></span>|<span data-ttu-id="f10bd-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10bd-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f10bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f10bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="f10bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f10bd-119">Request headers</span></span>
|<span data-ttu-id="f10bd-120">标头</span><span class="sxs-lookup"><span data-stu-id="f10bd-120">Header</span></span>|<span data-ttu-id="f10bd-121">值</span><span class="sxs-lookup"><span data-stu-id="f10bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f10bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f10bd-122">Authorization</span></span>|<span data-ttu-id="f10bd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f10bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f10bd-124">接受</span><span class="sxs-lookup"><span data-stu-id="f10bd-124">Accept</span></span>|<span data-ttu-id="f10bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f10bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f10bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f10bd-126">Request body</span></span>
<span data-ttu-id="f10bd-127">在请求正文中，提供 remoteAssistancePartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f10bd-127">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="f10bd-128">下表显示创建 remoteAssistancePartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f10bd-128">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="f10bd-129">属性</span><span class="sxs-lookup"><span data-stu-id="f10bd-129">Property</span></span>|<span data-ttu-id="f10bd-130">类型</span><span class="sxs-lookup"><span data-stu-id="f10bd-130">Type</span></span>|<span data-ttu-id="f10bd-131">说明</span><span class="sxs-lookup"><span data-stu-id="f10bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f10bd-132">id</span><span class="sxs-lookup"><span data-stu-id="f10bd-132">id</span></span>|<span data-ttu-id="f10bd-133">String</span><span class="sxs-lookup"><span data-stu-id="f10bd-133">String</span></span>|<span data-ttu-id="f10bd-134">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f10bd-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="f10bd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f10bd-135">displayName</span></span>|<span data-ttu-id="f10bd-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f10bd-136">String</span></span>|<span data-ttu-id="f10bd-137">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f10bd-137">Display name of the partner.</span></span>|
|<span data-ttu-id="f10bd-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="f10bd-138">onboardingUrl</span></span>|<span data-ttu-id="f10bd-139">String</span><span class="sxs-lookup"><span data-stu-id="f10bd-139">String</span></span>|<span data-ttu-id="f10bd-140">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="f10bd-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="f10bd-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="f10bd-141">onboardingStatus</span></span>|[<span data-ttu-id="f10bd-142">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="f10bd-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="f10bd-143">当前 TeamViewer 连接器状态的友好说明。</span><span class="sxs-lookup"><span data-stu-id="f10bd-143">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="f10bd-144">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="f10bd-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="f10bd-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="f10bd-145">lastConnectionDateTime</span></span>|<span data-ttu-id="f10bd-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f10bd-146">DateTimeOffset</span></span>|<span data-ttu-id="f10bd-147">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="f10bd-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="f10bd-148">响应</span><span class="sxs-lookup"><span data-stu-id="f10bd-148">Response</span></span>
<span data-ttu-id="f10bd-149">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f10bd-149">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f10bd-150">示例</span><span class="sxs-lookup"><span data-stu-id="f10bd-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f10bd-151">请求</span><span class="sxs-lookup"><span data-stu-id="f10bd-151">Request</span></span>
<span data-ttu-id="f10bd-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f10bd-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="f10bd-153">响应</span><span class="sxs-lookup"><span data-stu-id="f10bd-153">Response</span></span>
<span data-ttu-id="f10bd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f10bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




