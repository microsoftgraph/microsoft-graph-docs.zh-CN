---
title: 删除 printerShare
description: 删除打印机共享 (取消共享关联的打印机) 。 此操作无法撤消。 如果以后再次共享打印机，则之前安装了该打印机的任何 Windows 用户都需要发现并重新安装它。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 95a907f18693165304894fab41da36e28b551f35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771664"
---
# <a name="delete-printershare"></a><span data-ttu-id="9c4f0-105">删除 printerShare</span><span class="sxs-lookup"><span data-stu-id="9c4f0-105">Delete printerShare</span></span>
<span data-ttu-id="9c4f0-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c4f0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="9c4f0-107">删除打印机共享 (取消共享关联的[打印机) 。](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="9c4f0-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="9c4f0-108">此操作无法撤消。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-108">This action cannot be undone.</span></span> <span data-ttu-id="9c4f0-109">如果[以后](../resources/printer.md)再次共享打印机，则之前安装了打印机的任何 Windows 用户都需要发现并[](../resources/printer.md)重新安装打印机。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c4f0-110">权限</span><span class="sxs-lookup"><span data-stu-id="9c4f0-110">Permissions</span></span>
<span data-ttu-id="9c4f0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9c4f0-113">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-113">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="9c4f0-114">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-114">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="9c4f0-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c4f0-115">Permission type</span></span> | <span data-ttu-id="9c4f0-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c4f0-116">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9c4f0-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c4f0-117">Delegated (work or school account)</span></span>| <span data-ttu-id="9c4f0-118">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c4f0-118">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="9c4f0-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c4f0-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c4f0-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-120">Not Supported.</span></span>|
|<span data-ttu-id="9c4f0-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c4f0-121">Application</span></span>|<span data-ttu-id="9c4f0-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-122">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c4f0-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c4f0-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/shares/{printerShareId}
```

## <a name="request-headers"></a><span data-ttu-id="9c4f0-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c4f0-124">Request headers</span></span>
|<span data-ttu-id="9c4f0-125">名称</span><span class="sxs-lookup"><span data-stu-id="9c4f0-125">Name</span></span>|<span data-ttu-id="9c4f0-126">说明</span><span class="sxs-lookup"><span data-stu-id="9c4f0-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9c4f0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c4f0-127">Authorization</span></span>|<span data-ttu-id="9c4f0-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c4f0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c4f0-130">Request body</span></span>
<span data-ttu-id="9c4f0-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c4f0-132">响应</span><span class="sxs-lookup"><span data-stu-id="9c4f0-132">Response</span></span>

<span data-ttu-id="9c4f0-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9c4f0-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c4f0-135">示例</span><span class="sxs-lookup"><span data-stu-id="9c4f0-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c4f0-136">请求</span><span class="sxs-lookup"><span data-stu-id="9c4f0-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9c4f0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c4f0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```
# <a name="c"></a>[<span data-ttu-id="9c4f0-138">C#</span><span class="sxs-lookup"><span data-stu-id="9c4f0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c4f0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c4f0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c4f0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c4f0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c4f0-141">Java</span><span class="sxs-lookup"><span data-stu-id="9c4f0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9c4f0-142">响应</span><span class="sxs-lookup"><span data-stu-id="9c4f0-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

