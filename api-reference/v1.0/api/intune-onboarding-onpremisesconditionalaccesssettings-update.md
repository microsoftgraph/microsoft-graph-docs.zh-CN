---
title: 更新 onPremisesConditionalAccessSettings
description: 更新 onPremisesConditionalAccessSettings 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7691e10a3877b9bb29bdc27e62b5d5790925513b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757973"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="e4e9f-103">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="e4e9f-103">Update onPremisesConditionalAccessSettings</span></span>

<span data-ttu-id="e4e9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4e9f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4e9f-106">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-106">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4e9f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4e9f-107">Prerequisites</span></span>
<span data-ttu-id="e4e9f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e9f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4e9f-110">Permission type</span></span>|<span data-ttu-id="e4e9f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4e9f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4e9f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e9f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4e9f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e9f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e4e9f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e9f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4e9f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-115">Not supported.</span></span>|
|<span data-ttu-id="e4e9f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4e9f-116">Application</span></span>|<span data-ttu-id="e4e9f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e9f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4e9f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4e9f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="e4e9f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4e9f-119">Request headers</span></span>
|<span data-ttu-id="e4e9f-120">标头</span><span class="sxs-lookup"><span data-stu-id="e4e9f-120">Header</span></span>|<span data-ttu-id="e4e9f-121">值</span><span class="sxs-lookup"><span data-stu-id="e4e9f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4e9f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4e9f-122">Authorization</span></span>|<span data-ttu-id="e4e9f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4e9f-124">接受</span><span class="sxs-lookup"><span data-stu-id="e4e9f-124">Accept</span></span>|<span data-ttu-id="e4e9f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4e9f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e9f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4e9f-126">Request body</span></span>
<span data-ttu-id="e4e9f-127">在请求正文中，提供 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-127">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="e4e9f-128">下表显示创建 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-128">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="e4e9f-129">属性</span><span class="sxs-lookup"><span data-stu-id="e4e9f-129">Property</span></span>|<span data-ttu-id="e4e9f-130">类型</span><span class="sxs-lookup"><span data-stu-id="e4e9f-130">Type</span></span>|<span data-ttu-id="e4e9f-131">说明</span><span class="sxs-lookup"><span data-stu-id="e4e9f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4e9f-132">id</span><span class="sxs-lookup"><span data-stu-id="e4e9f-132">id</span></span>|<span data-ttu-id="e4e9f-133">String</span><span class="sxs-lookup"><span data-stu-id="e4e9f-133">String</span></span>|<span data-ttu-id="e4e9f-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4e9f-134">Not yet documented</span></span>|
|<span data-ttu-id="e4e9f-135">enabled</span><span class="sxs-lookup"><span data-stu-id="e4e9f-135">enabled</span></span>|<span data-ttu-id="e4e9f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4e9f-136">Boolean</span></span>|<span data-ttu-id="e4e9f-137">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="e4e9f-137">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="e4e9f-138">includedGroups</span><span class="sxs-lookup"><span data-stu-id="e4e9f-138">includedGroups</span></span>|<span data-ttu-id="e4e9f-139">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="e4e9f-139">Guid collection</span></span>|<span data-ttu-id="e4e9f-140">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-140">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="e4e9f-141">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-141">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="e4e9f-142">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="e4e9f-142">excludedGroups</span></span>|<span data-ttu-id="e4e9f-143">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="e4e9f-143">Guid collection</span></span>|<span data-ttu-id="e4e9f-144">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-144">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="e4e9f-145">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-145">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="e4e9f-146">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="e4e9f-146">overrideDefaultRule</span></span>|<span data-ttu-id="e4e9f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4e9f-147">Boolean</span></span>|<span data-ttu-id="e4e9f-148">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-148">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="e4e9f-149">响应</span><span class="sxs-lookup"><span data-stu-id="e4e9f-149">Response</span></span>
<span data-ttu-id="e4e9f-150">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-150">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e9f-151">示例</span><span class="sxs-lookup"><span data-stu-id="e4e9f-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4e9f-152">请求</span><span class="sxs-lookup"><span data-stu-id="e4e9f-152">Request</span></span>
<span data-ttu-id="e4e9f-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4e9f-154">响应</span><span class="sxs-lookup"><span data-stu-id="e4e9f-154">Response</span></span>
<span data-ttu-id="e4e9f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4e9f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




