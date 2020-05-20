---
title: servicePrincipals： List ownedObjects
description: 检索 servicePrincipal 拥有的对象的列表。  这可能包括应用程序或组。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e790368a9d6b2122174517adf5190c8c3440a556
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291102"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="09acb-104">servicePrincipals： List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="09acb-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="09acb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09acb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09acb-106">检索[servicePrincipal](../resources/serviceprincipal.md)拥有的对象的列表。</span><span class="sxs-lookup"><span data-stu-id="09acb-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="09acb-107">这可能包括应用程序或组。</span><span class="sxs-lookup"><span data-stu-id="09acb-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="09acb-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="09acb-108">Permissions</span></span>
<span data-ttu-id="09acb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09acb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09acb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="09acb-111">Permission type</span></span>      | <span data-ttu-id="09acb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09acb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09acb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09acb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="09acb-114">所有的读取全部、全部的 Directory.accessasuser.all、全部、全部、全部、目录、全部、</span><span class="sxs-lookup"><span data-stu-id="09acb-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09acb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09acb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09acb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09acb-116">Not supported.</span></span>    |
|<span data-ttu-id="09acb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="09acb-117">Application</span></span> | <span data-ttu-id="09acb-118">应用程序。全部，全部读取全部，全部为，全部为。</span><span class="sxs-lookup"><span data-stu-id="09acb-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="09acb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09acb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09acb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="09acb-120">Optional query parameters</span></span>
<span data-ttu-id="09acb-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="09acb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09acb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="09acb-122">Request headers</span></span>
| <span data-ttu-id="09acb-123">名称</span><span class="sxs-lookup"><span data-stu-id="09acb-123">Name</span></span>           | <span data-ttu-id="09acb-124">说明</span><span class="sxs-lookup"><span data-stu-id="09acb-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="09acb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="09acb-125">Authorization</span></span>  | <span data-ttu-id="09acb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09acb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09acb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="09acb-128">Request body</span></span>
<span data-ttu-id="09acb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09acb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09acb-130">响应</span><span class="sxs-lookup"><span data-stu-id="09acb-130">Response</span></span>

<span data-ttu-id="09acb-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="09acb-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="09acb-132">示例</span><span class="sxs-lookup"><span data-stu-id="09acb-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="09acb-133">请求</span><span class="sxs-lookup"><span data-stu-id="09acb-133">Request</span></span>
<span data-ttu-id="09acb-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09acb-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/ownedObjects
```

### <a name="response"></a><span data-ttu-id="09acb-135">响应</span><span class="sxs-lookup"><span data-stu-id="09acb-135">Response</span></span>
<span data-ttu-id="09acb-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="09acb-136">Here is an example of the response.</span></span> 
><span data-ttu-id="09acb-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09acb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
