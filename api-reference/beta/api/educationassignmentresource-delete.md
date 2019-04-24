---
title: 删除 educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0a6ac6f4cddde9d80e48080b0f54b2610e84782c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457919"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="c6450-103">删除 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="c6450-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6450-104">从工作分配中删除资源。</span><span class="sxs-lookup"><span data-stu-id="c6450-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="c6450-105">只有课堂中的教师才能删除资源。</span><span class="sxs-lookup"><span data-stu-id="c6450-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="c6450-106">向学生发布分配后, 教师将无法删除标记为 "distributeToStudents" 的资源。</span><span class="sxs-lookup"><span data-stu-id="c6450-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="c6450-107">权限</span><span class="sxs-lookup"><span data-stu-id="c6450-107">Permissions</span></span>
<span data-ttu-id="c6450-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6450-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6450-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6450-110">Permission type</span></span>      | <span data-ttu-id="c6450-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6450-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6450-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6450-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c6450-113">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="c6450-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c6450-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6450-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c6450-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6450-115">Not supported.</span></span>  |
|<span data-ttu-id="c6450-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6450-116">Application</span></span> | <span data-ttu-id="c6450-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6450-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c6450-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6450-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c6450-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6450-119">Request headers</span></span>
| <span data-ttu-id="c6450-120">标头</span><span class="sxs-lookup"><span data-stu-id="c6450-120">Header</span></span>       | <span data-ttu-id="c6450-121">值</span><span class="sxs-lookup"><span data-stu-id="c6450-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6450-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6450-122">Authorization</span></span>  | <span data-ttu-id="c6450-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6450-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6450-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6450-125">Request body</span></span>
<span data-ttu-id="c6450-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6450-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c6450-127">响应</span><span class="sxs-lookup"><span data-stu-id="c6450-127">Response</span></span>
<span data-ttu-id="c6450-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c6450-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6450-130">示例</span><span class="sxs-lookup"><span data-stu-id="c6450-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6450-131">请求</span><span class="sxs-lookup"><span data-stu-id="c6450-131">Request</span></span>
<span data-ttu-id="c6450-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6450-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="c6450-133">响应</span><span class="sxs-lookup"><span data-stu-id="c6450-133">Response</span></span>
<span data-ttu-id="c6450-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c6450-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
