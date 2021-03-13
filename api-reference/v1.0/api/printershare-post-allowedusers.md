---
title: 为 printerShare 创建 allowedUser
description: 向指定的用户授予将打印作业提交到关联的打印机共享的权限。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9a3d198c225633ebeecf7de8d5c069e49c014eeb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771426"
---
# <a name="create-alloweduser-for-printershare"></a><span data-ttu-id="02adb-103">为 printerShare 创建 allowedUser</span><span class="sxs-lookup"><span data-stu-id="02adb-103">Create allowedUser for printerShare</span></span>
<span data-ttu-id="02adb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02adb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="02adb-105">授予指定用户向关联的 printerShare 提交打印 [作业的权限](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="02adb-105">Grant the specified user access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="02adb-106">权限</span><span class="sxs-lookup"><span data-stu-id="02adb-106">Permissions</span></span>
<span data-ttu-id="02adb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02adb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="02adb-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="02adb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="02adb-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="02adb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="02adb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02adb-111">Permission type</span></span> | <span data-ttu-id="02adb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02adb-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="02adb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02adb-113">Delegated (work or school account)</span></span>| <span data-ttu-id="02adb-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02adb-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="02adb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02adb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02adb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="02adb-116">Not Supported.</span></span>|
|<span data-ttu-id="02adb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="02adb-117">Application</span></span>|<span data-ttu-id="02adb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="02adb-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02adb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02adb-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/allowedUsers/$ref
```

## <a name="request-headers"></a><span data-ttu-id="02adb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="02adb-120">Request headers</span></span>
|<span data-ttu-id="02adb-121">名称</span><span class="sxs-lookup"><span data-stu-id="02adb-121">Name</span></span>|<span data-ttu-id="02adb-122">说明</span><span class="sxs-lookup"><span data-stu-id="02adb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02adb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02adb-123">Authorization</span></span>|<span data-ttu-id="02adb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02adb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="02adb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02adb-126">Content-Type</span></span>|<span data-ttu-id="02adb-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="02adb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02adb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="02adb-129">Request body</span></span>
<span data-ttu-id="02adb-130">在请求正文中，使用 格式提供对用户实体的引用， `@odata.id` 如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="02adb-130">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="02adb-131">响应</span><span class="sxs-lookup"><span data-stu-id="02adb-131">Response</span></span>

<span data-ttu-id="02adb-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="02adb-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="02adb-133">示例</span><span class="sxs-lookup"><span data-stu-id="02adb-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02adb-134">请求</span><span class="sxs-lookup"><span data-stu-id="02adb-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02adb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="02adb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers/$ref
Content-Type: application/json
Content-length: 46

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{userId}"
}
```
# <a name="c"></a>[<span data-ttu-id="02adb-136">C#</span><span class="sxs-lookup"><span data-stu-id="02adb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02adb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02adb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02adb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02adb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02adb-139">Java</span><span class="sxs-lookup"><span data-stu-id="02adb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="02adb-140">响应</span><span class="sxs-lookup"><span data-stu-id="02adb-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
}
-->
```http
HTTP/1.1 204 No Content
```

