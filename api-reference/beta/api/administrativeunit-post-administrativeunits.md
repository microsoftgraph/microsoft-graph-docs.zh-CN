---
title: 创建 administrativeUnit
description: 使用此 API 创建新 administrativeUnit。
author: lleonard-msft
ms.openlocfilehash: 320fe1b2269213d8fc4a0a8295f7ae84e0714cb1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351154"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="5aa96-103">创建 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="5aa96-103">Create administrativeUnit</span></span>

> <span data-ttu-id="5aa96-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5aa96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5aa96-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5aa96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5aa96-106">使用此 API 创建新[administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="5aa96-106">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5aa96-107">权限</span><span class="sxs-lookup"><span data-stu-id="5aa96-107">Permissions</span></span>
<span data-ttu-id="5aa96-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5aa96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5aa96-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5aa96-110">Permission type</span></span>      | <span data-ttu-id="5aa96-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5aa96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5aa96-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5aa96-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5aa96-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5aa96-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5aa96-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5aa96-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aa96-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5aa96-115">Not supported.</span></span>    |
|<span data-ttu-id="5aa96-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5aa96-116">Application</span></span> | <span data-ttu-id="5aa96-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5aa96-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5aa96-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5aa96-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="5aa96-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5aa96-119">Request headers</span></span>
| <span data-ttu-id="5aa96-120">Name</span><span class="sxs-lookup"><span data-stu-id="5aa96-120">Name</span></span>      |<span data-ttu-id="5aa96-121">说明</span><span class="sxs-lookup"><span data-stu-id="5aa96-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5aa96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aa96-122">Authorization</span></span>  | <span data-ttu-id="5aa96-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5aa96-p103">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="5aa96-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5aa96-125">Request body</span></span>
<span data-ttu-id="5aa96-126">在请求正文中，提供[administrativeUnit](../resources/administrativeunit.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aa96-126">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="5aa96-127">由于**administrativeUnit**资源支持[扩展](/graph/extensibility-overview)，您可以使用`POST`操作并创建它时将使用您自己的数据的自定义属性添加到管理单元。</span><span class="sxs-lookup"><span data-stu-id="5aa96-127">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="5aa96-128">响应</span><span class="sxs-lookup"><span data-stu-id="5aa96-128">Response</span></span>

<span data-ttu-id="5aa96-129">如果成功，此方法返回`201 Created`响应正文中的响应代码和[administrativeUnit](../resources/administrativeunit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5aa96-129">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aa96-130">示例</span><span class="sxs-lookup"><span data-stu-id="5aa96-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5aa96-131">请求</span><span class="sxs-lookup"><span data-stu-id="5aa96-131">Request</span></span>
<span data-ttu-id="5aa96-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5aa96-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="5aa96-133">在请求正文中，提供[administrativeUnit](../resources/administrativeunit.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aa96-133">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5aa96-134">响应</span><span class="sxs-lookup"><span data-stu-id="5aa96-134">Response</span></span>
<span data-ttu-id="5aa96-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5aa96-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5aa96-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5aa96-138">See also</span></span>

- [<span data-ttu-id="5aa96-139">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5aa96-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5aa96-140">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5aa96-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->