---
title: 列出 taskFolders
description: 获取特定 outlookTaskGroup 中的 Outlook 任务文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3e7898f60068e6db0219911847d43faaf1894b5b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337836"
---
# <a name="list-taskfolders"></a><span data-ttu-id="f6ae9-103">列出 taskFolders</span><span class="sxs-lookup"><span data-stu-id="f6ae9-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6ae9-104">获取特定[outlookTaskGroup](../resources/outlooktaskgroup.md)中的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f6ae9-105">权限</span><span class="sxs-lookup"><span data-stu-id="f6ae9-105">Permissions</span></span>
<span data-ttu-id="f6ae9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ae9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6ae9-108">Permission type</span></span>      | <span data-ttu-id="f6ae9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6ae9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6ae9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6ae9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6ae9-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f6ae9-111">Tasks.Read</span></span>    |
|<span data-ttu-id="f6ae9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6ae9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6ae9-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f6ae9-113">Tasks.Read</span></span>    |
|<span data-ttu-id="f6ae9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6ae9-114">Application</span></span> | <span data-ttu-id="f6ae9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6ae9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6ae9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6ae9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f6ae9-117">Optional query parameters</span></span>
<span data-ttu-id="f6ae9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6ae9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6ae9-119">Request headers</span></span>
| <span data-ttu-id="f6ae9-120">名称</span><span class="sxs-lookup"><span data-stu-id="f6ae9-120">Name</span></span>      |<span data-ttu-id="f6ae9-121">说明</span><span class="sxs-lookup"><span data-stu-id="f6ae9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6ae9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6ae9-122">Authorization</span></span>  | <span data-ttu-id="f6ae9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6ae9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6ae9-125">Request body</span></span>
<span data-ttu-id="f6ae9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6ae9-127">响应</span><span class="sxs-lookup"><span data-stu-id="f6ae9-127">Response</span></span>

<span data-ttu-id="f6ae9-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6ae9-129">示例</span><span class="sxs-lookup"><span data-stu-id="f6ae9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6ae9-130">请求</span><span class="sxs-lookup"><span data-stu-id="f6ae9-130">Request</span></span>
<span data-ttu-id="f6ae9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
##### <a name="response"></a><span data-ttu-id="f6ae9-132">响应</span><span class="sxs-lookup"><span data-stu-id="f6ae9-132">Response</span></span>
<span data-ttu-id="f6ae9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6ae9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
