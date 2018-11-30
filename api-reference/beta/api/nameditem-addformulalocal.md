---
title: 添加已命名项 FormulaLocal
description: 使用用户的公式区域设置，将新名称添加到给定范围的集合。
ms.openlocfilehash: 931a6b928678802cc6bc60c42e4df73d09833ed4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043713"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="d5adb-103">添加已命名项 FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="d5adb-103">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="d5adb-104">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="d5adb-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5adb-105">权限</span><span class="sxs-lookup"><span data-stu-id="d5adb-105">Permissions</span></span>
<span data-ttu-id="d5adb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5adb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5adb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5adb-108">Permission type</span></span>      | <span data-ttu-id="d5adb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5adb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5adb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5adb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5adb-111">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5adb-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="d5adb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5adb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5adb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5adb-113">Not supported.</span></span>    |
|<span data-ttu-id="d5adb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5adb-114">Application</span></span> | <span data-ttu-id="d5adb-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5adb-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5adb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5adb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="d5adb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5adb-117">Request headers</span></span>
| <span data-ttu-id="d5adb-118">名称</span><span class="sxs-lookup"><span data-stu-id="d5adb-118">Name</span></span>       | <span data-ttu-id="d5adb-119">说明</span><span class="sxs-lookup"><span data-stu-id="d5adb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5adb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5adb-120">Authorization</span></span>  | <span data-ttu-id="d5adb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5adb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5adb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d5adb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d5adb-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d5adb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5adb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5adb-126">Request body</span></span>
<span data-ttu-id="d5adb-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d5adb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5adb-128">参数</span><span class="sxs-lookup"><span data-stu-id="d5adb-128">Parameter</span></span>    | <span data-ttu-id="d5adb-129">类型</span><span class="sxs-lookup"><span data-stu-id="d5adb-129">Type</span></span>   |<span data-ttu-id="d5adb-130">说明</span><span class="sxs-lookup"><span data-stu-id="d5adb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5adb-131">name</span><span class="sxs-lookup"><span data-stu-id="d5adb-131">name</span></span>|<span data-ttu-id="d5adb-132">string</span><span class="sxs-lookup"><span data-stu-id="d5adb-132">string</span></span>|<span data-ttu-id="d5adb-133">已命名项的名称。</span><span class="sxs-lookup"><span data-stu-id="d5adb-133">The name of the named item.</span></span>|
|<span data-ttu-id="d5adb-134">公式</span><span class="sxs-lookup"><span data-stu-id="d5adb-134">formula</span></span>|<span data-ttu-id="d5adb-135">字符串</span><span class="sxs-lookup"><span data-stu-id="d5adb-135">string</span></span>|<span data-ttu-id="d5adb-136">名称将引用的公式或区域。</span><span class="sxs-lookup"><span data-stu-id="d5adb-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="d5adb-137">comment</span><span class="sxs-lookup"><span data-stu-id="d5adb-137">comment</span></span>|<span data-ttu-id="d5adb-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d5adb-138">string</span></span>|<span data-ttu-id="d5adb-139">与此已命名项相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="d5adb-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="d5adb-140">响应</span><span class="sxs-lookup"><span data-stu-id="d5adb-140">Response</span></span>

<span data-ttu-id="d5adb-141">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [NamedItem](../resources/nameditem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5adb-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5adb-142">示例</span><span class="sxs-lookup"><span data-stu-id="d5adb-142">Example</span></span>
<span data-ttu-id="d5adb-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d5adb-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d5adb-144">请求</span><span class="sxs-lookup"><span data-stu-id="d5adb-144">Request</span></span>
<span data-ttu-id="d5adb-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5adb-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="d5adb-146">响应</span><span class="sxs-lookup"><span data-stu-id="d5adb-146">Response</span></span>
<span data-ttu-id="d5adb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5adb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
