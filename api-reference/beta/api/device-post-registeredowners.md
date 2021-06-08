---
title: 创建 registeredOwner
description: 将用户添加为设备的已注册所有者。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 65d49c3dc9f547ea9b1b88889bea44cde63d02be
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786031"
---
# <a name="create-registeredowner"></a><span data-ttu-id="8800b-103">创建 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="8800b-103">Create registeredOwner</span></span>

<span data-ttu-id="8800b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8800b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8800b-105">将用户添加为设备的已注册所有者。</span><span class="sxs-lookup"><span data-stu-id="8800b-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="8800b-106">权限</span><span class="sxs-lookup"><span data-stu-id="8800b-106">Permissions</span></span>
<span data-ttu-id="8800b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8800b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8800b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8800b-109">Permission type</span></span>      | <span data-ttu-id="8800b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8800b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8800b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8800b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8800b-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8800b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8800b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8800b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8800b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8800b-114">Not supported.</span></span>    |
|<span data-ttu-id="8800b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8800b-115">Application</span></span> | <span data-ttu-id="8800b-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8800b-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8800b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8800b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="8800b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8800b-118">Request headers</span></span>
| <span data-ttu-id="8800b-119">名称</span><span class="sxs-lookup"><span data-stu-id="8800b-119">Name</span></span>       | <span data-ttu-id="8800b-120">类型</span><span class="sxs-lookup"><span data-stu-id="8800b-120">Type</span></span> | <span data-ttu-id="8800b-121">说明</span><span class="sxs-lookup"><span data-stu-id="8800b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8800b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8800b-122">Authorization</span></span>  | <span data-ttu-id="8800b-123">string</span><span class="sxs-lookup"><span data-stu-id="8800b-123">string</span></span>  | <span data-ttu-id="8800b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8800b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8800b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8800b-126">Request body</span></span>
<span data-ttu-id="8800b-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8800b-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8800b-128">响应</span><span class="sxs-lookup"><span data-stu-id="8800b-128">Response</span></span>

<span data-ttu-id="8800b-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8800b-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8800b-130">示例</span><span class="sxs-lookup"><span data-stu-id="8800b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8800b-131">请求</span><span class="sxs-lookup"><span data-stu-id="8800b-131">Request</span></span>
<span data-ttu-id="8800b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8800b-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8800b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8800b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device_1"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="8800b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8800b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8800b-135">C#</span><span class="sxs-lookup"><span data-stu-id="8800b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8800b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8800b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8800b-137">Java</span><span class="sxs-lookup"><span data-stu-id="8800b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-device-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8800b-138">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8800b-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8800b-139">响应</span><span class="sxs-lookup"><span data-stu-id="8800b-139">Response</span></span>
<span data-ttu-id="8800b-p103">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8800b-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


