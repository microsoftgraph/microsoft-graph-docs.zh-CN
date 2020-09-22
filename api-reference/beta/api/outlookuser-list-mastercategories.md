---
title: 列出 Outlook 类别
description: 获取为用户定义的所有类别。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2eac32961535487627ced870cbc859455db2d5cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036216"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="24948-103">列出 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="24948-103">List Outlook categories</span></span>

<span data-ttu-id="24948-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24948-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24948-105">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="24948-105">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="24948-106">权限</span><span class="sxs-lookup"><span data-stu-id="24948-106">Permissions</span></span>
<span data-ttu-id="24948-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24948-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24948-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24948-109">Permission type</span></span>      | <span data-ttu-id="24948-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24948-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24948-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24948-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24948-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="24948-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="24948-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24948-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24948-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="24948-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="24948-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24948-115">Application</span></span> | <span data-ttu-id="24948-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="24948-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="24948-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24948-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24948-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="24948-118">Optional query parameters</span></span>
<span data-ttu-id="24948-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="24948-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24948-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="24948-120">Request headers</span></span>
| <span data-ttu-id="24948-121">名称</span><span class="sxs-lookup"><span data-stu-id="24948-121">Name</span></span>      |<span data-ttu-id="24948-122">说明</span><span class="sxs-lookup"><span data-stu-id="24948-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24948-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24948-123">Authorization</span></span>  | <span data-ttu-id="24948-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24948-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24948-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="24948-126">Request body</span></span>
<span data-ttu-id="24948-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24948-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24948-128">响应</span><span class="sxs-lookup"><span data-stu-id="24948-128">Response</span></span>

<span data-ttu-id="24948-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="24948-129">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24948-130">示例</span><span class="sxs-lookup"><span data-stu-id="24948-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24948-131">请求</span><span class="sxs-lookup"><span data-stu-id="24948-131">Request</span></span>
<span data-ttu-id="24948-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24948-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="24948-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="24948-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
# <a name="c"></a>[<span data-ttu-id="24948-134">C#</span><span class="sxs-lookup"><span data-stu-id="24948-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mastercategories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24948-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24948-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mastercategories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24948-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24948-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mastercategories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="24948-137">响应</span><span class="sxs-lookup"><span data-stu-id="24948-137">Response</span></span>
<span data-ttu-id="24948-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24948-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


