---
title: 删除 raProfileDatabaseEntity
description: 删除 raProfileDatabaseEntity。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 822f2e39642425e4de153757c0c3545dbcb10ebf
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124245"
---
# <a name="delete-raprofiledatabaseentity"></a><span data-ttu-id="85422-103">删除 raProfileDatabaseEntity</span><span class="sxs-lookup"><span data-stu-id="85422-103">Delete raProfileDatabaseEntity</span></span>

<span data-ttu-id="85422-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85422-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85422-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85422-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85422-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85422-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85422-107">删除[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)。</span><span class="sxs-lookup"><span data-stu-id="85422-107">Deletes a [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85422-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85422-108">Prerequisites</span></span>
<span data-ttu-id="85422-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85422-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85422-111">Permission type</span></span>|<span data-ttu-id="85422-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85422-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85422-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85422-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85422-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85422-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85422-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85422-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85422-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85422-116">Not supported.</span></span>|
|<span data-ttu-id="85422-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="85422-117">Application</span></span>|<span data-ttu-id="85422-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85422-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85422-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85422-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

## <a name="request-headers"></a><span data-ttu-id="85422-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="85422-120">Request headers</span></span>
|<span data-ttu-id="85422-121">标头</span><span class="sxs-lookup"><span data-stu-id="85422-121">Header</span></span>|<span data-ttu-id="85422-122">值</span><span class="sxs-lookup"><span data-stu-id="85422-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85422-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85422-123">Authorization</span></span>|<span data-ttu-id="85422-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85422-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85422-125">接受</span><span class="sxs-lookup"><span data-stu-id="85422-125">Accept</span></span>|<span data-ttu-id="85422-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85422-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85422-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85422-127">Request body</span></span>
<span data-ttu-id="85422-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="85422-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85422-129">响应</span><span class="sxs-lookup"><span data-stu-id="85422-129">Response</span></span>
<span data-ttu-id="85422-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85422-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85422-131">示例</span><span class="sxs-lookup"><span data-stu-id="85422-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="85422-132">请求</span><span class="sxs-lookup"><span data-stu-id="85422-132">Request</span></span>
<span data-ttu-id="85422-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85422-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

### <a name="response"></a><span data-ttu-id="85422-134">响应</span><span class="sxs-lookup"><span data-stu-id="85422-134">Response</span></span>
<span data-ttu-id="85422-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85422-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



