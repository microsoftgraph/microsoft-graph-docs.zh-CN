---
title: 列表 taskFolders
description: 获取特定 outlookTaskGroup Outlook 任务文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 16a3463a7cdc4a3bc4efd401c7ca1a8932c82b7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508284"
---
# <a name="list-taskfolders"></a><span data-ttu-id="263cd-103">列表 taskFolders</span><span class="sxs-lookup"><span data-stu-id="263cd-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="263cd-104">获取特定[outlookTaskGroup](../resources/outlooktaskgroup.md)Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="263cd-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="263cd-105">权限</span><span class="sxs-lookup"><span data-stu-id="263cd-105">Permissions</span></span>
<span data-ttu-id="263cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="263cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="263cd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="263cd-108">Permission type</span></span>      | <span data-ttu-id="263cd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="263cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="263cd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="263cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="263cd-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="263cd-111">Tasks.Read</span></span>    |
|<span data-ttu-id="263cd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="263cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="263cd-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="263cd-113">Tasks.Read</span></span>    |
|<span data-ttu-id="263cd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="263cd-114">Application</span></span> | <span data-ttu-id="263cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="263cd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="263cd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="263cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="263cd-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="263cd-117">Optional query parameters</span></span>
<span data-ttu-id="263cd-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="263cd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="263cd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="263cd-119">Request headers</span></span>
| <span data-ttu-id="263cd-120">名称</span><span class="sxs-lookup"><span data-stu-id="263cd-120">Name</span></span>      |<span data-ttu-id="263cd-121">说明</span><span class="sxs-lookup"><span data-stu-id="263cd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="263cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="263cd-122">Authorization</span></span>  | <span data-ttu-id="263cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="263cd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="263cd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="263cd-125">Request body</span></span>
<span data-ttu-id="263cd-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="263cd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="263cd-127">响应</span><span class="sxs-lookup"><span data-stu-id="263cd-127">Response</span></span>

<span data-ttu-id="263cd-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="263cd-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="263cd-129">示例</span><span class="sxs-lookup"><span data-stu-id="263cd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="263cd-130">请求</span><span class="sxs-lookup"><span data-stu-id="263cd-130">Request</span></span>
<span data-ttu-id="263cd-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="263cd-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="263cd-132">响应</span><span class="sxs-lookup"><span data-stu-id="263cd-132">Response</span></span>
<span data-ttu-id="263cd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="263cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-list-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
