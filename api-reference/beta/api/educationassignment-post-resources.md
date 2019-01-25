---
title: 创建 educationAssignmentResource
description: 正在创建 odata.type 以指示哪种类型的资源。 请注意，必须首先将基于文件的资源上载到分配**资源**。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 34e8740336acbef056ec0b3703547de51fdc42ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527988"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="e1165-104">创建 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e1165-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1165-105">创建一个[工作分配资源](../resources/educationassignmentresource.md)。</span><span class="sxs-lookup"><span data-stu-id="e1165-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="e1165-106">该资源本身有 @odata.type 以指示要创建哪种类型的资源。</span><span class="sxs-lookup"><span data-stu-id="e1165-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="e1165-107">请注意，必须首先将基于文件的资源上载到分配**资源**。</span><span class="sxs-lookup"><span data-stu-id="e1165-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1165-108">权限</span><span class="sxs-lookup"><span data-stu-id="e1165-108">Permissions</span></span>
<span data-ttu-id="e1165-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1165-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1165-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1165-111">Permission type</span></span>      | <span data-ttu-id="e1165-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1165-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1165-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1165-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1165-114">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1165-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e1165-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1165-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e1165-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1165-116">Not supported.</span></span>  |
|<span data-ttu-id="e1165-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1165-117">Application</span></span> | <span data-ttu-id="e1165-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1165-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e1165-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1165-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="e1165-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1165-120">Request headers</span></span>
| <span data-ttu-id="e1165-121">标头</span><span class="sxs-lookup"><span data-stu-id="e1165-121">Header</span></span>       | <span data-ttu-id="e1165-122">值</span><span class="sxs-lookup"><span data-stu-id="e1165-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1165-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1165-123">Authorization</span></span>  | <span data-ttu-id="e1165-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1165-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1165-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1165-126">Content-Type</span></span>  | <span data-ttu-id="e1165-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e1165-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1165-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1165-128">Request body</span></span>
<span data-ttu-id="e1165-129">在请求正文中，提供[educationAssignmentResource](../resources/educationassignmentresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1165-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e1165-130">响应</span><span class="sxs-lookup"><span data-stu-id="e1165-130">Response</span></span>
<span data-ttu-id="e1165-131">如果成功，此方法返回`201 Created`响应代码和响应正文中的[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1165-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1165-132">示例</span><span class="sxs-lookup"><span data-stu-id="e1165-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1165-133">请求</span><span class="sxs-lookup"><span data-stu-id="e1165-133">Request</span></span>
<span data-ttu-id="e1165-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1165-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<span data-ttu-id="e1165-135">在请求正文中，提供[educationAssignmentResource](../resources/educationassignmentresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1165-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e1165-136">响应</span><span class="sxs-lookup"><span data-stu-id="e1165-136">Response</span></span>
<span data-ttu-id="e1165-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1165-137">The following is an example of the response.</span></span> 

><span data-ttu-id="e1165-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e1165-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e1165-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1165-139">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 229

{
  "id": "122333",
  "distributeForStudentWork": false,
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-post-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
