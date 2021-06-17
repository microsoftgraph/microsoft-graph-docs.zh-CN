---
title: 获取 educationSynchronizationErrors
description: '获取验证期间和/或同步租户中的特定学校数据同步配置文件期间生成的错误。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6bcf581d70d3c214bc18904d73ba5a69a1321824
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971060"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="c4698-103">获取 educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="c4698-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="c4698-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4698-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4698-105">获取验证期间和/或同步租户中的特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 期间生成的错误。</span><span class="sxs-lookup"><span data-stu-id="c4698-105">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4698-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4698-106">Permissions</span></span>

<span data-ttu-id="c4698-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4698-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4698-109">Permission type</span></span>                       | <span data-ttu-id="c4698-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4698-110">Permissions (from least to most privileged)</span></span>                 |
| :------------------------------------ | :---------------------------------------------------------- |
| <span data-ttu-id="c4698-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4698-111">Delegated (work or school account)</span></span>    | <span data-ttu-id="c4698-112">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4698-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span>         |
| <span data-ttu-id="c4698-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="c4698-113">Delegated (personal Microsoft account</span></span> | <span data-ttu-id="c4698-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4698-114">Not supported.</span></span>                                              |
| <span data-ttu-id="c4698-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4698-115">Application</span></span>                           | <span data-ttu-id="c4698-116">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4698-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4698-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4698-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/synchronizationProfiles/{id}/errors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4698-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4698-118">Optional query parameters</span></span>

<span data-ttu-id="c4698-119">此方法支持以下 [OData](/graph/query-parameters) 查询参数来帮助自定义响应：$filter、$orderby、$top、$skip 和 \$ count。</span><span class="sxs-lookup"><span data-stu-id="c4698-119">This method supports the following [OData Query Parameters](/graph/query-parameters) to help customize the response: $filter, $orderby, $top, $skip, and \$count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4698-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4698-120">Request headers</span></span>

| <span data-ttu-id="c4698-121">名称</span><span class="sxs-lookup"><span data-stu-id="c4698-121">Name</span></span>          | <span data-ttu-id="c4698-122">类型</span><span class="sxs-lookup"><span data-stu-id="c4698-122">Type</span></span>   | <span data-ttu-id="c4698-123">说明</span><span class="sxs-lookup"><span data-stu-id="c4698-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="c4698-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4698-124">Authorization</span></span> | <span data-ttu-id="c4698-125">string</span><span class="sxs-lookup"><span data-stu-id="c4698-125">string</span></span> | <span data-ttu-id="c4698-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4698-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4698-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4698-128">Request body</span></span>

<span data-ttu-id="c4698-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4698-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4698-130">响应</span><span class="sxs-lookup"><span data-stu-id="c4698-130">Response</span></span>

<span data-ttu-id="c4698-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [同步错误](../resources/educationsynchronizationerror.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c4698-131">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4698-132">示例</span><span class="sxs-lookup"><span data-stu-id="c4698-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c4698-133">请求</span><span class="sxs-lookup"><span data-stu-id="c4698-133">Request</span></span>

<span data-ttu-id="c4698-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4698-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4698-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4698-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="c"></a>[<span data-ttu-id="c4698-136">C#</span><span class="sxs-lookup"><span data-stu-id="c4698-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4698-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4698-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4698-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4698-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4698-139">Java</span><span class="sxs-lookup"><span data-stu-id="c4698-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-error-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c4698-140">响应</span><span class="sxs-lookup"><span data-stu-id="c4698-140">Response</span></span>

<span data-ttu-id="c4698-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c4698-141">The following is an example of the response.</span></span>

> <span data-ttu-id="c4698-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c4698-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/errors",
  "@odata.count": 14,
  "value": [
    {
      "id": "92797B7C-02C3-4326-8ACC-E81C78753831",
      "entryType": "Student",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
      "joiningValue": "richard.2wilson@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:45Z",
      "reportableIdentifier": "richard.2wilson"
    },
    {
      "id": "94C1EB0E-8339-4EF4-8CB2-EB15C6228CE1",
      "entryType": "Teacher",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
      "joiningValue": "alberto2.dorsey@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:57Z",
      "reportableIdentifier": "alberto2.dorsey"
    },
    {
      "id": "98A82052-7716-49E9-90CC-C6FF406FC8E5",
      "entryType": "Teacher",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
      "joiningValue": "madeline2.bullock@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:57Z",
      "reportableIdentifier": "madeline2.bullock"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
