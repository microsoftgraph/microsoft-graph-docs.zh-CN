---
title: 更新 onPremisesConditionalAccessSettings
description: 更新 onPremisesConditionalAccessSettings 对象的属性。
author: tfitzmac
ms.openlocfilehash: 255693dfa1bb53083f792da950333a5c05717f1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346800"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="e55b0-103">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="e55b0-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="e55b0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e55b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e55b0-105">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e55b0-105">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e55b0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e55b0-106">Prerequisites</span></span>
<span data-ttu-id="e55b0-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e55b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e55b0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e55b0-109">Permission type</span></span>|<span data-ttu-id="e55b0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e55b0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e55b0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e55b0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e55b0-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e55b0-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e55b0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e55b0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e55b0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e55b0-114">Not supported.</span></span>|
|<span data-ttu-id="e55b0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e55b0-115">Application</span></span>|<span data-ttu-id="e55b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e55b0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e55b0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e55b0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="e55b0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e55b0-118">Request headers</span></span>
|<span data-ttu-id="e55b0-119">标头</span><span class="sxs-lookup"><span data-stu-id="e55b0-119">Header</span></span>|<span data-ttu-id="e55b0-120">值</span><span class="sxs-lookup"><span data-stu-id="e55b0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e55b0-121">授权</span><span class="sxs-lookup"><span data-stu-id="e55b0-121">Authorization</span></span>|<span data-ttu-id="e55b0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e55b0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e55b0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e55b0-123">Accept</span></span>|<span data-ttu-id="e55b0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e55b0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e55b0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e55b0-125">Request body</span></span>
<span data-ttu-id="e55b0-126">在请求正文中，提供 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e55b0-126">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="e55b0-127">下表显示创建 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e55b0-127">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="e55b0-128">属性</span><span class="sxs-lookup"><span data-stu-id="e55b0-128">Property</span></span>|<span data-ttu-id="e55b0-129">类型</span><span class="sxs-lookup"><span data-stu-id="e55b0-129">Type</span></span>|<span data-ttu-id="e55b0-130">说明</span><span class="sxs-lookup"><span data-stu-id="e55b0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e55b0-131">id</span><span class="sxs-lookup"><span data-stu-id="e55b0-131">id</span></span>|<span data-ttu-id="e55b0-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e55b0-132">String</span></span>|<span data-ttu-id="e55b0-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e55b0-133">Not yet documented</span></span>|
|<span data-ttu-id="e55b0-134">enabled</span><span class="sxs-lookup"><span data-stu-id="e55b0-134">enabled</span></span>|<span data-ttu-id="e55b0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e55b0-135">Boolean</span></span>|<span data-ttu-id="e55b0-136">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="e55b0-136">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="e55b0-137">includedGroups</span><span class="sxs-lookup"><span data-stu-id="e55b0-137">includedGroups</span></span>|<span data-ttu-id="e55b0-138">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="e55b0-138">Guid collection</span></span>|<span data-ttu-id="e55b0-139">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="e55b0-139">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="e55b0-140">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="e55b0-140">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="e55b0-141">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="e55b0-141">excludedGroups</span></span>|<span data-ttu-id="e55b0-142">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="e55b0-142">Guid collection</span></span>|<span data-ttu-id="e55b0-143">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="e55b0-143">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="e55b0-144">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="e55b0-144">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="e55b0-145">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="e55b0-145">overrideDefaultRule</span></span>|<span data-ttu-id="e55b0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e55b0-146">Boolean</span></span>|<span data-ttu-id="e55b0-147">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="e55b0-147">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="e55b0-148">响应</span><span class="sxs-lookup"><span data-stu-id="e55b0-148">Response</span></span>
<span data-ttu-id="e55b0-149">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e55b0-149">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e55b0-150">示例</span><span class="sxs-lookup"><span data-stu-id="e55b0-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="e55b0-151">请求</span><span class="sxs-lookup"><span data-stu-id="e55b0-151">Request</span></span>
<span data-ttu-id="e55b0-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e55b0-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
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

### <a name="response"></a><span data-ttu-id="e55b0-153">响应</span><span class="sxs-lookup"><span data-stu-id="e55b0-153">Response</span></span>
<span data-ttu-id="e55b0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e55b0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



