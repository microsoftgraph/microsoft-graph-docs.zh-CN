---
title: 列出 orgContacts
description: 检索此组织的组织联系人列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ced1cd140f322617d1b7a75d1af83fd938360fc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622593"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="7ecd8-103">列出 orgContacts</span><span class="sxs-lookup"><span data-stu-id="7ecd8-103">List orgContacts</span></span>

<span data-ttu-id="7ecd8-104">获取此组织的[组织联系人](../resources/orgcontact.md)列表。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-104">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ecd8-105">权限</span><span class="sxs-lookup"><span data-stu-id="7ecd8-105">Permissions</span></span>
<span data-ttu-id="7ecd8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ecd8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ecd8-108">Permission type</span></span>      | <span data-ttu-id="7ecd8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ecd8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ecd8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ecd8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ecd8-111">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ecd8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ecd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ecd8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-113">Not supported.</span></span>    |
|<span data-ttu-id="7ecd8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ecd8-114">Application</span></span> | <span data-ttu-id="7ecd8-115">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ecd8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ecd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ecd8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7ecd8-117">Optional query parameters</span></span>
<span data-ttu-id="7ecd8-118">此方法支持`$expand`、 `$filter`、 `$select`和`$top` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-118">This method supports the `$expand`, `$filter`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ecd8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ecd8-119">Request headers</span></span>
| <span data-ttu-id="7ecd8-120">标头</span><span class="sxs-lookup"><span data-stu-id="7ecd8-120">Header</span></span>       | <span data-ttu-id="7ecd8-121">值</span><span class="sxs-lookup"><span data-stu-id="7ecd8-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7ecd8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ecd8-122">Authorization</span></span>  |<span data-ttu-id="7ecd8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ecd8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ecd8-125">Request body</span></span>
<span data-ttu-id="7ecd8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ecd8-127">响应</span><span class="sxs-lookup"><span data-stu-id="7ecd8-127">Response</span></span>

<span data-ttu-id="7ecd8-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-128">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ecd8-129">示例</span><span class="sxs-lookup"><span data-stu-id="7ecd8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ecd8-130">请求</span><span class="sxs-lookup"><span data-stu-id="7ecd8-130">Request</span></span>
<span data-ttu-id="7ecd8-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/v1.0/contacts
```

##### <a name="response"></a><span data-ttu-id="7ecd8-132">响应</span><span class="sxs-lookup"><span data-stu-id="7ecd8-132">Response</span></span>
<span data-ttu-id="7ecd8-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-133">The following is an example of the response.</span></span>
><span data-ttu-id="7ecd8-134">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7ecd8-134">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "addresses":[
          {
            "city": "string",
            "countryOrRegion": "string",
            "officeLocation": "string",
            "postalCode": "string",
            "state": "string",
            "street": "string"
          }
      ],
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "phones":[
          {
            "type": "string",
            "number": "string"
          }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
