---
title: 创建 educationAssignmentResource
description: odata.type，指示要创建的资源类型。 请注意，必须先将基于文件的资源上载到工作分配 **resourceFolder**。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8001af1c46ee374d47c9235f67080f87af74b4bc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044254"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="fd6af-104">创建 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="fd6af-104">Create educationAssignmentResource</span></span>

<span data-ttu-id="fd6af-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd6af-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd6af-106">创建工作 [分配资源](../resources/educationassignmentresource.md)。</span><span class="sxs-lookup"><span data-stu-id="fd6af-106">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="fd6af-107">资源本身具有 @odata.type，用于指示要创建的资源类型。</span><span class="sxs-lookup"><span data-stu-id="fd6af-107">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="fd6af-108">请注意，必须先将基于文件的资源上载到工作分配 **resourceFolder**。</span><span class="sxs-lookup"><span data-stu-id="fd6af-108">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd6af-109">权限</span><span class="sxs-lookup"><span data-stu-id="fd6af-109">Permissions</span></span>
<span data-ttu-id="fd6af-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd6af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd6af-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd6af-112">Permission type</span></span>      | <span data-ttu-id="fd6af-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd6af-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd6af-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd6af-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="fd6af-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd6af-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="fd6af-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd6af-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fd6af-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd6af-117">Not supported.</span></span>  |
|<span data-ttu-id="fd6af-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd6af-118">Application</span></span> | <span data-ttu-id="fd6af-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd6af-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fd6af-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd6af-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="fd6af-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd6af-121">Request headers</span></span>
| <span data-ttu-id="fd6af-122">标头</span><span class="sxs-lookup"><span data-stu-id="fd6af-122">Header</span></span>       | <span data-ttu-id="fd6af-123">值</span><span class="sxs-lookup"><span data-stu-id="fd6af-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd6af-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd6af-124">Authorization</span></span>  | <span data-ttu-id="fd6af-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd6af-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd6af-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd6af-127">Content-Type</span></span>  | <span data-ttu-id="fd6af-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fd6af-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd6af-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd6af-129">Request body</span></span>
<span data-ttu-id="fd6af-130">在请求正文中，提供 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd6af-130">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="fd6af-131">响应</span><span class="sxs-lookup"><span data-stu-id="fd6af-131">Response</span></span>
<span data-ttu-id="fd6af-132">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd6af-132">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd6af-133">示例</span><span class="sxs-lookup"><span data-stu-id="fd6af-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd6af-134">请求</span><span class="sxs-lookup"><span data-stu-id="fd6af-134">Request</span></span>
<span data-ttu-id="fd6af-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fd6af-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="fd6af-136">在请求正文中，提供 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd6af-136">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fd6af-137">响应</span><span class="sxs-lookup"><span data-stu-id="fd6af-137">Response</span></span>
<span data-ttu-id="fd6af-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fd6af-138">The following is an example of the response.</span></span> 

><span data-ttu-id="fd6af-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fd6af-139">**Note:** The response object shown here might be shortened for readability.</span></span>


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


