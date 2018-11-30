---
title: 更新 remoteAssistancePartner
description: 更新 remoteAssistancePartner 对象的属性。
ms.openlocfilehash: 62647e197d7c4666ce177fff6c2f1fb7dd1271af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043967"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="88a78-103">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="88a78-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="88a78-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88a78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88a78-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88a78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88a78-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88a78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88a78-107">更新 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88a78-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88a78-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88a78-108">Prerequisites</span></span>
<span data-ttu-id="88a78-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="88a78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a78-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88a78-111">Permission type</span></span>|<span data-ttu-id="88a78-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88a78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88a78-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88a78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88a78-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a78-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88a78-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88a78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88a78-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88a78-116">Not supported.</span></span>|
|<span data-ttu-id="88a78-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88a78-117">Application</span></span>|<span data-ttu-id="88a78-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="88a78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88a78-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88a78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="88a78-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88a78-120">Request headers</span></span>
|<span data-ttu-id="88a78-121">标头</span><span class="sxs-lookup"><span data-stu-id="88a78-121">Header</span></span>|<span data-ttu-id="88a78-122">值</span><span class="sxs-lookup"><span data-stu-id="88a78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88a78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88a78-123">Authorization</span></span>|<span data-ttu-id="88a78-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88a78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88a78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88a78-125">Accept</span></span>|<span data-ttu-id="88a78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88a78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88a78-127">Request body</span></span>
<span data-ttu-id="88a78-128">在请求正文中，提供 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88a78-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="88a78-129">下表显示创建 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88a78-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="88a78-130">属性</span><span class="sxs-lookup"><span data-stu-id="88a78-130">Property</span></span>|<span data-ttu-id="88a78-131">类型</span><span class="sxs-lookup"><span data-stu-id="88a78-131">Type</span></span>|<span data-ttu-id="88a78-132">说明</span><span class="sxs-lookup"><span data-stu-id="88a78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a78-133">id</span><span class="sxs-lookup"><span data-stu-id="88a78-133">id</span></span>|<span data-ttu-id="88a78-134">String</span><span class="sxs-lookup"><span data-stu-id="88a78-134">String</span></span>|<span data-ttu-id="88a78-135">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="88a78-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="88a78-136">displayName</span><span class="sxs-lookup"><span data-stu-id="88a78-136">displayName</span></span>|<span data-ttu-id="88a78-137">String</span><span class="sxs-lookup"><span data-stu-id="88a78-137">String</span></span>|<span data-ttu-id="88a78-138">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="88a78-138">Display name of the partner.</span></span>|
|<span data-ttu-id="88a78-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="88a78-139">onboardingUrl</span></span>|<span data-ttu-id="88a78-140">String</span><span class="sxs-lookup"><span data-stu-id="88a78-140">String</span></span>|<span data-ttu-id="88a78-141">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="88a78-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="88a78-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="88a78-142">onboardingStatus</span></span>|[<span data-ttu-id="88a78-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="88a78-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="88a78-144">TBD。</span><span class="sxs-lookup"><span data-stu-id="88a78-144">TBD.</span></span> <span data-ttu-id="88a78-145">可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="88a78-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="88a78-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="88a78-146">lastConnectionDateTime</span></span>|<span data-ttu-id="88a78-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a78-147">DateTimeOffset</span></span>|<span data-ttu-id="88a78-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="88a78-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="88a78-149">响应</span><span class="sxs-lookup"><span data-stu-id="88a78-149">Response</span></span>
<span data-ttu-id="88a78-150">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88a78-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88a78-151">示例</span><span class="sxs-lookup"><span data-stu-id="88a78-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="88a78-152">请求</span><span class="sxs-lookup"><span data-stu-id="88a78-152">Request</span></span>
<span data-ttu-id="88a78-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88a78-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="88a78-154">响应</span><span class="sxs-lookup"><span data-stu-id="88a78-154">Response</span></span>
<span data-ttu-id="88a78-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88a78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





