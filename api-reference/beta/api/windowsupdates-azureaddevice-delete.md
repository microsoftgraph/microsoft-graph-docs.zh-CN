---
title: 删除 azureADDevice
description: 删除 azureADDevice 对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 82e457f433ab3e307eaf727dc09d18144f3dd844
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241445"
---
# <a name="delete-azureaddevice"></a><span data-ttu-id="f25a9-103">删除 azureADDevice</span><span class="sxs-lookup"><span data-stu-id="f25a9-103">Delete azureADDevice</span></span>
<span data-ttu-id="f25a9-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f25a9-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f25a9-105">删除 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f25a9-105">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

<span data-ttu-id="f25a9-106">删除 Azure AD 设备后，它将从部署服务注销，并自动注销该服务管理的所有更新类别，以及从每个 [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) 和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)中删除。</span><span class="sxs-lookup"><span data-stu-id="f25a9-106">When an Azure AD device is deleted, it is unregistered from the deployment service and automatically unenrolled from management by the service for all update categories, as well as removed from every [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f25a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="f25a9-107">Permissions</span></span>
<span data-ttu-id="f25a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f25a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f25a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f25a9-110">Permission type</span></span>|<span data-ttu-id="f25a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f25a9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f25a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f25a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f25a9-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25a9-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="f25a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f25a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f25a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f25a9-115">Not supported.</span></span>|
|<span data-ttu-id="f25a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f25a9-116">Application</span></span>|<span data-ttu-id="f25a9-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25a9-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f25a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f25a9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="f25a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f25a9-119">Request headers</span></span>
|<span data-ttu-id="f25a9-120">名称</span><span class="sxs-lookup"><span data-stu-id="f25a9-120">Name</span></span>|<span data-ttu-id="f25a9-121">说明</span><span class="sxs-lookup"><span data-stu-id="f25a9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f25a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f25a9-122">Authorization</span></span>|<span data-ttu-id="f25a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f25a9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f25a9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f25a9-125">Request body</span></span>
<span data-ttu-id="f25a9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f25a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f25a9-127">响应</span><span class="sxs-lookup"><span data-stu-id="f25a9-127">Response</span></span>

<span data-ttu-id="f25a9-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f25a9-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f25a9-130">示例</span><span class="sxs-lookup"><span data-stu-id="f25a9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f25a9-131">请求</span><span class="sxs-lookup"><span data-stu-id="f25a9-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f25a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f25a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_azureaddevice"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```
# <a name="c"></a>[<span data-ttu-id="f25a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="f25a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-azureaddevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f25a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f25a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-azureaddevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f25a9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f25a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-azureaddevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f25a9-136">Java</span><span class="sxs-lookup"><span data-stu-id="f25a9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-azureaddevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f25a9-137">响应</span><span class="sxs-lookup"><span data-stu-id="f25a9-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

