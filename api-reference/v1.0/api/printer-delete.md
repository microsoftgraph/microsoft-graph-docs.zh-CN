---
title: 删除打印机
description: 删除 (注销) 打印机。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 94841d1668363ffeb98d8416527c06d53bb7c517
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776926"
---
# <a name="delete-printer"></a><span data-ttu-id="20072-103">删除打印机</span><span class="sxs-lookup"><span data-stu-id="20072-103">Delete printer</span></span>
<span data-ttu-id="20072-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20072-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="20072-105">删除 (注销) 打印机[。](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="20072-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="20072-106">权限</span><span class="sxs-lookup"><span data-stu-id="20072-106">Permissions</span></span>
<span data-ttu-id="20072-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="20072-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="20072-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="20072-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="20072-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="20072-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="20072-111">Permission type</span></span> | <span data-ttu-id="20072-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20072-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="20072-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20072-113">Delegated (work or school account)</span></span>| <span data-ttu-id="20072-114">Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="20072-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="20072-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20072-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20072-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20072-116">Not Supported.</span></span>|
|<span data-ttu-id="20072-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="20072-117">Application</span></span>|<span data-ttu-id="20072-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="20072-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20072-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20072-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="20072-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="20072-120">Request headers</span></span>
|<span data-ttu-id="20072-121">名称</span><span class="sxs-lookup"><span data-stu-id="20072-121">Name</span></span>|<span data-ttu-id="20072-122">说明</span><span class="sxs-lookup"><span data-stu-id="20072-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20072-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20072-123">Authorization</span></span>|<span data-ttu-id="20072-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20072-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20072-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="20072-126">Request body</span></span>
<span data-ttu-id="20072-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20072-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20072-128">响应</span><span class="sxs-lookup"><span data-stu-id="20072-128">Response</span></span>

<span data-ttu-id="20072-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="20072-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="20072-130">示例</span><span class="sxs-lookup"><span data-stu-id="20072-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20072-131">请求</span><span class="sxs-lookup"><span data-stu-id="20072-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20072-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="20072-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}
```
# <a name="c"></a>[<span data-ttu-id="20072-133">C#</span><span class="sxs-lookup"><span data-stu-id="20072-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20072-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20072-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20072-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20072-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20072-136">Java</span><span class="sxs-lookup"><span data-stu-id="20072-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="20072-137">响应</span><span class="sxs-lookup"><span data-stu-id="20072-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

