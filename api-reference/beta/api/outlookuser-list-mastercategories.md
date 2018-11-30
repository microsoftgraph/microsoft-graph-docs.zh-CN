---
title: 列出 Outlook 类别
description: 获取为用户定义的所有类别。
ms.openlocfilehash: 7eff66ea876c88e6a75953f4bd219e817a9a2e2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046817"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="0b395-103">列出 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="0b395-103">List Outlook categories</span></span>

> <span data-ttu-id="0b395-104">**重要说明**： 在 Microsoft Graph 中的 /beta 版本下的 Api 在预览，并会受到更改。</span><span class="sxs-lookup"><span data-stu-id="0b395-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b395-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b395-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b395-106">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="0b395-106">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b395-107">权限</span><span class="sxs-lookup"><span data-stu-id="0b395-107">Permissions</span></span>
<span data-ttu-id="0b395-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b395-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b395-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b395-110">Permission type</span></span>      | <span data-ttu-id="0b395-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b395-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b395-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b395-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b395-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0b395-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0b395-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b395-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b395-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0b395-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0b395-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b395-116">Application</span></span> | <span data-ttu-id="0b395-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0b395-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b395-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b395-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b395-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b395-119">Optional query parameters</span></span>
<span data-ttu-id="0b395-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b395-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b395-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b395-121">Request headers</span></span>
| <span data-ttu-id="0b395-122">名称</span><span class="sxs-lookup"><span data-stu-id="0b395-122">Name</span></span>      |<span data-ttu-id="0b395-123">说明</span><span class="sxs-lookup"><span data-stu-id="0b395-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b395-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b395-124">Authorization</span></span>  | <span data-ttu-id="0b395-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b395-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b395-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b395-127">Request body</span></span>
<span data-ttu-id="0b395-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b395-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b395-129">响应</span><span class="sxs-lookup"><span data-stu-id="0b395-129">Response</span></span>

<span data-ttu-id="0b395-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0b395-130">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b395-131">示例</span><span class="sxs-lookup"><span data-stu-id="0b395-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b395-132">请求</span><span class="sxs-lookup"><span data-stu-id="0b395-132">Request</span></span>
<span data-ttu-id="0b395-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b395-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="0b395-134">响应</span><span class="sxs-lookup"><span data-stu-id="0b395-134">Response</span></span>
<span data-ttu-id="0b395-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b395-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->