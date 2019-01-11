---
title: 更新 nameditem
description: 更新 nameditem 对象的属性。
localization_priority: Normal
ms.openlocfilehash: 59919e030d06e4c84242396d61c68d601433cc7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838708"
---
# <a name="update-nameditem"></a><span data-ttu-id="7d41f-103">更新 nameditem</span><span class="sxs-lookup"><span data-stu-id="7d41f-103">Update nameditem</span></span>

<span data-ttu-id="7d41f-104">更新 nameditem 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7d41f-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d41f-105">权限</span><span class="sxs-lookup"><span data-stu-id="7d41f-105">Permissions</span></span>
<span data-ttu-id="7d41f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d41f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d41f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d41f-108">Permission type</span></span>      | <span data-ttu-id="7d41f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d41f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d41f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d41f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d41f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d41f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d41f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d41f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d41f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d41f-113">Not supported.</span></span>    |
|<span data-ttu-id="7d41f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d41f-114">Application</span></span> | <span data-ttu-id="7d41f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d41f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d41f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d41f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7d41f-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="7d41f-117">Optional request headers</span></span>
| <span data-ttu-id="7d41f-118">名称</span><span class="sxs-lookup"><span data-stu-id="7d41f-118">Name</span></span>       | <span data-ttu-id="7d41f-119">说明</span><span class="sxs-lookup"><span data-stu-id="7d41f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7d41f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d41f-120">Authorization</span></span>  | <span data-ttu-id="7d41f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d41f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d41f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d41f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d41f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7d41f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d41f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d41f-126">Request body</span></span>
<span data-ttu-id="7d41f-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7d41f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7d41f-130">属性</span><span class="sxs-lookup"><span data-stu-id="7d41f-130">Property</span></span>     | <span data-ttu-id="7d41f-131">类型</span><span class="sxs-lookup"><span data-stu-id="7d41f-131">Type</span></span>   |<span data-ttu-id="7d41f-132">说明</span><span class="sxs-lookup"><span data-stu-id="7d41f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d41f-133">visible</span><span class="sxs-lookup"><span data-stu-id="7d41f-133">visible</span></span>|<span data-ttu-id="7d41f-134">boolean</span><span class="sxs-lookup"><span data-stu-id="7d41f-134">boolean</span></span>|<span data-ttu-id="7d41f-135">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="7d41f-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="7d41f-136">comment</span><span class="sxs-lookup"><span data-stu-id="7d41f-136">comment</span></span>|   <span data-ttu-id="7d41f-137">string</span><span class="sxs-lookup"><span data-stu-id="7d41f-137">string</span></span>  |<span data-ttu-id="7d41f-138">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="7d41f-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="7d41f-139">响应</span><span class="sxs-lookup"><span data-stu-id="7d41f-139">Response</span></span>

<span data-ttu-id="7d41f-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[WorkbookNamedItem](../resources/nameditem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7d41f-140">If successful, this method returns a `200 OK` response code and updated [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d41f-141">示例</span><span class="sxs-lookup"><span data-stu-id="7d41f-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d41f-142">请求</span><span class="sxs-lookup"><span data-stu-id="7d41f-142">Request</span></span>
<span data-ttu-id="7d41f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d41f-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="7d41f-144">响应</span><span class="sxs-lookup"><span data-stu-id="7d41f-144">Response</span></span>
<span data-ttu-id="7d41f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7d41f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
