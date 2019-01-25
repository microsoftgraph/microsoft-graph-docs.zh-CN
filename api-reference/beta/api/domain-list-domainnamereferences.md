---
title: 列出 domainNameReferences
description: 通过对域的引用检索 directoryObject 列表。返回列表将包含依赖域的所有目录对象。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 082c66367e87ad556cd79fa267eb7dfd8f1e0b56
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525764"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="a2c88-104">列出 domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="a2c88-104">List domainNameReferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2c88-p102">通过对域的引用检索 [directoryObject](../resources/directoryobject.md) 列表。返回列表将包含依赖域的所有目录对象。</span><span class="sxs-lookup"><span data-stu-id="a2c88-p102">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2c88-107">权限</span><span class="sxs-lookup"><span data-stu-id="a2c88-107">Permissions</span></span>

<span data-ttu-id="a2c88-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2c88-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a2c88-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2c88-110">Permission type</span></span>      | <span data-ttu-id="a2c88-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2c88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2c88-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2c88-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a2c88-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2c88-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="a2c88-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2c88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2c88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2c88-115">Not supported.</span></span>    |
|<span data-ttu-id="a2c88-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2c88-116">Application</span></span> | <span data-ttu-id="a2c88-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2c88-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2c88-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2c88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="a2c88-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="a2c88-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a2c88-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a2c88-120">Optional query parameters</span></span>

<span data-ttu-id="a2c88-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a2c88-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2c88-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2c88-122">Request headers</span></span>

| <span data-ttu-id="a2c88-123">名称</span><span class="sxs-lookup"><span data-stu-id="a2c88-123">Name</span></span>      |<span data-ttu-id="a2c88-124">说明</span><span class="sxs-lookup"><span data-stu-id="a2c88-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2c88-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2c88-125">Authorization</span></span>  | <span data-ttu-id="a2c88-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2c88-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2c88-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2c88-128">Request body</span></span>

<span data-ttu-id="a2c88-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2c88-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2c88-130">响应</span><span class="sxs-lookup"><span data-stu-id="a2c88-130">Response</span></span>

<span data-ttu-id="a2c88-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2c88-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2c88-132">示例</span><span class="sxs-lookup"><span data-stu-id="a2c88-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2c88-133">请求</span><span class="sxs-lookup"><span data-stu-id="a2c88-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="a2c88-134">响应</span><span class="sxs-lookup"><span data-stu-id="a2c88-134">Response</span></span>
<span data-ttu-id="a2c88-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2c88-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-domainnamereferences.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
