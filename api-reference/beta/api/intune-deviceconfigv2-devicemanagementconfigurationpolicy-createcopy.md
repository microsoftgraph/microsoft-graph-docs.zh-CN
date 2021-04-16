---
title: createCopy 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 353c55305eb0a09cdf26beecf1cf5e222338af3b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868482"
---
# <a name="createcopy-action"></a><span data-ttu-id="3f09f-103">createCopy 操作</span><span class="sxs-lookup"><span data-stu-id="3f09f-103">createCopy action</span></span>

<span data-ttu-id="3f09f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f09f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f09f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f09f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f09f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f09f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f09f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f09f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f09f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f09f-108">Prerequisites</span></span>
<span data-ttu-id="3f09f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f09f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f09f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f09f-111">Permission type</span></span>|<span data-ttu-id="3f09f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f09f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f09f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f09f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f09f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f09f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f09f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f09f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f09f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f09f-116">Not supported.</span></span>|
|<span data-ttu-id="3f09f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f09f-117">Application</span></span>|<span data-ttu-id="3f09f-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f09f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f09f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f09f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy
```

## <a name="request-headers"></a><span data-ttu-id="3f09f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f09f-120">Request headers</span></span>
|<span data-ttu-id="3f09f-121">标头</span><span class="sxs-lookup"><span data-stu-id="3f09f-121">Header</span></span>|<span data-ttu-id="3f09f-122">值</span><span class="sxs-lookup"><span data-stu-id="3f09f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f09f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f09f-123">Authorization</span></span>|<span data-ttu-id="3f09f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f09f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f09f-125">接受</span><span class="sxs-lookup"><span data-stu-id="3f09f-125">Accept</span></span>|<span data-ttu-id="3f09f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f09f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f09f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f09f-127">Request body</span></span>
<span data-ttu-id="3f09f-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f09f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3f09f-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="3f09f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3f09f-130">属性</span><span class="sxs-lookup"><span data-stu-id="3f09f-130">Property</span></span>|<span data-ttu-id="3f09f-131">类型</span><span class="sxs-lookup"><span data-stu-id="3f09f-131">Type</span></span>|<span data-ttu-id="3f09f-132">说明</span><span class="sxs-lookup"><span data-stu-id="3f09f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f09f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3f09f-133">displayName</span></span>|<span data-ttu-id="3f09f-134">String</span><span class="sxs-lookup"><span data-stu-id="3f09f-134">String</span></span>|<span data-ttu-id="3f09f-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f09f-135">Not yet documented</span></span>|
|<span data-ttu-id="3f09f-136">说明</span><span class="sxs-lookup"><span data-stu-id="3f09f-136">description</span></span>|<span data-ttu-id="3f09f-137">String</span><span class="sxs-lookup"><span data-stu-id="3f09f-137">String</span></span>|<span data-ttu-id="3f09f-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f09f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f09f-139">响应</span><span class="sxs-lookup"><span data-stu-id="3f09f-139">Response</span></span>
<span data-ttu-id="3f09f-140">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [deviceManagementConfigurationPolicy。](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3f09f-140">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f09f-141">示例</span><span class="sxs-lookup"><span data-stu-id="3f09f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f09f-142">请求</span><span class="sxs-lookup"><span data-stu-id="3f09f-142">Request</span></span>
<span data-ttu-id="3f09f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f09f-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy

Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="3f09f-144">响应</span><span class="sxs-lookup"><span data-stu-id="3f09f-144">Response</span></span>
<span data-ttu-id="3f09f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f09f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
    "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
    "name": "Name value",
    "description": "Description value",
    "platforms": "macOS",
    "technologies": "mdm",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "settingCount": 12,
    "creationSource": "Creation Source value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "isAssigned": true,
    "templateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
      "templateId": "Template Id value",
      "templateFamily": "endpointSecurityAntivirus",
      "templateDisplayName": "Template Display Name value",
      "templateDisplayVersion": "Template Display Version value"
    }
  }
}
```




