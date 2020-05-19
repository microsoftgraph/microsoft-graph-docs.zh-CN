---
title: servicePrincipal：添加所有者
description: 添加服务主体的所有者。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 31851eb6e4e653d1c97ba56fda8c7a80e6e5803f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290010"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="f2aeb-103">servicePrincipal：添加所有者</span><span class="sxs-lookup"><span data-stu-id="f2aeb-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="f2aeb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2aeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2aeb-105">为[servicePrincipal](../resources/serviceprincipal.md)添加所有者。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2aeb-106">权限</span><span class="sxs-lookup"><span data-stu-id="f2aeb-106">Permissions</span></span>
<span data-ttu-id="f2aeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2aeb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2aeb-109">Permission type</span></span>      | <span data-ttu-id="f2aeb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2aeb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2aeb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2aeb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2aeb-112">"ReadWrite"、"全部" 和 "Directory.accessasuser.all"、"全部" 和 "所有"。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2aeb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2aeb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2aeb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-114">Not supported.</span></span>    |
|<span data-ttu-id="f2aeb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2aeb-115">Application</span></span> | <span data-ttu-id="f2aeb-116">Application.readwrite.ownedby 和 Application.readwrite.ownedby 和所有和所有的读写全部，all 和所有读写全部。 all 和所有读写全部。 all 和所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f2aeb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2aeb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="f2aeb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2aeb-118">Request headers</span></span>
| <span data-ttu-id="f2aeb-119">名称</span><span class="sxs-lookup"><span data-stu-id="f2aeb-119">Name</span></span>       | <span data-ttu-id="f2aeb-120">说明</span><span class="sxs-lookup"><span data-stu-id="f2aeb-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="f2aeb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2aeb-121">Authorization</span></span> | <span data-ttu-id="f2aeb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2aeb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2aeb-124">Request body</span></span>
<span data-ttu-id="f2aeb-125">在请求正文中，提供[directoryObject](../resources/directoryobject.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f2aeb-126">响应</span><span class="sxs-lookup"><span data-stu-id="f2aeb-126">Response</span></span>

<span data-ttu-id="f2aeb-127">如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2aeb-128">示例</span><span class="sxs-lookup"><span data-stu-id="f2aeb-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f2aeb-129">请求</span><span class="sxs-lookup"><span data-stu-id="f2aeb-129">Request</span></span>
<span data-ttu-id="f2aeb-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-130">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

<span data-ttu-id="f2aeb-131">在请求正文中，提供[directoryObject](../resources/directoryobject.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-131">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="f2aeb-132">响应</span><span class="sxs-lookup"><span data-stu-id="f2aeb-132">Response</span></span>
<span data-ttu-id="f2aeb-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f2aeb-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
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
