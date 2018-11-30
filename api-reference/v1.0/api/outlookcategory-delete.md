---
title: 删除 Outlook 类别
description: 删除指定的 outlookCategory 对象。
ms.openlocfilehash: 4e28eff91c582fcb234c69cb9930c64c84d71724
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011023"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="50d28-103">删除 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="50d28-103">Delete Outlook category</span></span>


<span data-ttu-id="50d28-104">删除指定的 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50d28-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="50d28-105">权限</span><span class="sxs-lookup"><span data-stu-id="50d28-105">Permissions</span></span>
<span data-ttu-id="50d28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50d28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d28-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="50d28-108">Permission type</span></span>      | <span data-ttu-id="50d28-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50d28-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50d28-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50d28-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50d28-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50d28-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="50d28-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50d28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50d28-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50d28-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="50d28-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="50d28-114">Application</span></span> | <span data-ttu-id="50d28-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50d28-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50d28-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50d28-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50d28-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50d28-117">Optional query parameters</span></span>
<span data-ttu-id="50d28-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="50d28-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50d28-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50d28-119">Request headers</span></span>
| <span data-ttu-id="50d28-120">名称</span><span class="sxs-lookup"><span data-stu-id="50d28-120">Name</span></span>      |<span data-ttu-id="50d28-121">说明</span><span class="sxs-lookup"><span data-stu-id="50d28-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50d28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50d28-122">Authorization</span></span>  | <span data-ttu-id="50d28-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50d28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50d28-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="50d28-125">Request body</span></span>
<span data-ttu-id="50d28-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50d28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50d28-127">响应</span><span class="sxs-lookup"><span data-stu-id="50d28-127">Response</span></span>

<span data-ttu-id="50d28-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="50d28-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d28-130">示例</span><span class="sxs-lookup"><span data-stu-id="50d28-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50d28-131">请求</span><span class="sxs-lookup"><span data-stu-id="50d28-131">Request</span></span>
<span data-ttu-id="50d28-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50d28-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="50d28-133">响应</span><span class="sxs-lookup"><span data-stu-id="50d28-133">Response</span></span>
<span data-ttu-id="50d28-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="50d28-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->