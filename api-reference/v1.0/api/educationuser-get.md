---
title: 获取 educationUser
description: 读取 educationUser 对象的属性和关系。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e550f1dc17f562f0d9f6db51001b4bcc26166eed
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231275"
---
# <a name="get-educationuser"></a><span data-ttu-id="ad053-103">获取 educationUser</span><span class="sxs-lookup"><span data-stu-id="ad053-103">Get educationUser</span></span>

<span data-ttu-id="ad053-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad053-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad053-105">读取 [educationUser 对象的属性和](../resources/educationuser.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ad053-105">Read the properties and relationships of an [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad053-106">权限</span><span class="sxs-lookup"><span data-stu-id="ad053-106">Permissions</span></span>
<span data-ttu-id="ad053-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad053-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad053-109">Permission type</span></span>      | <span data-ttu-id="ad053-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad053-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad053-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad053-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ad053-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ad053-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="ad053-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad053-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ad053-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad053-114">Not supported.</span></span>  |
|<span data-ttu-id="ad053-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad053-115">Application</span></span> | <span data-ttu-id="ad053-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad053-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="ad053-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad053-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ad053-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ad053-118">Optional query parameters</span></span>
<span data-ttu-id="ad053-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ad053-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad053-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad053-120">Request headers</span></span>
| <span data-ttu-id="ad053-121">标头</span><span class="sxs-lookup"><span data-stu-id="ad053-121">Header</span></span>       | <span data-ttu-id="ad053-122">值</span><span class="sxs-lookup"><span data-stu-id="ad053-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad053-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad053-123">Authorization</span></span>  | <span data-ttu-id="ad053-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad053-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad053-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad053-126">Request body</span></span>
<span data-ttu-id="ad053-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad053-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ad053-128">响应</span><span class="sxs-lookup"><span data-stu-id="ad053-128">Response</span></span>
<span data-ttu-id="ad053-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad053-129">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad053-130">示例</span><span class="sxs-lookup"><span data-stu-id="ad053-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad053-131">请求</span><span class="sxs-lookup"><span data-stu-id="ad053-131">Request</span></span>
<span data-ttu-id="ad053-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ad053-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad053-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad053-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="ad053-134">C#</span><span class="sxs-lookup"><span data-stu-id="ad053-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad053-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad053-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad053-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad053-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad053-137">Java</span><span class="sxs-lookup"><span data-stu-id="ad053-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ad053-138">响应</span><span class="sxs-lookup"><span data-stu-id="ad053-138">Response</span></span>
<span data-ttu-id="ad053-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ad053-139">The following is an example of the response.</span></span> 

><span data-ttu-id="ad053-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad053-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationUser",
    "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
    "primaryRole": "String",
    "middleName": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "residenceAddress": {
      "@odata.type": "microsoft.graph.physicalAddress"
    },
    "mailingAddress": {
      "@odata.type": "microsoft.graph.physicalAddress"
    },
    "student": {
      "@odata.type": "microsoft.graph.educationStudent"
    },
    "teacher": {
      "@odata.type": "microsoft.graph.educationTeacher"
    },
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "accountEnabled": "Boolean",
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense"
      }
    ],
    "assignedPlans": [
      {
        "@odata.type": "microsoft.graph.assignedPlan"
      }
    ],
    "businessPhones": [
      "String"
    ],
    "department": "String",
    "displayName": "String",
    "givenName": "String",
    "mail": "String",
    "mailNickname": "String",
    "mobilePhone": "String",
    "passwordPolicies": "String",
    "passwordProfile": {
      "@odata.type": "microsoft.graph.passwordProfile"
    },
    "officeLocation": "String",
    "preferredLanguage": "String",
    "provisionedPlans": [
      {
        "@odata.type": "microsoft.graph.provisionedPlan"
      }
    ],
    "refreshTokensValidFromDateTime": "String (timestamp)",
    "showInAddressList": "Boolean",
    "surname": "String",
    "usageLocation": "String",
    "userPrincipalName": "String",
    "userType": "String",
    "onPremisesInfo": {
      "@odata.type": "microsoft.graph.educationOnPremisesInfo"
    }
  }
}
```
