---
title: 更新 onPremisesConditionalAccessSettings
description: 更新 onPremisesConditionalAccessSettings 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 80aa93482b6d71a3367b58f2a78019e909cd089b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872980"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="93cd9-103">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="93cd9-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="93cd9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="93cd9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93cd9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="93cd9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93cd9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="93cd9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93cd9-107">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93cd9-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93cd9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="93cd9-108">Prerequisites</span></span>
<span data-ttu-id="93cd9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="93cd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93cd9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="93cd9-111">Permission type</span></span>|<span data-ttu-id="93cd9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93cd9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93cd9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93cd9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93cd9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93cd9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93cd9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93cd9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93cd9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="93cd9-116">Not supported.</span></span>|
|<span data-ttu-id="93cd9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="93cd9-117">Application</span></span>|<span data-ttu-id="93cd9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="93cd9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93cd9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93cd9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="93cd9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="93cd9-120">Request headers</span></span>
|<span data-ttu-id="93cd9-121">标头</span><span class="sxs-lookup"><span data-stu-id="93cd9-121">Header</span></span>|<span data-ttu-id="93cd9-122">值</span><span class="sxs-lookup"><span data-stu-id="93cd9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93cd9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="93cd9-123">Authorization</span></span>|<span data-ttu-id="93cd9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93cd9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93cd9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93cd9-125">Accept</span></span>|<span data-ttu-id="93cd9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93cd9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93cd9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93cd9-127">Request body</span></span>
<span data-ttu-id="93cd9-128">在请求正文中，提供 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93cd9-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="93cd9-129">下表显示创建 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93cd9-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="93cd9-130">属性</span><span class="sxs-lookup"><span data-stu-id="93cd9-130">Property</span></span>|<span data-ttu-id="93cd9-131">类型</span><span class="sxs-lookup"><span data-stu-id="93cd9-131">Type</span></span>|<span data-ttu-id="93cd9-132">说明</span><span class="sxs-lookup"><span data-stu-id="93cd9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93cd9-133">id</span><span class="sxs-lookup"><span data-stu-id="93cd9-133">id</span></span>|<span data-ttu-id="93cd9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="93cd9-134">String</span></span>|<span data-ttu-id="93cd9-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="93cd9-135">Not yet documented</span></span>|
|<span data-ttu-id="93cd9-136">enabled</span><span class="sxs-lookup"><span data-stu-id="93cd9-136">enabled</span></span>|<span data-ttu-id="93cd9-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="93cd9-137">Boolean</span></span>|<span data-ttu-id="93cd9-138">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="93cd9-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="93cd9-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="93cd9-139">includedGroups</span></span>|<span data-ttu-id="93cd9-140">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="93cd9-140">Guid collection</span></span>|<span data-ttu-id="93cd9-141">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="93cd9-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="93cd9-142">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="93cd9-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="93cd9-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="93cd9-143">excludedGroups</span></span>|<span data-ttu-id="93cd9-144">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="93cd9-144">Guid collection</span></span>|<span data-ttu-id="93cd9-145">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="93cd9-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="93cd9-146">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="93cd9-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="93cd9-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="93cd9-147">overrideDefaultRule</span></span>|<span data-ttu-id="93cd9-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="93cd9-148">Boolean</span></span>|<span data-ttu-id="93cd9-149">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="93cd9-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="93cd9-150">响应</span><span class="sxs-lookup"><span data-stu-id="93cd9-150">Response</span></span>
<span data-ttu-id="93cd9-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93cd9-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93cd9-152">示例</span><span class="sxs-lookup"><span data-stu-id="93cd9-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="93cd9-153">请求</span><span class="sxs-lookup"><span data-stu-id="93cd9-153">Request</span></span>
<span data-ttu-id="93cd9-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93cd9-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 201

{
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="93cd9-155">响应</span><span class="sxs-lookup"><span data-stu-id="93cd9-155">Response</span></span>
<span data-ttu-id="93cd9-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93cd9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```





