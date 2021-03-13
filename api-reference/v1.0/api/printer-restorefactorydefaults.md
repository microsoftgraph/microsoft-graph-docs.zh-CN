---
title: printer： restoreFactoryDefaults
description: 重置打印机的默认设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 68bf2f96336e6156a28cab9d42e9e5ee5971a659
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771790"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="d1c8f-103">printer： restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="d1c8f-103">printer: restoreFactoryDefaults</span></span>
<span data-ttu-id="d1c8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1c8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d1c8f-105">将 [打印机](../resources/printer.md)的默认设置还原到制造商指定的值。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1c8f-106">权限</span><span class="sxs-lookup"><span data-stu-id="d1c8f-106">Permissions</span></span>
<span data-ttu-id="d1c8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d1c8f-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="d1c8f-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="d1c8f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1c8f-111">Permission type</span></span> | <span data-ttu-id="d1c8f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1c8f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d1c8f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1c8f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d1c8f-114">Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d1c8f-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="d1c8f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1c8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1c8f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-116">Not Supported.</span></span>|
|<span data-ttu-id="d1c8f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1c8f-117">Application</span></span>| <span data-ttu-id="d1c8f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1c8f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1c8f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/restoreFactoryDefaults
```

## <a name="request-headers"></a><span data-ttu-id="d1c8f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1c8f-120">Request headers</span></span>
|<span data-ttu-id="d1c8f-121">名称</span><span class="sxs-lookup"><span data-stu-id="d1c8f-121">Name</span></span>|<span data-ttu-id="d1c8f-122">说明</span><span class="sxs-lookup"><span data-stu-id="d1c8f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d1c8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1c8f-123">Authorization</span></span>|<span data-ttu-id="d1c8f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c8f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1c8f-126">Request body</span></span>
<span data-ttu-id="d1c8f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1c8f-128">响应</span><span class="sxs-lookup"><span data-stu-id="d1c8f-128">Response</span></span>

<span data-ttu-id="d1c8f-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d1c8f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1c8f-131">示例</span><span class="sxs-lookup"><span data-stu-id="d1c8f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1c8f-132">请求</span><span class="sxs-lookup"><span data-stu-id="d1c8f-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d1c8f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1c8f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer_restorefactorydefaults"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/restoreFactoryDefaults
```
# <a name="c"></a>[<span data-ttu-id="d1c8f-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1c8f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-restorefactorydefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1c8f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1c8f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-restorefactorydefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1c8f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1c8f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-restorefactorydefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1c8f-137">Java</span><span class="sxs-lookup"><span data-stu-id="d1c8f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-restorefactorydefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d1c8f-138">响应</span><span class="sxs-lookup"><span data-stu-id="d1c8f-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

