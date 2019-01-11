---
title: 列表 orgContacts
description: 检索为组织的组织联系人列表中。
localization_priority: Normal
ms.openlocfilehash: 0b4dc4a099562b8817396bee8f3141fa32c28572
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831974"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="c88c5-103">列表 orgContacts</span><span class="sxs-lookup"><span data-stu-id="c88c5-103">List orgContacts</span></span>

> <span data-ttu-id="c88c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c88c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c88c5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c88c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c88c5-106">检索为组织的组织联系人列表中。</span><span class="sxs-lookup"><span data-stu-id="c88c5-106">Retrieve the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c88c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="c88c5-107">Permissions</span></span>
<span data-ttu-id="c88c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c88c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c88c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c88c5-110">Permission type</span></span>      | <span data-ttu-id="c88c5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c88c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c88c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c88c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c88c5-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c88c5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c88c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c88c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88c5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c88c5-115">Not supported.</span></span>    |
|<span data-ttu-id="c88c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c88c5-116">Application</span></span> | <span data-ttu-id="c88c5-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c88c5-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88c5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c88c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c88c5-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c88c5-119">Optional query parameters</span></span>
<span data-ttu-id="c88c5-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c88c5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c88c5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c88c5-121">Request headers</span></span>
| <span data-ttu-id="c88c5-122">名称</span><span class="sxs-lookup"><span data-stu-id="c88c5-122">Name</span></span>       | <span data-ttu-id="c88c5-123">类型</span><span class="sxs-lookup"><span data-stu-id="c88c5-123">Type</span></span> | <span data-ttu-id="c88c5-124">说明</span><span class="sxs-lookup"><span data-stu-id="c88c5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c88c5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c88c5-125">Authorization</span></span>  | <span data-ttu-id="c88c5-126">string</span><span class="sxs-lookup"><span data-stu-id="c88c5-126">string</span></span>  | <span data-ttu-id="c88c5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c88c5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c88c5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c88c5-129">Request body</span></span>
<span data-ttu-id="c88c5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c88c5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c88c5-131">响应</span><span class="sxs-lookup"><span data-stu-id="c88c5-131">Response</span></span>

<span data-ttu-id="c88c5-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[orgContact](../resources/orgcontact.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c88c5-132">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c88c5-133">示例</span><span class="sxs-lookup"><span data-stu-id="c88c5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c88c5-134">请求</span><span class="sxs-lookup"><span data-stu-id="c88c5-134">Request</span></span>
<span data-ttu-id="c88c5-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c88c5-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
##### <a name="response"></a><span data-ttu-id="c88c5-136">响应</span><span class="sxs-lookup"><span data-stu-id="c88c5-136">Response</span></span>
<span data-ttu-id="c88c5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c88c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
