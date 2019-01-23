---
title: 更新 onPremisesConditionalAccessSettings
description: 更新 onPremisesConditionalAccessSettings 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: efd5ba18c958bd09e10a461350b76eb97aa56cb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424033"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="48af1-103">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="48af1-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="48af1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="48af1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48af1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48af1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48af1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48af1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48af1-107">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48af1-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48af1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="48af1-108">Prerequisites</span></span>
<span data-ttu-id="48af1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="48af1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48af1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48af1-111">Permission type</span></span>|<span data-ttu-id="48af1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48af1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48af1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48af1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48af1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48af1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48af1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48af1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48af1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48af1-116">Not supported.</span></span>|
|<span data-ttu-id="48af1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48af1-117">Application</span></span>|<span data-ttu-id="48af1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="48af1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48af1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48af1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="48af1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="48af1-120">Request headers</span></span>
|<span data-ttu-id="48af1-121">标头</span><span class="sxs-lookup"><span data-stu-id="48af1-121">Header</span></span>|<span data-ttu-id="48af1-122">值</span><span class="sxs-lookup"><span data-stu-id="48af1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48af1-123">授权</span><span class="sxs-lookup"><span data-stu-id="48af1-123">Authorization</span></span>|<span data-ttu-id="48af1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48af1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48af1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48af1-125">Accept</span></span>|<span data-ttu-id="48af1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48af1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48af1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="48af1-127">Request body</span></span>
<span data-ttu-id="48af1-128">在请求正文中，提供 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48af1-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="48af1-129">下表显示创建 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="48af1-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="48af1-130">属性</span><span class="sxs-lookup"><span data-stu-id="48af1-130">Property</span></span>|<span data-ttu-id="48af1-131">类型</span><span class="sxs-lookup"><span data-stu-id="48af1-131">Type</span></span>|<span data-ttu-id="48af1-132">说明</span><span class="sxs-lookup"><span data-stu-id="48af1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48af1-133">id</span><span class="sxs-lookup"><span data-stu-id="48af1-133">id</span></span>|<span data-ttu-id="48af1-134">String</span><span class="sxs-lookup"><span data-stu-id="48af1-134">String</span></span>|<span data-ttu-id="48af1-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="48af1-135">Not yet documented</span></span>|
|<span data-ttu-id="48af1-136">enabled</span><span class="sxs-lookup"><span data-stu-id="48af1-136">enabled</span></span>|<span data-ttu-id="48af1-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="48af1-137">Boolean</span></span>|<span data-ttu-id="48af1-138">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="48af1-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="48af1-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="48af1-139">includedGroups</span></span>|<span data-ttu-id="48af1-140">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="48af1-140">Guid collection</span></span>|<span data-ttu-id="48af1-141">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="48af1-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="48af1-142">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="48af1-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="48af1-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="48af1-143">excludedGroups</span></span>|<span data-ttu-id="48af1-144">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="48af1-144">Guid collection</span></span>|<span data-ttu-id="48af1-145">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="48af1-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="48af1-146">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="48af1-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="48af1-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="48af1-147">overrideDefaultRule</span></span>|<span data-ttu-id="48af1-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="48af1-148">Boolean</span></span>|<span data-ttu-id="48af1-149">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="48af1-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="48af1-150">响应</span><span class="sxs-lookup"><span data-stu-id="48af1-150">Response</span></span>
<span data-ttu-id="48af1-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48af1-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48af1-152">示例</span><span class="sxs-lookup"><span data-stu-id="48af1-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="48af1-153">请求</span><span class="sxs-lookup"><span data-stu-id="48af1-153">Request</span></span>
<span data-ttu-id="48af1-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48af1-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
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

### <a name="response"></a><span data-ttu-id="48af1-155">响应</span><span class="sxs-lookup"><span data-stu-id="48af1-155">Response</span></span>
<span data-ttu-id="48af1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48af1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




