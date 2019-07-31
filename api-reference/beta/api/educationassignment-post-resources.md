---
title: 创建 educationAssignmentResource
description: odata。键入以指示要创建的资源的类型。 请注意, 必须首先将基于文件的资源上载到工作分配**resourceFolder**。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 86cf738f7558814a76d07e7a7eb5ffd22d988d29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955653"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="ae4db-104">创建 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="ae4db-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae4db-105">创建[工作分配资源](../resources/educationassignmentresource.md)。</span><span class="sxs-lookup"><span data-stu-id="ae4db-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="ae4db-106">资源本身有一个 @odata。若要指示正在创建的资源的类型, 请键入。</span><span class="sxs-lookup"><span data-stu-id="ae4db-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="ae4db-107">请注意, 必须首先将基于文件的资源上载到工作分配**resourceFolder**。</span><span class="sxs-lookup"><span data-stu-id="ae4db-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae4db-108">权限</span><span class="sxs-lookup"><span data-stu-id="ae4db-108">Permissions</span></span>
<span data-ttu-id="ae4db-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae4db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae4db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae4db-111">Permission type</span></span>      | <span data-ttu-id="ae4db-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae4db-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae4db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae4db-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="ae4db-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="ae4db-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ae4db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae4db-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ae4db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae4db-116">Not supported.</span></span>  |
|<span data-ttu-id="ae4db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae4db-117">Application</span></span> | <span data-ttu-id="ae4db-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae4db-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ae4db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae4db-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="ae4db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae4db-120">Request headers</span></span>
| <span data-ttu-id="ae4db-121">标头</span><span class="sxs-lookup"><span data-stu-id="ae4db-121">Header</span></span>       | <span data-ttu-id="ae4db-122">值</span><span class="sxs-lookup"><span data-stu-id="ae4db-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae4db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae4db-123">Authorization</span></span>  | <span data-ttu-id="ae4db-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae4db-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae4db-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae4db-126">Content-Type</span></span>  | <span data-ttu-id="ae4db-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ae4db-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae4db-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae4db-128">Request body</span></span>
<span data-ttu-id="ae4db-129">在请求正文中, 提供[educationAssignmentResource](../resources/educationassignmentresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae4db-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ae4db-130">响应</span><span class="sxs-lookup"><span data-stu-id="ae4db-130">Response</span></span>
<span data-ttu-id="ae4db-131">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ae4db-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae4db-132">示例</span><span class="sxs-lookup"><span data-stu-id="ae4db-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae4db-133">请求</span><span class="sxs-lookup"><span data-stu-id="ae4db-133">Request</span></span>
<span data-ttu-id="ae4db-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae4db-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="ae4db-135">在请求正文中, 提供[educationAssignmentResource](../resources/educationassignmentresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae4db-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ae4db-136">响应</span><span class="sxs-lookup"><span data-stu-id="ae4db-136">Response</span></span>
<span data-ttu-id="ae4db-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ae4db-137">The following is an example of the response.</span></span> 

><span data-ttu-id="ae4db-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ae4db-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ae4db-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae4db-139">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": []
}
-->
