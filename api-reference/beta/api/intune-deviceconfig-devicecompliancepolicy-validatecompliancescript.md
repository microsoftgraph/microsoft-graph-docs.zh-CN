---
title: validateComplianceScript 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16d7b5ad18a1ba9389d4c68bb88d5f88335efc2c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793050"
---
# <a name="validatecompliancescript-action"></a><span data-ttu-id="1646c-103">validateComplianceScript 操作</span><span class="sxs-lookup"><span data-stu-id="1646c-103">validateComplianceScript action</span></span>

<span data-ttu-id="1646c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1646c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1646c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1646c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1646c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1646c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1646c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1646c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1646c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1646c-108">Prerequisites</span></span>
<span data-ttu-id="1646c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1646c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1646c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1646c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1646c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1646c-111">Permission type</span></span>|<span data-ttu-id="1646c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1646c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1646c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1646c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1646c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1646c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1646c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1646c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1646c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1646c-116">Not supported.</span></span>|
|<span data-ttu-id="1646c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1646c-117">Application</span></span>|<span data-ttu-id="1646c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1646c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1646c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1646c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/validateComplianceScript
```

## <a name="request-headers"></a><span data-ttu-id="1646c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1646c-120">Request headers</span></span>
|<span data-ttu-id="1646c-121">标头</span><span class="sxs-lookup"><span data-stu-id="1646c-121">Header</span></span>|<span data-ttu-id="1646c-122">值</span><span class="sxs-lookup"><span data-stu-id="1646c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1646c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1646c-123">Authorization</span></span>|<span data-ttu-id="1646c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1646c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1646c-125">接受</span><span class="sxs-lookup"><span data-stu-id="1646c-125">Accept</span></span>|<span data-ttu-id="1646c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1646c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1646c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1646c-127">Request body</span></span>
<span data-ttu-id="1646c-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1646c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1646c-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1646c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1646c-130">属性</span><span class="sxs-lookup"><span data-stu-id="1646c-130">Property</span></span>|<span data-ttu-id="1646c-131">类型</span><span class="sxs-lookup"><span data-stu-id="1646c-131">Type</span></span>|<span data-ttu-id="1646c-132">说明</span><span class="sxs-lookup"><span data-stu-id="1646c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1646c-133">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="1646c-133">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="1646c-134">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="1646c-134">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="1646c-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1646c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1646c-136">响应</span><span class="sxs-lookup"><span data-stu-id="1646c-136">Response</span></span>
<span data-ttu-id="1646c-137">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和[deviceComplianceScriptValidationResult](../resources/intune-deviceconfig-devicecompliancescriptvalidationresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="1646c-137">If successful, this action returns a `200 OK` response code and a [deviceComplianceScriptValidationResult](../resources/intune-deviceconfig-devicecompliancescriptvalidationresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1646c-138">示例</span><span class="sxs-lookup"><span data-stu-id="1646c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1646c-139">请求</span><span class="sxs-lookup"><span data-stu-id="1646c-139">Request</span></span>
<span data-ttu-id="1646c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1646c-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/validateComplianceScript

Content-type: application/json
Content-length: 224

{
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```

### <a name="response"></a><span data-ttu-id="1646c-141">响应</span><span class="sxs-lookup"><span data-stu-id="1646c-141">Response</span></span>
<span data-ttu-id="1646c-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1646c-142">Here is an example of the response.</span></span> <span data-ttu-id="1646c-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1646c-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1646c-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1646c-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": {
    "@odata.type": "microsoft.graph.deviceComplianceScriptValidationResult",
    "rules": [
      {
        "@odata.type": "microsoft.graph.deviceComplianceScriptRule",
        "settingName": "Setting Name value",
        "operator": "and",
        "dataType": "boolean",
        "operand": "Operand value"
      }
    ],
    "scriptErrors": [
      {
        "@odata.type": "microsoft.graph.deviceComplianceScriptError",
        "code": "jsonFileInvalid",
        "message": "Message value"
      }
    ],
    "ruleErrors": [
      {
        "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
        "code": "jsonFileInvalid",
        "message": "Message value",
        "settingName": "Setting Name value"
      }
    ]
  }
}
```



