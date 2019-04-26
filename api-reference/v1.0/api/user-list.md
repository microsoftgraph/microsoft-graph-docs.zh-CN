---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7529097f5d22443b95123cc7a2f578f0521b8ca4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563894"
---
# <a name="list-users"></a><span data-ttu-id="ee959-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="ee959-103">List users</span></span>

<span data-ttu-id="ee959-104">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ee959-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee959-105">权限</span><span class="sxs-lookup"><span data-stu-id="ee959-105">Permissions</span></span>

<span data-ttu-id="ee959-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee959-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee959-108">Permission type</span></span>      | <span data-ttu-id="ee959-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee959-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee959-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee959-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee959-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee959-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee959-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee959-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee959-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee959-113">Not supported.</span></span>    |
|<span data-ttu-id="ee959-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee959-114">Application</span></span> | <span data-ttu-id="ee959-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee959-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee959-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee959-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee959-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ee959-117">Optional query parameters</span></span>

<span data-ttu-id="ee959-118">此方法支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ee959-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ee959-119">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="ee959-119">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="ee959-120">若要返回其他属性，必须使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="ee959-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="ee959-121">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="ee959-121">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="ee959-p103">注意：某些属性无法在用户集合中返回。以下属性仅在[检索单个用户 ](./user-get.md) 时受支持：_aboutMe、birthday、hireDate、interests、mySite、pastProjects、preferredName、responsibilities、schools、skills、mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="ee959-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee959-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee959-124">Request headers</span></span>

| <span data-ttu-id="ee959-125">标头</span><span class="sxs-lookup"><span data-stu-id="ee959-125">Header</span></span>        | <span data-ttu-id="ee959-126">值</span><span class="sxs-lookup"><span data-stu-id="ee959-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="ee959-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee959-127">Authorization</span></span> | <span data-ttu-id="ee959-128">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="ee959-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="ee959-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee959-129">Content-Type</span></span>  | <span data-ttu-id="ee959-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ee959-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="ee959-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee959-131">Request body</span></span>

<span data-ttu-id="ee959-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee959-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee959-133">响应</span><span class="sxs-lookup"><span data-stu-id="ee959-133">Response</span></span>

<span data-ttu-id="ee959-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ee959-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee959-135">示例</span><span class="sxs-lookup"><span data-stu-id="ee959-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="ee959-136">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="ee959-136">Example 1: Standard users request</span></span>

<span data-ttu-id="ee959-137">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="ee959-137">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="ee959-138">此示例演示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="ee959-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="ee959-139">请求</span><span class="sxs-lookup"><span data-stu-id="ee959-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="ee959-140">响应</span><span class="sxs-lookup"><span data-stu-id="ee959-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="ee959-141">示例 2：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="ee959-141">Example 2: Users request using $select</span></span>

<span data-ttu-id="ee959-142">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="ee959-142">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="ee959-143">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="ee959-143">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="ee959-144">请求</span><span class="sxs-lookup"><span data-stu-id="ee959-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="ee959-145">响应</span><span class="sxs-lookup"><span data-stu-id="ee959-145">Response</span></span>

<span data-ttu-id="ee959-146">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee959-146">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
