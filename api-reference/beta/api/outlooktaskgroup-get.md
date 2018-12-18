---
title: 获取 outlookTaskGroup
description: 要获取的属性和指定 Outlook 任务组的关系。
author: angelgolfer-ms
ms.openlocfilehash: c464a6ac9b219ca84538e6d369009e0f5f515c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306746"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="e2d7d-103">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="e2d7d-103">Get outlookTaskGroup</span></span>

> <span data-ttu-id="e2d7d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2d7d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2d7d-106">要获取的属性和指定 Outlook 任务组的关系。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-106">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2d7d-107">权限</span><span class="sxs-lookup"><span data-stu-id="e2d7d-107">Permissions</span></span>
<span data-ttu-id="e2d7d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2d7d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2d7d-110">Permission type</span></span>      | <span data-ttu-id="e2d7d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2d7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2d7d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2d7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2d7d-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e2d7d-113">Tasks.Read</span></span>    |
|<span data-ttu-id="e2d7d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2d7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2d7d-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e2d7d-115">Tasks.Read</span></span>    |
|<span data-ttu-id="e2d7d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2d7d-116">Application</span></span> | <span data-ttu-id="e2d7d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2d7d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2d7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2d7d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2d7d-119">Optional query parameters</span></span>
<span data-ttu-id="e2d7d-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2d7d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2d7d-121">Request headers</span></span>
| <span data-ttu-id="e2d7d-122">Name</span><span class="sxs-lookup"><span data-stu-id="e2d7d-122">Name</span></span>      |<span data-ttu-id="e2d7d-123">说明</span><span class="sxs-lookup"><span data-stu-id="e2d7d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2d7d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2d7d-124">Authorization</span></span>  | <span data-ttu-id="e2d7d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2d7d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2d7d-127">Request body</span></span>
<span data-ttu-id="e2d7d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2d7d-129">响应</span><span class="sxs-lookup"><span data-stu-id="e2d7d-129">Response</span></span>

<span data-ttu-id="e2d7d-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-130">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2d7d-131">示例</span><span class="sxs-lookup"><span data-stu-id="e2d7d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2d7d-132">请求</span><span class="sxs-lookup"><span data-stu-id="e2d7d-132">Request</span></span>
<span data-ttu-id="e2d7d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="e2d7d-134">响应</span><span class="sxs-lookup"><span data-stu-id="e2d7d-134">Response</span></span>
<span data-ttu-id="e2d7d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2d7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->