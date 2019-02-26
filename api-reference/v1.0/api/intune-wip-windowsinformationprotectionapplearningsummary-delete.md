---
title: 删除 windowsInformationProtectionAppLearningSummary
description: 删除 windowsInformationProtectionAppLearningSummary。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c6b0f877aac23c026920a347ba0051a9f7faf4b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261318"
---
# <a name="delete-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="549aa-103">删除 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="549aa-103">Delete windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="549aa-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="549aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="549aa-105">删除 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="549aa-105">Deletes a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="549aa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="549aa-106">Prerequisites</span></span>
<span data-ttu-id="549aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="549aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="549aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="549aa-109">Permission type</span></span>|<span data-ttu-id="549aa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="549aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="549aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="549aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="549aa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="549aa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="549aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="549aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="549aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="549aa-114">Not supported.</span></span>|
|<span data-ttu-id="549aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="549aa-115">Application</span></span>|<span data-ttu-id="549aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="549aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="549aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="549aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="549aa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="549aa-118">Request headers</span></span>
|<span data-ttu-id="549aa-119">标头</span><span class="sxs-lookup"><span data-stu-id="549aa-119">Header</span></span>|<span data-ttu-id="549aa-120">值</span><span class="sxs-lookup"><span data-stu-id="549aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="549aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="549aa-121">Authorization</span></span>|<span data-ttu-id="549aa-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="549aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="549aa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="549aa-123">Accept</span></span>|<span data-ttu-id="549aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="549aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="549aa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="549aa-125">Request body</span></span>
<span data-ttu-id="549aa-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="549aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="549aa-127">响应</span><span class="sxs-lookup"><span data-stu-id="549aa-127">Response</span></span>
<span data-ttu-id="549aa-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="549aa-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="549aa-129">示例</span><span class="sxs-lookup"><span data-stu-id="549aa-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="549aa-130">请求</span><span class="sxs-lookup"><span data-stu-id="549aa-130">Request</span></span>
<span data-ttu-id="549aa-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="549aa-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="549aa-132">响应</span><span class="sxs-lookup"><span data-stu-id="549aa-132">Response</span></span>
<span data-ttu-id="549aa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="549aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



