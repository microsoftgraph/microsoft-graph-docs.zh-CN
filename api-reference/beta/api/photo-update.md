---
title: 更新照片
description: 更新 photo 对象的属性。
ms.openlocfilehash: 8071c9e331f9af72c9a288239206f396d9ad3fcb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041752"
---
# <a name="update-photo"></a><span data-ttu-id="ddc1b-103">更新照片</span><span class="sxs-lookup"><span data-stu-id="ddc1b-103">Update photo</span></span>

> <span data-ttu-id="ddc1b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddc1b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddc1b-106">更新 photo 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-106">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ddc1b-107">权限</span><span class="sxs-lookup"><span data-stu-id="ddc1b-107">Permissions</span></span>
<span data-ttu-id="ddc1b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc1b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddc1b-110">Permission type</span></span>      | <span data-ttu-id="ddc1b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddc1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddc1b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddc1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ddc1b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-113">Not supported.</span></span>    |
|<span data-ttu-id="ddc1b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddc1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddc1b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-115">Not supported.</span></span>    |
|<span data-ttu-id="ddc1b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddc1b-116">Application</span></span> | <span data-ttu-id="ddc1b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddc1b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddc1b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="ddc1b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddc1b-119">Request headers</span></span>
| <span data-ttu-id="ddc1b-120">名称</span><span class="sxs-lookup"><span data-stu-id="ddc1b-120">Name</span></span>       | <span data-ttu-id="ddc1b-121">类型</span><span class="sxs-lookup"><span data-stu-id="ddc1b-121">Type</span></span> | <span data-ttu-id="ddc1b-122">说明</span><span class="sxs-lookup"><span data-stu-id="ddc1b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddc1b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddc1b-123">Authorization</span></span>  | <span data-ttu-id="ddc1b-124">string</span><span class="sxs-lookup"><span data-stu-id="ddc1b-124">string</span></span>  | <span data-ttu-id="ddc1b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddc1b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddc1b-127">Request body</span></span>
<span data-ttu-id="ddc1b-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ddc1b-131">属性</span><span class="sxs-lookup"><span data-stu-id="ddc1b-131">Property</span></span>     | <span data-ttu-id="ddc1b-132">类型</span><span class="sxs-lookup"><span data-stu-id="ddc1b-132">Type</span></span>   |<span data-ttu-id="ddc1b-133">说明</span><span class="sxs-lookup"><span data-stu-id="ddc1b-133">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="ddc1b-134">响应</span><span class="sxs-lookup"><span data-stu-id="ddc1b-134">Response</span></span>

<span data-ttu-id="ddc1b-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-135">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ddc1b-136">示例</span><span class="sxs-lookup"><span data-stu-id="ddc1b-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddc1b-137">请求</span><span class="sxs-lookup"><span data-stu-id="ddc1b-137">Request</span></span>
<span data-ttu-id="ddc1b-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="ddc1b-139">响应</span><span class="sxs-lookup"><span data-stu-id="ddc1b-139">Response</span></span>
<span data-ttu-id="ddc1b-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ddc1b-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
