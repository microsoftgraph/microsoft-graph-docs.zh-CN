---
title: 获取 educationSchool
description: 读取 educationSchool 对象的属性和关系。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3ec682a7674bc24eca3d168e3f92b3d3c05f3bda
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474900"
---
# <a name="get-educationschool"></a><span data-ttu-id="8a48f-103">获取 educationSchool</span><span class="sxs-lookup"><span data-stu-id="8a48f-103">Get educationSchool</span></span>

<span data-ttu-id="8a48f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a48f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a48f-105">读取 [educationSchool 对象的属性和](../resources/educationschool.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="8a48f-105">Read the properties and relationships of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a48f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8a48f-106">Permissions</span></span>

<span data-ttu-id="8a48f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a48f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a48f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a48f-109">Permission type</span></span>                        | <span data-ttu-id="8a48f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a48f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8a48f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a48f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a48f-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8a48f-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="8a48f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a48f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a48f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a48f-114">Not supported.</span></span>                              |
| <span data-ttu-id="8a48f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a48f-115">Application</span></span>                            | <span data-ttu-id="8a48f-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a48f-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a48f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a48f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a48f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8a48f-118">Optional query parameters</span></span>

<span data-ttu-id="8a48f-119">此方法支持与 Get User 相同的 OData [查询参数](../api/user-get.md#optional-query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8a48f-119">This method supports the same OData query parameters as [Get User](../api/user-get.md#optional-query-parameters).</span></span> <span data-ttu-id="8a48f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8a48f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a48f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a48f-121">Request headers</span></span>

| <span data-ttu-id="8a48f-122">名称</span><span class="sxs-lookup"><span data-stu-id="8a48f-122">Name</span></span>          | <span data-ttu-id="8a48f-123">说明</span><span class="sxs-lookup"><span data-stu-id="8a48f-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8a48f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a48f-124">Authorization</span></span> | <span data-ttu-id="8a48f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a48f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a48f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a48f-127">Request body</span></span>

<span data-ttu-id="8a48f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a48f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a48f-129">响应</span><span class="sxs-lookup"><span data-stu-id="8a48f-129">Response</span></span>

<span data-ttu-id="8a48f-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a48f-130">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a48f-131">示例</span><span class="sxs-lookup"><span data-stu-id="8a48f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a48f-132">请求</span><span class="sxs-lookup"><span data-stu-id="8a48f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8a48f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a48f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{educationSchoolId}
```
# <a name="c"></a>[<span data-ttu-id="8a48f-134">C#</span><span class="sxs-lookup"><span data-stu-id="8a48f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a48f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a48f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a48f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a48f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a48f-137">Java</span><span class="sxs-lookup"><span data-stu-id="8a48f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a48f-138">响应</span><span class="sxs-lookup"><span data-stu-id="8a48f-138">Response</span></span>

><span data-ttu-id="8a48f-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8a48f-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSchool",
    "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
    "displayName": "String",
    "description": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "principalEmail": "String",
    "principalName": "String",
    "externalPrincipalId": "String",
    "lowestGrade": "String",
    "highestGrade": "String",
    "schoolNumber": "String",
    "externalId": "String",
    "phone": "String",
    "fax": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  }
}
```
