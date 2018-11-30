---
title: 列出成员
description: 检索参加课程的教师和学生。 请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。
ms.openlocfilehash: e8f31720733fec3942d4ddb35fa7f2fdac1b26f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042003"
---
# <a name="list-members"></a><span data-ttu-id="4ace2-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="4ace2-104">List members</span></span>

> <span data-ttu-id="4ace2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ace2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ace2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ace2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ace2-107">检索参加课程的教师和学生。</span><span class="sxs-lookup"><span data-stu-id="4ace2-107">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="4ace2-108">请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。</span><span class="sxs-lookup"><span data-stu-id="4ace2-108">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ace2-109">权限</span><span class="sxs-lookup"><span data-stu-id="4ace2-109">Permissions</span></span>
<span data-ttu-id="4ace2-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ace2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ace2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ace2-112">Permission type</span></span>      | <span data-ttu-id="4ace2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ace2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ace2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ace2-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="4ace2-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="4ace2-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="4ace2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ace2-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4ace2-117">不支持</span><span class="sxs-lookup"><span data-stu-id="4ace2-117">Not supported</span></span>  |
|<span data-ttu-id="4ace2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ace2-118">Application</span></span> | <span data-ttu-id="4ace2-119">EduRoster.Read.All、 EduRoster.ReadWrite.All 以及 Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="4ace2-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4ace2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ace2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ace2-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ace2-121">Optional query parameters</span></span>
<span data-ttu-id="4ace2-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ace2-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ace2-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ace2-123">Request headers</span></span>
| <span data-ttu-id="4ace2-124">标头</span><span class="sxs-lookup"><span data-stu-id="4ace2-124">Header</span></span>       | <span data-ttu-id="4ace2-125">值</span><span class="sxs-lookup"><span data-stu-id="4ace2-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ace2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ace2-126">Authorization</span></span>  | <span data-ttu-id="4ace2-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ace2-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ace2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ace2-129">Request body</span></span>
<span data-ttu-id="4ace2-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ace2-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4ace2-131">响应</span><span class="sxs-lookup"><span data-stu-id="4ace2-131">Response</span></span>
<span data-ttu-id="4ace2-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4ace2-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ace2-133">示例</span><span class="sxs-lookup"><span data-stu-id="4ace2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ace2-134">请求</span><span class="sxs-lookup"><span data-stu-id="4ace2-134">Request</span></span>
<span data-ttu-id="4ace2-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ace2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11016/members
```
##### <a name="response"></a><span data-ttu-id="4ace2-136">响应</span><span class="sxs-lookup"><span data-stu-id="4ace2-136">Response</span></span>
<span data-ttu-id="4ace2-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ace2-137">The following is an example of the response.</span></span> 

><span data-ttu-id="4ace2-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4ace2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "externalId": "13013",
      "teacherNumber": "8802",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z",
      "gender": "female",
      "grade": "9",
      "graduationYear": "2019",
      "studentNumber": "13005",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
