---
title: 创建 educationAssignmentResource
description: 正在创建 odata.type 以指示哪种类型的资源。 请注意，必须首先将基于文件的资源上载到分配**资源**。
localization_priority: Normal
ms.openlocfilehash: 206e7db8c8e96f230bc0062fa9b080831b1b4e1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854010"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="fde0c-104">创建 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="fde0c-104">Create educationAssignmentResource</span></span>

> <span data-ttu-id="fde0c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fde0c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fde0c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fde0c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fde0c-107">创建一个[工作分配资源](../resources/educationassignmentresource.md)。</span><span class="sxs-lookup"><span data-stu-id="fde0c-107">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="fde0c-108">该资源本身有 @odata.type 以指示要创建哪种类型的资源。</span><span class="sxs-lookup"><span data-stu-id="fde0c-108">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="fde0c-109">请注意，必须首先将基于文件的资源上载到分配**资源**。</span><span class="sxs-lookup"><span data-stu-id="fde0c-109">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="fde0c-110">权限</span><span class="sxs-lookup"><span data-stu-id="fde0c-110">Permissions</span></span>
<span data-ttu-id="fde0c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fde0c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fde0c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="fde0c-113">Permission type</span></span>      | <span data-ttu-id="fde0c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fde0c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fde0c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fde0c-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="fde0c-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fde0c-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="fde0c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fde0c-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fde0c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fde0c-118">Not supported.</span></span>  |
|<span data-ttu-id="fde0c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="fde0c-119">Application</span></span> | <span data-ttu-id="fde0c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="fde0c-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fde0c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fde0c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="fde0c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fde0c-122">Request headers</span></span>
| <span data-ttu-id="fde0c-123">标头</span><span class="sxs-lookup"><span data-stu-id="fde0c-123">Header</span></span>       | <span data-ttu-id="fde0c-124">值</span><span class="sxs-lookup"><span data-stu-id="fde0c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fde0c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fde0c-125">Authorization</span></span>  | <span data-ttu-id="fde0c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fde0c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fde0c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fde0c-128">Content-Type</span></span>  | <span data-ttu-id="fde0c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fde0c-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fde0c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fde0c-130">Request body</span></span>
<span data-ttu-id="fde0c-131">在请求正文中，提供[educationAssignmentResource](../resources/educationassignmentresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fde0c-131">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="fde0c-132">响应</span><span class="sxs-lookup"><span data-stu-id="fde0c-132">Response</span></span>
<span data-ttu-id="fde0c-133">如果成功，此方法返回`201 Created`响应代码和响应正文中的[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fde0c-133">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fde0c-134">示例</span><span class="sxs-lookup"><span data-stu-id="fde0c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fde0c-135">请求</span><span class="sxs-lookup"><span data-stu-id="fde0c-135">Request</span></span>
<span data-ttu-id="fde0c-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fde0c-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="fde0c-137">在请求正文中，提供[educationAssignmentResource](../resources/educationassignmentresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fde0c-137">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fde0c-138">响应</span><span class="sxs-lookup"><span data-stu-id="fde0c-138">Response</span></span>
<span data-ttu-id="fde0c-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fde0c-139">The following is an example of the response.</span></span> 

><span data-ttu-id="fde0c-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fde0c-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fde0c-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fde0c-141">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
