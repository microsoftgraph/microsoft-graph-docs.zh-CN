---
title: 列表 taskFolders
description: 获取特定 outlookTaskGroup Outlook 任务文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 66f755a994ea04a862051b6b32ce3ae9e6b39d0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857650"
---
# <a name="list-taskfolders"></a><span data-ttu-id="f084b-103">列表 taskFolders</span><span class="sxs-lookup"><span data-stu-id="f084b-103">List taskFolders</span></span>

> <span data-ttu-id="f084b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f084b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f084b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f084b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f084b-106">获取特定[outlookTaskGroup](../resources/outlooktaskgroup.md)Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="f084b-106">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f084b-107">权限</span><span class="sxs-lookup"><span data-stu-id="f084b-107">Permissions</span></span>
<span data-ttu-id="f084b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f084b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f084b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f084b-110">Permission type</span></span>      | <span data-ttu-id="f084b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f084b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f084b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f084b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f084b-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f084b-113">Tasks.Read</span></span>    |
|<span data-ttu-id="f084b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f084b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f084b-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f084b-115">Tasks.Read</span></span>    |
|<span data-ttu-id="f084b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f084b-116">Application</span></span> | <span data-ttu-id="f084b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f084b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f084b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f084b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f084b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f084b-119">Optional query parameters</span></span>
<span data-ttu-id="f084b-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f084b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f084b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f084b-121">Request headers</span></span>
| <span data-ttu-id="f084b-122">名称</span><span class="sxs-lookup"><span data-stu-id="f084b-122">Name</span></span>      |<span data-ttu-id="f084b-123">说明</span><span class="sxs-lookup"><span data-stu-id="f084b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f084b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f084b-124">Authorization</span></span>  | <span data-ttu-id="f084b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f084b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f084b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f084b-127">Request body</span></span>
<span data-ttu-id="f084b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f084b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f084b-129">响应</span><span class="sxs-lookup"><span data-stu-id="f084b-129">Response</span></span>

<span data-ttu-id="f084b-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f084b-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f084b-131">示例</span><span class="sxs-lookup"><span data-stu-id="f084b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f084b-132">请求</span><span class="sxs-lookup"><span data-stu-id="f084b-132">Request</span></span>
<span data-ttu-id="f084b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f084b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="f084b-134">响应</span><span class="sxs-lookup"><span data-stu-id="f084b-134">Response</span></span>
<span data-ttu-id="f084b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f084b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
    {
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
