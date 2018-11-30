---
title: 列表 taskGroups
description: 获取用户的邮箱中的所有 Outlook 任务组。
ms.openlocfilehash: ba4291f72c1fc6afe3c5f445026169d11f8030db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046820"
---
# <a name="list-taskgroups"></a><span data-ttu-id="0dba5-103">列表 taskGroups</span><span class="sxs-lookup"><span data-stu-id="0dba5-103">List taskGroups</span></span>

> <span data-ttu-id="0dba5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0dba5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0dba5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0dba5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0dba5-106">获取用户的邮箱中的所有 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="0dba5-106">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="0dba5-107">响应始终包括默认任务组`My Tasks`，以及任何其他已创建的邮箱中的任务组。</span><span class="sxs-lookup"><span data-stu-id="0dba5-107">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="0dba5-108">权限</span><span class="sxs-lookup"><span data-stu-id="0dba5-108">Permissions</span></span>
<span data-ttu-id="0dba5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0dba5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dba5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0dba5-111">Permission type</span></span>      | <span data-ttu-id="0dba5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0dba5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dba5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0dba5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0dba5-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0dba5-114">Tasks.Read</span></span>    |
|<span data-ttu-id="0dba5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0dba5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dba5-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0dba5-116">Tasks.Read</span></span>    |
|<span data-ttu-id="0dba5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0dba5-117">Application</span></span> | <span data-ttu-id="0dba5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dba5-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dba5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0dba5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0dba5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0dba5-120">Optional query parameters</span></span>
<span data-ttu-id="0dba5-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0dba5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0dba5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0dba5-122">Request headers</span></span>
| <span data-ttu-id="0dba5-123">名称</span><span class="sxs-lookup"><span data-stu-id="0dba5-123">Name</span></span>      |<span data-ttu-id="0dba5-124">说明</span><span class="sxs-lookup"><span data-stu-id="0dba5-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0dba5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dba5-125">Authorization</span></span>  | <span data-ttu-id="0dba5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0dba5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dba5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0dba5-128">Request body</span></span>
<span data-ttu-id="0dba5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0dba5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dba5-130">响应</span><span class="sxs-lookup"><span data-stu-id="0dba5-130">Response</span></span>

<span data-ttu-id="0dba5-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0dba5-131">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0dba5-132">示例</span><span class="sxs-lookup"><span data-stu-id="0dba5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0dba5-133">请求</span><span class="sxs-lookup"><span data-stu-id="0dba5-133">Request</span></span>
<span data-ttu-id="0dba5-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0dba5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="0dba5-135">响应</span><span class="sxs-lookup"><span data-stu-id="0dba5-135">Response</span></span>
<span data-ttu-id="0dba5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0dba5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->