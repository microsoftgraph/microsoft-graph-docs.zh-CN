---
title: 将 educationRubric 附加到 educationAssignment
description: 将现有的 educationRubric 对象附加到 educationAssignment。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 50d3cdd61578cb2ae2474a7b58220caf2b94463b
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173186"
---
# <a name="create-educationrubric"></a><span data-ttu-id="ad72b-103">创建 educationRubric</span><span class="sxs-lookup"><span data-stu-id="ad72b-103">Create educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad72b-104">将现有的[educationRubric](../resources/educationrubric.md)对象附加到[educationAssignment](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="ad72b-104">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad72b-105">权限</span><span class="sxs-lookup"><span data-stu-id="ad72b-105">Permissions</span></span>

<span data-ttu-id="ad72b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad72b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad72b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad72b-108">Permission type</span></span>                        | <span data-ttu-id="ad72b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad72b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ad72b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad72b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad72b-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="ad72b-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="ad72b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad72b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad72b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad72b-113">Not supported.</span></span> |
| <span data-ttu-id="ad72b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad72b-114">Application</span></span>                            | <span data-ttu-id="ad72b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad72b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad72b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad72b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ad72b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad72b-117">Request headers</span></span>

| <span data-ttu-id="ad72b-118">名称</span><span class="sxs-lookup"><span data-stu-id="ad72b-118">Name</span></span>          | <span data-ttu-id="ad72b-119">说明</span><span class="sxs-lookup"><span data-stu-id="ad72b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ad72b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad72b-120">Authorization</span></span> | <span data-ttu-id="ad72b-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ad72b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad72b-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad72b-122">Request body</span></span>

<span data-ttu-id="ad72b-123">在请求正文中, 提供现有[educationRubric](../resources/educationrubric.md)对象的 OData ID。</span><span class="sxs-lookup"><span data-stu-id="ad72b-123">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ad72b-124">响应</span><span class="sxs-lookup"><span data-stu-id="ad72b-124">Response</span></span>

<span data-ttu-id="ad72b-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ad72b-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad72b-127">示例</span><span class="sxs-lookup"><span data-stu-id="ad72b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad72b-128">请求</span><span class="sxs-lookup"><span data-stu-id="ad72b-128">Request</span></span>

<span data-ttu-id="ad72b-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ad72b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationassignment"
}-->

```http
PUT https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
}
```

### <a name="response"></a><span data-ttu-id="ad72b-130">响应</span><span class="sxs-lookup"><span data-stu-id="ad72b-130">Response</span></span>

<span data-ttu-id="ad72b-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ad72b-131">The following is an example of the response.</span></span>

> <span data-ttu-id="ad72b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad72b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
