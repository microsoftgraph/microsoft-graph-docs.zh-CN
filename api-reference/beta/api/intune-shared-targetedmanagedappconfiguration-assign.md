---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81797d545203f758faeb09d8eb72b5268190e1a0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863021"
---
# <a name="assign-action"></a><span data-ttu-id="b4f72-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="b4f72-103">assign action</span></span>

<span data-ttu-id="b4f72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4f72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4f72-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4f72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4f72-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4f72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4f72-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b4f72-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4f72-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4f72-108">Prerequisites</span></span>
<span data-ttu-id="b4f72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4f72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4f72-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4f72-111">Permission type</span></span>|<span data-ttu-id="b4f72-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b4f72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4f72-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4f72-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b4f72-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b4f72-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b4f72-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f72-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4f72-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4f72-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4f72-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4f72-117">Not supported.</span></span>|
|<span data-ttu-id="b4f72-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4f72-118">Application</span></span>||
| <span data-ttu-id="b4f72-119">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b4f72-119">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b4f72-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f72-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4f72-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4f72-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b4f72-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4f72-122">Request headers</span></span>
|<span data-ttu-id="b4f72-123">标头</span><span class="sxs-lookup"><span data-stu-id="b4f72-123">Header</span></span>|<span data-ttu-id="b4f72-124">值</span><span class="sxs-lookup"><span data-stu-id="b4f72-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4f72-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4f72-125">Authorization</span></span>|<span data-ttu-id="b4f72-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4f72-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4f72-127">接受</span><span class="sxs-lookup"><span data-stu-id="b4f72-127">Accept</span></span>|<span data-ttu-id="b4f72-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b4f72-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4f72-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4f72-129">Request body</span></span>
<span data-ttu-id="b4f72-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4f72-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b4f72-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b4f72-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b4f72-132">属性</span><span class="sxs-lookup"><span data-stu-id="b4f72-132">Property</span></span>|<span data-ttu-id="b4f72-133">类型</span><span class="sxs-lookup"><span data-stu-id="b4f72-133">Type</span></span>|<span data-ttu-id="b4f72-134">说明</span><span class="sxs-lookup"><span data-stu-id="b4f72-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4f72-135">assignments</span><span class="sxs-lookup"><span data-stu-id="b4f72-135">assignments</span></span>|<span data-ttu-id="b4f72-136">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4f72-136">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="b4f72-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b4f72-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b4f72-138">响应</span><span class="sxs-lookup"><span data-stu-id="b4f72-138">Response</span></span>
<span data-ttu-id="b4f72-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b4f72-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4f72-140">示例</span><span class="sxs-lookup"><span data-stu-id="b4f72-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4f72-141">请求</span><span class="sxs-lookup"><span data-stu-id="b4f72-141">Request</span></span>
<span data-ttu-id="b4f72-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4f72-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

Content-type: application/json
Content-length: 351

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b4f72-143">响应</span><span class="sxs-lookup"><span data-stu-id="b4f72-143">Response</span></span>
<span data-ttu-id="b4f72-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4f72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







