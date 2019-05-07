---
title: 创建 administrativeUnit
description: 使用此 API 创建新的 administrativeUnit。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4815082a8a5930e426e0843d2dcf2ebe6ef190d5
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636630"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="90323-103">创建 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="90323-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90323-104">使用此 API 创建新的[administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="90323-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="90323-105">权限</span><span class="sxs-lookup"><span data-stu-id="90323-105">Permissions</span></span>
<span data-ttu-id="90323-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="90323-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="90323-108">Permission type</span></span>      | <span data-ttu-id="90323-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90323-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90323-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90323-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90323-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90323-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90323-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90323-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90323-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="90323-113">Not supported.</span></span>    |
|<span data-ttu-id="90323-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="90323-114">Application</span></span> | <span data-ttu-id="90323-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90323-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90323-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90323-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="90323-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="90323-117">Request headers</span></span>
| <span data-ttu-id="90323-118">名称</span><span class="sxs-lookup"><span data-stu-id="90323-118">Name</span></span>      |<span data-ttu-id="90323-119">说明</span><span class="sxs-lookup"><span data-stu-id="90323-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90323-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="90323-120">Authorization</span></span>  | <span data-ttu-id="90323-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90323-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="90323-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="90323-123">Request body</span></span>
<span data-ttu-id="90323-124">在请求正文中, 提供[administrativeUnit](../resources/administrativeunit.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90323-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="90323-125">由于**administrativeUnit**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用`POST`操作, 并在创建自定义属性时将自己的数据添加到管理单元中。</span><span class="sxs-lookup"><span data-stu-id="90323-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="90323-126">响应</span><span class="sxs-lookup"><span data-stu-id="90323-126">Response</span></span>

<span data-ttu-id="90323-127">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[administrativeUnit](../resources/administrativeunit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90323-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90323-128">示例</span><span class="sxs-lookup"><span data-stu-id="90323-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90323-129">请求</span><span class="sxs-lookup"><span data-stu-id="90323-129">Request</span></span>
<span data-ttu-id="90323-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90323-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true"
}
```
<span data-ttu-id="90323-131">在请求正文中, 提供[administrativeUnit](../resources/administrativeunit.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90323-131">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="90323-132">响应</span><span class="sxs-lookup"><span data-stu-id="90323-132">Response</span></span>
<span data-ttu-id="90323-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90323-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
  "administrativeUnit": {
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="90323-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="90323-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="90323-137">语言</span><span class="sxs-lookup"><span data-stu-id="90323-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90323-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="90323-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="90323-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="90323-139">See also</span></span>

- [<span data-ttu-id="90323-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="90323-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="90323-141">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="90323-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
