---
title: 删除 educationClass
description: 从学校删除课程。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 69e5bab04ac9c9c4d595eb40f76d379082806717
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815433"
---
# <a name="remove-educationclass"></a><span data-ttu-id="56837-103">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="56837-103">Remove educationClass</span></span>

<span data-ttu-id="56837-104">从学校删除课程。</span><span class="sxs-lookup"><span data-stu-id="56837-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="56837-105">权限</span><span class="sxs-lookup"><span data-stu-id="56837-105">Permissions</span></span>
<span data-ttu-id="56837-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56837-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="56837-108">Permission type</span></span>      | <span data-ttu-id="56837-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56837-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56837-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56837-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="56837-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="56837-111">Not supported.</span></span>  |
|<span data-ttu-id="56837-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56837-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="56837-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="56837-113">Not supported.</span></span>  |
|<span data-ttu-id="56837-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="56837-114">Application</span></span> | <span data-ttu-id="56837-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56837-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="56837-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56837-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="56837-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="56837-117">Request headers</span></span>
| <span data-ttu-id="56837-118">标头</span><span class="sxs-lookup"><span data-stu-id="56837-118">Header</span></span>       | <span data-ttu-id="56837-119">值</span><span class="sxs-lookup"><span data-stu-id="56837-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56837-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="56837-120">Authorization</span></span>  | <span data-ttu-id="56837-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56837-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56837-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="56837-123">Request body</span></span>
<span data-ttu-id="56837-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56837-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="56837-125">响应</span><span class="sxs-lookup"><span data-stu-id="56837-125">Response</span></span>
<span data-ttu-id="56837-126">如果成功，此方法将返回 `204 No Content` 响应代码和响应正文。</span><span class="sxs-lookup"><span data-stu-id="56837-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="56837-127">示例</span><span class="sxs-lookup"><span data-stu-id="56837-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56837-128">请求</span><span class="sxs-lookup"><span data-stu-id="56837-128">Request</span></span>
<span data-ttu-id="56837-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56837-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="56837-130">响应</span><span class="sxs-lookup"><span data-stu-id="56837-130">Response</span></span>
<span data-ttu-id="56837-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56837-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
