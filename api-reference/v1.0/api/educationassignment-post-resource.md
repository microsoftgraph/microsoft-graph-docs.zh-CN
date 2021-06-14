---
title: 创建 educationAssignmentResource
description: 创建教育作业资源。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 20719f61e7b01c42bd6615ef2c0bb032fe8b5c36
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912288"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="0d945-103">创建 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="0d945-103">Create educationAssignmentResource</span></span>

<span data-ttu-id="0d945-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d945-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d945-105">创建工作 [分配资源](../resources/educationassignmentresource.md)。</span><span class="sxs-lookup"><span data-stu-id="0d945-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> 

<span data-ttu-id="0d945-106">每个资源都有一@odata.type 属性来指示要创建的资源类型。</span><span class="sxs-lookup"><span data-stu-id="0d945-106">Every resource has an @odata.type property to indicate which type of resource is being created.</span></span> 

[!IMPORTANT] 
<span data-ttu-id="0d945-107">Upload创建资源之前，将基于 `resourcesFolder` 文件的资源指定给工作分配。</span><span class="sxs-lookup"><span data-stu-id="0d945-107">Upload file-based resource to the assignments `resourcesFolder` before creating the resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0d945-108">权限</span><span class="sxs-lookup"><span data-stu-id="0d945-108">Permissions</span></span>
<span data-ttu-id="0d945-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d945-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d945-111">Permission type</span></span>      | <span data-ttu-id="0d945-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d945-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d945-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d945-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="0d945-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d945-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0d945-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d945-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0d945-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d945-116">Not supported.</span></span>  |
|<span data-ttu-id="0d945-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d945-117">Application</span></span> | <span data-ttu-id="0d945-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d945-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="0d945-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d945-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="0d945-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d945-120">Request headers</span></span>
| <span data-ttu-id="0d945-121">标头</span><span class="sxs-lookup"><span data-stu-id="0d945-121">Header</span></span>       | <span data-ttu-id="0d945-122">值</span><span class="sxs-lookup"><span data-stu-id="0d945-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d945-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d945-123">Authorization</span></span>  | <span data-ttu-id="0d945-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d945-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d945-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d945-126">Content-Type</span></span>  | <span data-ttu-id="0d945-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0d945-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d945-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d945-128">Request body</span></span>
<span data-ttu-id="0d945-129">在请求正文中，提供 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d945-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0d945-130">响应</span><span class="sxs-lookup"><span data-stu-id="0d945-130">Response</span></span>
<span data-ttu-id="0d945-131">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d945-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d945-132">示例</span><span class="sxs-lookup"><span data-stu-id="0d945-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d945-133">请求</span><span class="sxs-lookup"><span data-stu-id="0d945-133">Request</span></span>
<span data-ttu-id="0d945-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d945-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "educationLinkResource"
  }
}

```
<span data-ttu-id="0d945-135">在请求正文中，提供 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d945-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="0d945-136">响应</span><span class="sxs-lookup"><span data-stu-id="0d945-136">Response</span></span>
<span data-ttu-id="0d945-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d945-137">The following is an example of the response.</span></span> 

><span data-ttu-id="0d945-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0d945-138">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "response",
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


