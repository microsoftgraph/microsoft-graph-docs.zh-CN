---
title: 向服务主体授予的 List appRoleAssignments
description: 检索授予服务主体的应用程序角色分配的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: b16b48affc8d4ba07305537ed805294f8b2475e3
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345917"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="13267-103">向服务主体授予的 List appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="13267-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="13267-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13267-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13267-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13267-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13267-106">检索已授予服务主体的[appRoleAssignment](../resources/approleassignment.md)列表。</span><span class="sxs-lookup"><span data-stu-id="13267-106">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="13267-107">分配给服务主体的应用程序角色也称为 "[应用程序权限](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types)"。</span><span class="sxs-lookup"><span data-stu-id="13267-107">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="13267-108">可以通过创建应用程序角色分配或通过[许可体验](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience)直接授予应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="13267-108">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="13267-109">权限</span><span class="sxs-lookup"><span data-stu-id="13267-109">Permissions</span></span>

<span data-ttu-id="13267-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13267-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13267-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="13267-112">Permission type</span></span>      | <span data-ttu-id="13267-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13267-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13267-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13267-114">Delegated (work or school account)</span></span> | <span data-ttu-id="13267-115">"Application"、"all"、"Directory.accessasuser.all"、"全部"、"全部"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="13267-115">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="13267-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13267-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13267-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="13267-117">Not supported.</span></span>    |
|<span data-ttu-id="13267-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="13267-118">Application</span></span> | <span data-ttu-id="13267-119">"Application"、"all"、"全部"、"所有"、"所有"、"所有"</span><span class="sxs-lookup"><span data-stu-id="13267-119">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13267-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13267-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13267-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="13267-121">Optional query parameters</span></span>

<span data-ttu-id="13267-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13267-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13267-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="13267-123">Request headers</span></span>

| <span data-ttu-id="13267-124">名称</span><span class="sxs-lookup"><span data-stu-id="13267-124">Name</span></span>           | <span data-ttu-id="13267-125">说明</span><span class="sxs-lookup"><span data-stu-id="13267-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="13267-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="13267-126">Authorization</span></span>  | <span data-ttu-id="13267-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13267-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13267-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="13267-129">Request body</span></span>

<span data-ttu-id="13267-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13267-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13267-131">响应</span><span class="sxs-lookup"><span data-stu-id="13267-131">Response</span></span>

<span data-ttu-id="13267-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="13267-132">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13267-133">示例</span><span class="sxs-lookup"><span data-stu-id="13267-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="13267-134">请求</span><span class="sxs-lookup"><span data-stu-id="13267-134">Request</span></span>

<span data-ttu-id="13267-135">下面的示例演示了检索已分配给服务主体的应用程序角色的请求。</span><span class="sxs-lookup"><span data-stu-id="13267-135">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="13267-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="13267-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="13267-137">C#</span><span class="sxs-lookup"><span data-stu-id="13267-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13267-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13267-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13267-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13267-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="13267-140">响应</span><span class="sxs-lookup"><span data-stu-id="13267-140">Response</span></span>

<span data-ttu-id="13267-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="13267-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="13267-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13267-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
