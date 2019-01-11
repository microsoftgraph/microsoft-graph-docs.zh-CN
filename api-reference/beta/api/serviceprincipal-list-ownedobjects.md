---
title: servicePrincipals： 列表 ownedObjects
description: 检索拥有的 servicePrincipal 对象的列表。  这可能包括应用程序或组。
localization_priority: Normal
ms.openlocfilehash: f061a99c6389651985779ac71df2ced5a91ba527
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882864"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="c6b58-104">servicePrincipals： 列表 ownedObjects</span><span class="sxs-lookup"><span data-stu-id="c6b58-104">servicePrincipals: List ownedObjects</span></span>

> <span data-ttu-id="c6b58-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6b58-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6b58-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6b58-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6b58-107">检索拥有的 servicePrincipal 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c6b58-107">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="c6b58-108">这可能包括应用程序或组。</span><span class="sxs-lookup"><span data-stu-id="c6b58-108">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6b58-109">权限</span><span class="sxs-lookup"><span data-stu-id="c6b58-109">Permissions</span></span>
<span data-ttu-id="c6b58-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6b58-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6b58-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6b58-112">Permission type</span></span>      | <span data-ttu-id="c6b58-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6b58-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b58-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6b58-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c6b58-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6b58-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6b58-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6b58-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b58-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6b58-117">Not supported.</span></span>    |
|<span data-ttu-id="c6b58-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6b58-118">Application</span></span> | <span data-ttu-id="c6b58-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b58-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6b58-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6b58-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6b58-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c6b58-121">Optional query parameters</span></span>
<span data-ttu-id="c6b58-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c6b58-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6b58-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6b58-123">Request headers</span></span>
| <span data-ttu-id="c6b58-124">名称</span><span class="sxs-lookup"><span data-stu-id="c6b58-124">Name</span></span>       | <span data-ttu-id="c6b58-125">类型</span><span class="sxs-lookup"><span data-stu-id="c6b58-125">Type</span></span> | <span data-ttu-id="c6b58-126">说明</span><span class="sxs-lookup"><span data-stu-id="c6b58-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c6b58-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6b58-127">Authorization</span></span>  | <span data-ttu-id="c6b58-128">string</span><span class="sxs-lookup"><span data-stu-id="c6b58-128">string</span></span>  | <span data-ttu-id="c6b58-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6b58-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6b58-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6b58-131">Request body</span></span>
<span data-ttu-id="c6b58-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6b58-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6b58-133">响应</span><span class="sxs-lookup"><span data-stu-id="c6b58-133">Response</span></span>

<span data-ttu-id="c6b58-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c6b58-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6b58-135">示例</span><span class="sxs-lookup"><span data-stu-id="c6b58-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6b58-136">请求</span><span class="sxs-lookup"><span data-stu-id="c6b58-136">Request</span></span>
<span data-ttu-id="c6b58-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6b58-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="c6b58-138">响应</span><span class="sxs-lookup"><span data-stu-id="c6b58-138">Response</span></span>
<span data-ttu-id="c6b58-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6b58-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
