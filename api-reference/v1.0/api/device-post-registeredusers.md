---
title: 创建 registeredUser
description: 添加设备的已注册用户。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 29a2314eb53d1ff1e79ef2375d8f887434809a6e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053214"
---
# <a name="create-registereduser"></a><span data-ttu-id="7b4cc-103">创建 registeredUser</span><span class="sxs-lookup"><span data-stu-id="7b4cc-103">Create registeredUser</span></span>

<span data-ttu-id="7b4cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b4cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b4cc-105">添加设备的已注册用户。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b4cc-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b4cc-106">Permissions</span></span>
<span data-ttu-id="7b4cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7b4cc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b4cc-109">Permission type</span></span>      | <span data-ttu-id="7b4cc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b4cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b4cc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b4cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b4cc-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b4cc-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b4cc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b4cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b4cc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-114">Not supported.</span></span>    |
|<span data-ttu-id="7b4cc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b4cc-115">Application</span></span> | <span data-ttu-id="7b4cc-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b4cc-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b4cc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b4cc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7b4cc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b4cc-118">Request headers</span></span>
| <span data-ttu-id="7b4cc-119">名称</span><span class="sxs-lookup"><span data-stu-id="7b4cc-119">Name</span></span>       | <span data-ttu-id="7b4cc-120">类型</span><span class="sxs-lookup"><span data-stu-id="7b4cc-120">Type</span></span> | <span data-ttu-id="7b4cc-121">说明</span><span class="sxs-lookup"><span data-stu-id="7b4cc-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b4cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b4cc-122">Authorization</span></span>  | <span data-ttu-id="7b4cc-123">string</span><span class="sxs-lookup"><span data-stu-id="7b4cc-123">string</span></span>  | <span data-ttu-id="7b4cc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b4cc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b4cc-126">Request body</span></span>
<span data-ttu-id="7b4cc-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7b4cc-128">响应</span><span class="sxs-lookup"><span data-stu-id="7b4cc-128">Response</span></span>

<span data-ttu-id="7b4cc-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7b4cc-130">示例</span><span class="sxs-lookup"><span data-stu-id="7b4cc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b4cc-131">请求</span><span class="sxs-lookup"><span data-stu-id="7b4cc-131">Request</span></span>
<span data-ttu-id="7b4cc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b4cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b4cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7b4cc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b4cc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7b4cc-135">C#</span><span class="sxs-lookup"><span data-stu-id="7b4cc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b4cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b4cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b4cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="7b4cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-device-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7b4cc-138">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7b4cc-139">响应</span><span class="sxs-lookup"><span data-stu-id="7b4cc-139">Response</span></span>
<span data-ttu-id="7b4cc-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-140">Here is an example of the response.</span></span> <span data-ttu-id="7b4cc-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b4cc-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

