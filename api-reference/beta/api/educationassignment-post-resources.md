---
title: 创建 educationAssignmentResource
description: 创建教育作业资源。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3ca73c7b078520f5f25b0948b8a41f272ba73669
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911891"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="730a0-103">创建 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="730a0-103">Create educationAssignmentResource</span></span>

<span data-ttu-id="730a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="730a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="730a0-105">创建工作 [分配资源](../resources/educationassignmentresource.md)。</span><span class="sxs-lookup"><span data-stu-id="730a0-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="730a0-106">资源本身具有 @odata.type，用于指示要创建的资源类型。</span><span class="sxs-lookup"><span data-stu-id="730a0-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="730a0-107">请注意，必须先将基于文件的资源上载到工作分配 **resourceFolder**。</span><span class="sxs-lookup"><span data-stu-id="730a0-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="730a0-108">权限</span><span class="sxs-lookup"><span data-stu-id="730a0-108">Permissions</span></span>
<span data-ttu-id="730a0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="730a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="730a0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="730a0-111">Permission type</span></span>      | <span data-ttu-id="730a0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="730a0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="730a0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="730a0-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="730a0-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="730a0-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="730a0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="730a0-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="730a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="730a0-116">Not supported.</span></span>  |
|<span data-ttu-id="730a0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="730a0-117">Application</span></span> | <span data-ttu-id="730a0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="730a0-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="730a0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="730a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="730a0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="730a0-120">Request headers</span></span>
| <span data-ttu-id="730a0-121">标头</span><span class="sxs-lookup"><span data-stu-id="730a0-121">Header</span></span>       | <span data-ttu-id="730a0-122">值</span><span class="sxs-lookup"><span data-stu-id="730a0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="730a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="730a0-123">Authorization</span></span>  | <span data-ttu-id="730a0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="730a0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="730a0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="730a0-126">Content-Type</span></span>  | <span data-ttu-id="730a0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="730a0-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="730a0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="730a0-128">Request body</span></span>
<span data-ttu-id="730a0-129">在请求正文中，提供 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="730a0-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="730a0-130">响应</span><span class="sxs-lookup"><span data-stu-id="730a0-130">Response</span></span>
<span data-ttu-id="730a0-131">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="730a0-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="730a0-132">示例</span><span class="sxs-lookup"><span data-stu-id="730a0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="730a0-133">请求</span><span class="sxs-lookup"><span data-stu-id="730a0-133">Request</span></span>
<span data-ttu-id="730a0-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="730a0-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="730a0-135">在请求正文中，提供 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="730a0-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="730a0-136">响应</span><span class="sxs-lookup"><span data-stu-id="730a0-136">Response</span></span>
<span data-ttu-id="730a0-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="730a0-137">The following is an example of the response.</span></span> 

><span data-ttu-id="730a0-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="730a0-138">**Note:** The response object shown here might be shortened for readability.</span></span>


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


