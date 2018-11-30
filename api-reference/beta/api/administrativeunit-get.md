---
title: Get administrativeUnit
description: 检索的属性和 administrativeUnit 对象的关系。
ms.openlocfilehash: d6e19762a74883da3dcff1d8ea423dc06192dd46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042986"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="14817-103">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="14817-103">Get administrativeUnit</span></span>

> <span data-ttu-id="14817-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="14817-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14817-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="14817-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14817-106">检索的属性和[administrativeUnit](../resources/administrativeunit.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="14817-106">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="14817-107">由于**administrativeUnit**资源支持[扩展](/graph/extensibility-overview)，您还可以使用`GET`操作来获取**administrativeUnit**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="14817-107">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="14817-108">权限</span><span class="sxs-lookup"><span data-stu-id="14817-108">Permissions</span></span>
<span data-ttu-id="14817-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14817-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="14817-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="14817-111">Permission type</span></span>      | <span data-ttu-id="14817-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14817-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14817-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14817-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14817-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14817-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14817-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14817-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14817-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14817-116">Not supported.</span></span>    |
|<span data-ttu-id="14817-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="14817-117">Application</span></span> | <span data-ttu-id="14817-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14817-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14817-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14817-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14817-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14817-120">Optional query parameters</span></span>
<span data-ttu-id="14817-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="14817-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14817-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="14817-122">Request headers</span></span>
| <span data-ttu-id="14817-123">名称</span><span class="sxs-lookup"><span data-stu-id="14817-123">Name</span></span>      |<span data-ttu-id="14817-124">说明</span><span class="sxs-lookup"><span data-stu-id="14817-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14817-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="14817-125">Authorization</span></span>  | <span data-ttu-id="14817-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14817-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14817-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="14817-128">Request body</span></span>
<span data-ttu-id="14817-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14817-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14817-130">响应</span><span class="sxs-lookup"><span data-stu-id="14817-130">Response</span></span>

<span data-ttu-id="14817-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[administrativeUnit](../resources/administrativeunit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14817-131">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14817-132">示例</span><span class="sxs-lookup"><span data-stu-id="14817-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14817-133">请求</span><span class="sxs-lookup"><span data-stu-id="14817-133">Request</span></span>
<span data-ttu-id="14817-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14817-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="14817-135">响应</span><span class="sxs-lookup"><span data-stu-id="14817-135">Response</span></span>
<span data-ttu-id="14817-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14817-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="14817-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="14817-139">See also</span></span>

- [<span data-ttu-id="14817-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="14817-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="14817-141">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="14817-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->