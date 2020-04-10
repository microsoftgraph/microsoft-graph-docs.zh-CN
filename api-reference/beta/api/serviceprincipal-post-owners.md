---
title: servicePrincipal：添加所有者
description: 使用此 API 添加服务主体的所有者。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: fa760a3a88377782abbb797fe4ce2496ca4b7a6a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218617"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="2d97c-103">servicePrincipal：添加所有者</span><span class="sxs-lookup"><span data-stu-id="2d97c-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="2d97c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d97c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d97c-105">使用此 API 添加服务主体的所有者。</span><span class="sxs-lookup"><span data-stu-id="2d97c-105">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d97c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2d97c-106">Permissions</span></span>
<span data-ttu-id="2d97c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d97c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d97c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d97c-109">Permission type</span></span>      | <span data-ttu-id="2d97c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d97c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d97c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d97c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d97c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d97c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d97c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d97c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d97c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d97c-114">Not supported.</span></span>    |
|<span data-ttu-id="2d97c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d97c-115">Application</span></span> | <span data-ttu-id="2d97c-116">Application.readwrite.ownedby 和 "全部读取"。全部、全部读取全部和全部读取全部。</span><span class="sxs-lookup"><span data-stu-id="2d97c-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d97c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d97c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="2d97c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d97c-118">Request headers</span></span>
| <span data-ttu-id="2d97c-119">名称</span><span class="sxs-lookup"><span data-stu-id="2d97c-119">Name</span></span>       | <span data-ttu-id="2d97c-120">类型</span><span class="sxs-lookup"><span data-stu-id="2d97c-120">Type</span></span> | <span data-ttu-id="2d97c-121">说明</span><span class="sxs-lookup"><span data-stu-id="2d97c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d97c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d97c-122">Authorization</span></span>  | <span data-ttu-id="2d97c-123">string</span><span class="sxs-lookup"><span data-stu-id="2d97c-123">string</span></span>  | <span data-ttu-id="2d97c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d97c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d97c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d97c-126">Request body</span></span>
<span data-ttu-id="2d97c-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d97c-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2d97c-128">响应</span><span class="sxs-lookup"><span data-stu-id="2d97c-128">Response</span></span>

<span data-ttu-id="2d97c-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d97c-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d97c-130">示例</span><span class="sxs-lookup"><span data-stu-id="2d97c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d97c-131">请求</span><span class="sxs-lookup"><span data-stu-id="2d97c-131">Request</span></span>
<span data-ttu-id="2d97c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d97c-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d97c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d97c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="2d97c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d97c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2d97c-135">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d97c-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2d97c-136">响应</span><span class="sxs-lookup"><span data-stu-id="2d97c-136">Response</span></span>
<span data-ttu-id="2d97c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d97c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
