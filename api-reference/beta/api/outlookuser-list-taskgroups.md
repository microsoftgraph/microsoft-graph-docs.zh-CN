---
title: 列出 taskGroups
description: 获取用户邮箱中的所有 Outlook 任务组。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ec1d32d40c1d9478111fac937f5a72a01965e96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337929"
---
# <a name="list-taskgroups"></a><span data-ttu-id="6fb2e-103">列出 taskGroups</span><span class="sxs-lookup"><span data-stu-id="6fb2e-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb2e-104">获取用户邮箱中的所有 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="6fb2e-105">响应始终包括默认任务组`My Tasks`以及邮箱中已创建的任何其他任务组。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fb2e-106">权限</span><span class="sxs-lookup"><span data-stu-id="6fb2e-106">Permissions</span></span>
<span data-ttu-id="6fb2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb2e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fb2e-109">Permission type</span></span>      | <span data-ttu-id="6fb2e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fb2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb2e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb2e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb2e-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="6fb2e-112">Tasks.Read</span></span>    |
|<span data-ttu-id="6fb2e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb2e-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="6fb2e-114">Tasks.Read</span></span>    |
|<span data-ttu-id="6fb2e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fb2e-115">Application</span></span> | <span data-ttu-id="6fb2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fb2e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fb2e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fb2e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6fb2e-118">Optional query parameters</span></span>
<span data-ttu-id="6fb2e-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fb2e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fb2e-120">Request headers</span></span>
| <span data-ttu-id="6fb2e-121">名称</span><span class="sxs-lookup"><span data-stu-id="6fb2e-121">Name</span></span>      |<span data-ttu-id="6fb2e-122">说明</span><span class="sxs-lookup"><span data-stu-id="6fb2e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6fb2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fb2e-123">Authorization</span></span>  | <span data-ttu-id="6fb2e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fb2e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fb2e-126">Request body</span></span>
<span data-ttu-id="6fb2e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb2e-128">响应</span><span class="sxs-lookup"><span data-stu-id="6fb2e-128">Response</span></span>

<span data-ttu-id="6fb2e-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fb2e-130">示例</span><span class="sxs-lookup"><span data-stu-id="6fb2e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fb2e-131">请求</span><span class="sxs-lookup"><span data-stu-id="6fb2e-131">Request</span></span>
<span data-ttu-id="6fb2e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="6fb2e-133">响应</span><span class="sxs-lookup"><span data-stu-id="6fb2e-133">Response</span></span>
<span data-ttu-id="6fb2e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fb2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
