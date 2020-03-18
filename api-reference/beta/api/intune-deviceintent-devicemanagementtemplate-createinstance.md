---
title: createInstance 操作
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a0632f228ea6cab56cefed18878b14241a1cba54
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771136"
---
# <a name="createinstance-action"></a><span data-ttu-id="08885-103">createInstance 操作</span><span class="sxs-lookup"><span data-stu-id="08885-103">createInstance action</span></span>

> <span data-ttu-id="08885-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08885-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08885-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08885-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08885-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="08885-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08885-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="08885-107">Prerequisites</span></span>
<span data-ttu-id="08885-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08885-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="08885-110">Permission type</span></span>|<span data-ttu-id="08885-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08885-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08885-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08885-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08885-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08885-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08885-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08885-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08885-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08885-115">Not supported.</span></span>|
|<span data-ttu-id="08885-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="08885-116">Application</span></span>|<span data-ttu-id="08885-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08885-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08885-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08885-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="08885-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="08885-119">Request headers</span></span>
|<span data-ttu-id="08885-120">标头</span><span class="sxs-lookup"><span data-stu-id="08885-120">Header</span></span>|<span data-ttu-id="08885-121">值</span><span class="sxs-lookup"><span data-stu-id="08885-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08885-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08885-122">Authorization</span></span>|<span data-ttu-id="08885-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08885-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08885-124">接受</span><span class="sxs-lookup"><span data-stu-id="08885-124">Accept</span></span>|<span data-ttu-id="08885-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08885-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08885-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="08885-126">Request body</span></span>
<span data-ttu-id="08885-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08885-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="08885-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="08885-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="08885-129">属性</span><span class="sxs-lookup"><span data-stu-id="08885-129">Property</span></span>|<span data-ttu-id="08885-130">类型</span><span class="sxs-lookup"><span data-stu-id="08885-130">Type</span></span>|<span data-ttu-id="08885-131">说明</span><span class="sxs-lookup"><span data-stu-id="08885-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08885-132">displayName</span><span class="sxs-lookup"><span data-stu-id="08885-132">displayName</span></span>|<span data-ttu-id="08885-133">String</span><span class="sxs-lookup"><span data-stu-id="08885-133">String</span></span>|<span data-ttu-id="08885-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="08885-134">Not yet documented</span></span>|
|<span data-ttu-id="08885-135">说明</span><span class="sxs-lookup"><span data-stu-id="08885-135">description</span></span>|<span data-ttu-id="08885-136">String</span><span class="sxs-lookup"><span data-stu-id="08885-136">String</span></span>|<span data-ttu-id="08885-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="08885-137">Not yet documented</span></span>|
|<span data-ttu-id="08885-138">settingsDelta</span><span class="sxs-lookup"><span data-stu-id="08885-138">settingsDelta</span></span>|<span data-ttu-id="08885-139">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="08885-139">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="08885-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="08885-140">Not yet documented</span></span>|
|<span data-ttu-id="08885-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08885-141">roleScopeTagIds</span></span>|<span data-ttu-id="08885-142">String collection</span><span class="sxs-lookup"><span data-stu-id="08885-142">String collection</span></span>|<span data-ttu-id="08885-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="08885-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="08885-144">响应</span><span class="sxs-lookup"><span data-stu-id="08885-144">Response</span></span>
<span data-ttu-id="08885-145">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 。</span><span class="sxs-lookup"><span data-stu-id="08885-145">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08885-146">示例</span><span class="sxs-lookup"><span data-stu-id="08885-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="08885-147">请求</span><span class="sxs-lookup"><span data-stu-id="08885-147">Request</span></span>
<span data-ttu-id="08885-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08885-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 398

{
  "displayName": "Display Name value",
  "description": "Description value",
  "settingsDelta": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="08885-149">响应</span><span class="sxs-lookup"><span data-stu-id="08885-149">Response</span></span>
<span data-ttu-id="08885-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08885-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




