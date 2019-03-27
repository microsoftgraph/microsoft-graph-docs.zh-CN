---
title: 获取 outlookTaskFolder
description: 获取指定的 Outlook 任务文件夹的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 70ef38ce8b3d808bb66064f69353ef4f2ed0fb5b
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869412"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="4b6f6-103">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4b6f6-103">Get outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b6f6-104">获取指定的 Outlook 任务文件夹的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-104">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b6f6-105">权限</span><span class="sxs-lookup"><span data-stu-id="4b6f6-105">Permissions</span></span>
<span data-ttu-id="4b6f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b6f6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b6f6-108">Permission type</span></span>      | <span data-ttu-id="4b6f6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b6f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b6f6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b6f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b6f6-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="4b6f6-111">Tasks.Read</span></span>    |
|<span data-ttu-id="4b6f6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b6f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b6f6-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="4b6f6-113">Tasks.Read</span></span>    |
|<span data-ttu-id="4b6f6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b6f6-114">Application</span></span> | <span data-ttu-id="4b6f6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b6f6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b6f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b6f6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b6f6-117">Optional query parameters</span></span>
<span data-ttu-id="4b6f6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b6f6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b6f6-119">Request headers</span></span>
| <span data-ttu-id="4b6f6-120">名称</span><span class="sxs-lookup"><span data-stu-id="4b6f6-120">Name</span></span>      |<span data-ttu-id="4b6f6-121">说明</span><span class="sxs-lookup"><span data-stu-id="4b6f6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b6f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b6f6-122">Authorization</span></span>  | <span data-ttu-id="4b6f6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b6f6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b6f6-125">Request body</span></span>
<span data-ttu-id="4b6f6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b6f6-127">响应</span><span class="sxs-lookup"><span data-stu-id="4b6f6-127">Response</span></span>

<span data-ttu-id="4b6f6-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-128">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b6f6-129">示例</span><span class="sxs-lookup"><span data-stu-id="4b6f6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b6f6-130">请求</span><span class="sxs-lookup"><span data-stu-id="4b6f6-130">Request</span></span>
<span data-ttu-id="4b6f6-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAAABrJAAA=')
```
##### <a name="response"></a><span data-ttu-id="4b6f6-132">响应</span><span class="sxs-lookup"><span data-stu-id="4b6f6-132">Response</span></span>
<span data-ttu-id="4b6f6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b6f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
