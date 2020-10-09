---
title: List servicePrincipal transitive memberOf
description: 获取此服务主体所属的组和目录角色。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 6f4b3e0bf58590c151a1e0c3e3d781d642c1f671
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404110"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="ebab4-103">List servicePrincipal transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="ebab4-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="ebab4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebab4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebab4-105">获取此 [servicePrincipal](../resources/serviceprincipal.md) 所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="ebab4-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="ebab4-106">此操作是可传递的，将包括此服务主体以嵌套方式所属的组。</span><span class="sxs-lookup"><span data-stu-id="ebab4-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebab4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ebab4-107">Permissions</span></span>
<span data-ttu-id="ebab4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebab4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebab4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebab4-110">Permission type</span></span>      | <span data-ttu-id="ebab4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebab4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebab4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebab4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebab4-113">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ebab4-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ebab4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebab4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebab4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebab4-115">Not supported.</span></span>    |
|<span data-ttu-id="ebab4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebab4-116">Application</span></span> | <span data-ttu-id="ebab4-117">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebab4-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ebab4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebab4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebab4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ebab4-119">Optional query parameters</span></span>
<span data-ttu-id="ebab4-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ebab4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebab4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebab4-121">Request headers</span></span>
| <span data-ttu-id="ebab4-122">名称</span><span class="sxs-lookup"><span data-stu-id="ebab4-122">Name</span></span>           | <span data-ttu-id="ebab4-123">说明</span><span class="sxs-lookup"><span data-stu-id="ebab4-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="ebab4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebab4-124">Authorization</span></span>  | <span data-ttu-id="ebab4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebab4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebab4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebab4-127">Request body</span></span>
<span data-ttu-id="ebab4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebab4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebab4-129">响应</span><span class="sxs-lookup"><span data-stu-id="ebab4-129">Response</span></span>

<span data-ttu-id="ebab4-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ebab4-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebab4-131">示例</span><span class="sxs-lookup"><span data-stu-id="ebab4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebab4-132">请求</span><span class="sxs-lookup"><span data-stu-id="ebab4-132">Request</span></span>

<span data-ttu-id="ebab4-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebab4-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ebab4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebab4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="ebab4-135">C#</span><span class="sxs-lookup"><span data-stu-id="ebab4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebab4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebab4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebab4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebab4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ebab4-138">响应</span><span class="sxs-lookup"><span data-stu-id="ebab4-138">Response</span></span>

<span data-ttu-id="ebab4-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebab4-139">Here is an example of the response.</span></span> 

><span data-ttu-id="ebab4-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ebab4-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->