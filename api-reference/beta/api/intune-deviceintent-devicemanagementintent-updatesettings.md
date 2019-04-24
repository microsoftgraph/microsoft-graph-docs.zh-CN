---
title: updateSettings 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a67166d560409738469192e3b5486a033978d32d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32508398"
---
# <a name="updatesettings-action"></a><span data-ttu-id="f93d2-103">updateSettings 操作</span><span class="sxs-lookup"><span data-stu-id="f93d2-103">updateSettings action</span></span>

> <span data-ttu-id="f93d2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f93d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f93d2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f93d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f93d2-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f93d2-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f93d2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f93d2-107">Prerequisites</span></span>
<span data-ttu-id="f93d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f93d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f93d2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f93d2-110">Permission type</span></span>|<span data-ttu-id="f93d2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f93d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f93d2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f93d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f93d2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f93d2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f93d2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f93d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f93d2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f93d2-115">Not supported.</span></span>|
|<span data-ttu-id="f93d2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f93d2-116">Application</span></span>|<span data-ttu-id="f93d2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f93d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f93d2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f93d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="f93d2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f93d2-119">Request headers</span></span>
|<span data-ttu-id="f93d2-120">标头</span><span class="sxs-lookup"><span data-stu-id="f93d2-120">Header</span></span>|<span data-ttu-id="f93d2-121">值</span><span class="sxs-lookup"><span data-stu-id="f93d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f93d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f93d2-122">Authorization</span></span>|<span data-ttu-id="f93d2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f93d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f93d2-124">接受</span><span class="sxs-lookup"><span data-stu-id="f93d2-124">Accept</span></span>|<span data-ttu-id="f93d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f93d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f93d2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f93d2-126">Request body</span></span>
<span data-ttu-id="f93d2-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f93d2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f93d2-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f93d2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f93d2-129">属性</span><span class="sxs-lookup"><span data-stu-id="f93d2-129">Property</span></span>|<span data-ttu-id="f93d2-130">类型</span><span class="sxs-lookup"><span data-stu-id="f93d2-130">Type</span></span>|<span data-ttu-id="f93d2-131">说明</span><span class="sxs-lookup"><span data-stu-id="f93d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f93d2-132">settings</span><span class="sxs-lookup"><span data-stu-id="f93d2-132">settings</span></span>|<span data-ttu-id="f93d2-133">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="f93d2-133">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="f93d2-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f93d2-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f93d2-135">响应</span><span class="sxs-lookup"><span data-stu-id="f93d2-135">Response</span></span>
<span data-ttu-id="f93d2-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f93d2-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f93d2-137">示例</span><span class="sxs-lookup"><span data-stu-id="f93d2-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f93d2-138">请求</span><span class="sxs-lookup"><span data-stu-id="f93d2-138">Request</span></span>
<span data-ttu-id="f93d2-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f93d2-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/updateSettings

Content-type: application/json
Content-length: 252

{
  "settings": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f93d2-140">响应</span><span class="sxs-lookup"><span data-stu-id="f93d2-140">Response</span></span>
<span data-ttu-id="f93d2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f93d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





