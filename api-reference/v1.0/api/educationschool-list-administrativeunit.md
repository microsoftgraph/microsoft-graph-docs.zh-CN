---
title: 列出 administrativeUnit an educationSchool
description: 获取与 educationSchool 对象关联的 administrativeUnits 列表。
author: mmast
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a8ca5a51c6fb71c3cab0d6f0a7be239eb2101999
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474848"
---
# <a name="list-administrativeunit-an-educationschool"></a><span data-ttu-id="df9df-103">列出 administrativeUnit an educationSchool</span><span class="sxs-lookup"><span data-stu-id="df9df-103">List administrativeUnit an educationSchool</span></span>

<span data-ttu-id="df9df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df9df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df9df-105">获取与 [educationSchool](../resources/educationschool.md)对象关联的 **administrativeUnits** 列表。</span><span class="sxs-lookup"><span data-stu-id="df9df-105">Get a list of **administrativeUnits** associated with an [educationSchool](../resources/educationschool.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="df9df-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="df9df-106">Permissions</span></span>

<span data-ttu-id="df9df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df9df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df9df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df9df-109">Permission type</span></span>                        | <span data-ttu-id="df9df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df9df-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="df9df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df9df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df9df-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="df9df-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="df9df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df9df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df9df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df9df-114">Not supported.</span></span>                              |
| <span data-ttu-id="df9df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df9df-115">Application</span></span>                            | <span data-ttu-id="df9df-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df9df-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df9df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df9df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}/administrativeUnit
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df9df-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="df9df-118">Optional query parameters</span></span>

<span data-ttu-id="df9df-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="df9df-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="df9df-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="df9df-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="df9df-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="df9df-121">Request headers</span></span>

| <span data-ttu-id="df9df-122">名称</span><span class="sxs-lookup"><span data-stu-id="df9df-122">Name</span></span>          | <span data-ttu-id="df9df-123">说明</span><span class="sxs-lookup"><span data-stu-id="df9df-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="df9df-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="df9df-124">Authorization</span></span> | <span data-ttu-id="df9df-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df9df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df9df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df9df-127">Request body</span></span>

<span data-ttu-id="df9df-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df9df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df9df-129">响应</span><span class="sxs-lookup"><span data-stu-id="df9df-129">Response</span></span>

<span data-ttu-id="df9df-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="df9df-130">If successful, this method returns a `200 OK` response code and a collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df9df-131">示例</span><span class="sxs-lookup"><span data-stu-id="df9df-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df9df-132">请求</span><span class="sxs-lookup"><span data-stu-id="df9df-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="df9df-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="df9df-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_administrativeunit"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit
```
# <a name="c"></a>[<span data-ttu-id="df9df-134">C#</span><span class="sxs-lookup"><span data-stu-id="df9df-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df9df-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df9df-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df9df-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df9df-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df9df-137">Java</span><span class="sxs-lookup"><span data-stu-id="df9df-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df9df-138">响应</span><span class="sxs-lookup"><span data-stu-id="df9df-138">Response</span></span>

> <span data-ttu-id="df9df-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="df9df-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.administrativeUnit",
      "id": "03e281d6-81d6-03e2-d681-e203d681e203",
      "deletedDateTime": "String (timestamp)",
      "displayName": "String",
      "description": "String",
      "visibility": "String"
    }
  ]
}
```
