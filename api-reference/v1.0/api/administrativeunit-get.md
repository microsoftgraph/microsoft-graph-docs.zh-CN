---
title: 获取 administrativeUnit
description: 检索 administrativeUnit 对象的属性和关系。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5329863a01eacaebd0d356a99b47d6db690df19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020233"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="3e38b-103">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="3e38b-103">Get administrativeUnit</span></span>

<span data-ttu-id="3e38b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e38b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e38b-105">检索 [administrativeUnit](../resources/administrativeunit.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e38b-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="3e38b-106">权限</span><span class="sxs-lookup"><span data-stu-id="3e38b-106">Permissions</span></span>
<span data-ttu-id="3e38b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e38b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3e38b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e38b-109">Permission type</span></span>      | <span data-ttu-id="3e38b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e38b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e38b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e38b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e38b-112">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="3e38b-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e38b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e38b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e38b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e38b-114">Not supported.</span></span>    |
|<span data-ttu-id="3e38b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e38b-115">Application</span></span> | <span data-ttu-id="3e38b-116">AdministrativeUnit、AdministrativeUnit、all、all、all、All 和所有的</span><span class="sxs-lookup"><span data-stu-id="3e38b-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e38b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e38b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e38b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3e38b-118">Optional query parameters</span></span>
<span data-ttu-id="3e38b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3e38b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e38b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e38b-120">Request headers</span></span>
| <span data-ttu-id="3e38b-121">名称</span><span class="sxs-lookup"><span data-stu-id="3e38b-121">Name</span></span>      |<span data-ttu-id="3e38b-122">说明</span><span class="sxs-lookup"><span data-stu-id="3e38b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e38b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e38b-123">Authorization</span></span>  | <span data-ttu-id="3e38b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e38b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e38b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e38b-126">Request body</span></span>
<span data-ttu-id="3e38b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e38b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e38b-128">响应</span><span class="sxs-lookup"><span data-stu-id="3e38b-128">Response</span></span>

<span data-ttu-id="3e38b-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e38b-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e38b-130">示例</span><span class="sxs-lookup"><span data-stu-id="3e38b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e38b-131">请求</span><span class="sxs-lookup"><span data-stu-id="3e38b-131">Request</span></span>
<span data-ttu-id="3e38b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e38b-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
```

---

##### <a name="response"></a><span data-ttu-id="3e38b-133">响应</span><span class="sxs-lookup"><span data-stu-id="3e38b-133">Response</span></span>
<span data-ttu-id="3e38b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e38b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3e38b-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3e38b-137">See also</span></span>

- [<span data-ttu-id="3e38b-138">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3e38b-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3e38b-139">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="3e38b-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
