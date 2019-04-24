---
title: 列出所有者
description: 检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 477a8fd2e647d8bdc3babdcb48bccba469912e93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502076"
---
# <a name="list-owners"></a><span data-ttu-id="f039d-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="f039d-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f039d-p102">检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="f039d-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f039d-107">权限</span><span class="sxs-lookup"><span data-stu-id="f039d-107">Permissions</span></span>
<span data-ttu-id="f039d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f039d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f039d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f039d-110">Permission type</span></span>      | <span data-ttu-id="f039d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f039d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f039d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f039d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f039d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f039d-113">Not supported.</span></span>    |
|<span data-ttu-id="f039d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f039d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f039d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f039d-115">Not supported.</span></span>    |
|<span data-ttu-id="f039d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f039d-116">Application</span></span> | <span data-ttu-id="f039d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f039d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f039d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f039d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f039d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f039d-119">Optional query parameters</span></span>
<span data-ttu-id="f039d-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f039d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f039d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f039d-121">Request headers</span></span>
| <span data-ttu-id="f039d-122">名称</span><span class="sxs-lookup"><span data-stu-id="f039d-122">Name</span></span>       | <span data-ttu-id="f039d-123">类型</span><span class="sxs-lookup"><span data-stu-id="f039d-123">Type</span></span> | <span data-ttu-id="f039d-124">说明</span><span class="sxs-lookup"><span data-stu-id="f039d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f039d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f039d-125">Authorization</span></span>  | <span data-ttu-id="f039d-126">string</span><span class="sxs-lookup"><span data-stu-id="f039d-126">string</span></span>  | <span data-ttu-id="f039d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f039d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f039d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f039d-129">Request body</span></span>
<span data-ttu-id="f039d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f039d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f039d-131">响应</span><span class="sxs-lookup"><span data-stu-id="f039d-131">Response</span></span>
<span data-ttu-id="f039d-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f039d-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f039d-133">示例</span><span class="sxs-lookup"><span data-stu-id="f039d-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f039d-134">请求</span><span class="sxs-lookup"><span data-stu-id="f039d-134">Request</span></span>
<span data-ttu-id="f039d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f039d-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="f039d-136">响应</span><span class="sxs-lookup"><span data-stu-id="f039d-136">Response</span></span>
<span data-ttu-id="f039d-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f039d-137">The following is an example of the response.</span></span>
><span data-ttu-id="f039d-138">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f039d-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f039d-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f039d-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
