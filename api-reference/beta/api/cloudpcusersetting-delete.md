---
title: 删除 cloudPcUserSetting
description: 删除 cloudPcUserSetting 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6f434d4536eff7361311ad20d2bc17498b700af3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207832"
---
# <a name="delete-cloudpcusersetting"></a><span data-ttu-id="16b12-103">删除 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="16b12-103">Delete cloudPcUserSetting</span></span>

<span data-ttu-id="16b12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16b12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16b12-105">删除 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16b12-105">Delete a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="16b12-106">权限</span><span class="sxs-lookup"><span data-stu-id="16b12-106">Permissions</span></span>

<span data-ttu-id="16b12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b12-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="16b12-109">Permission type</span></span>|<span data-ttu-id="16b12-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16b12-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16b12-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16b12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16b12-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b12-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="16b12-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16b12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16b12-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="16b12-114">Not supported.</span></span>|
|<span data-ttu-id="16b12-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="16b12-115">Application</span></span>|<span data-ttu-id="16b12-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b12-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16b12-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16b12-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="16b12-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="16b12-118">Request headers</span></span>
|<span data-ttu-id="16b12-119">名称</span><span class="sxs-lookup"><span data-stu-id="16b12-119">Name</span></span>|<span data-ttu-id="16b12-120">说明</span><span class="sxs-lookup"><span data-stu-id="16b12-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16b12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b12-121">Authorization</span></span>|<span data-ttu-id="16b12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16b12-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16b12-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="16b12-124">Request body</span></span>
<span data-ttu-id="16b12-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16b12-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b12-126">响应</span><span class="sxs-lookup"><span data-stu-id="16b12-126">Response</span></span>

<span data-ttu-id="16b12-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="16b12-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="16b12-128">示例</span><span class="sxs-lookup"><span data-stu-id="16b12-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16b12-129">请求</span><span class="sxs-lookup"><span data-stu-id="16b12-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="16b12-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="16b12-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_cloudpcusersetting"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
```
# <a name="c"></a>[<span data-ttu-id="16b12-131">C#</span><span class="sxs-lookup"><span data-stu-id="16b12-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16b12-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16b12-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16b12-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16b12-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16b12-134">Java</span><span class="sxs-lookup"><span data-stu-id="16b12-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="16b12-135">响应</span><span class="sxs-lookup"><span data-stu-id="16b12-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
