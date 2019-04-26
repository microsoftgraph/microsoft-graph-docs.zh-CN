---
title: 获取 servicePrincipal
description: 检索 serviceprincipal 对象的属性和关系。
localization_priority: Priority
ms.openlocfilehash: 785249d6fa6e1cc6239832bcd8d6b95c99381c7b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335974"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="f27a2-103">获取 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="f27a2-103">Get servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f27a2-104">检索 serviceprincipal 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f27a2-104">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f27a2-105">权限</span><span class="sxs-lookup"><span data-stu-id="f27a2-105">Permissions</span></span>
<span data-ttu-id="f27a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f27a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f27a2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f27a2-108">Permission type</span></span>      | <span data-ttu-id="f27a2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f27a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f27a2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f27a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f27a2-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f27a2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f27a2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f27a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f27a2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f27a2-113">Not supported.</span></span>    |
|<span data-ttu-id="f27a2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f27a2-114">Application</span></span> | <span data-ttu-id="f27a2-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f27a2-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f27a2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f27a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f27a2-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f27a2-117">Optional query parameters</span></span>
<span data-ttu-id="f27a2-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f27a2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f27a2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f27a2-119">Request headers</span></span>
| <span data-ttu-id="f27a2-120">名称</span><span class="sxs-lookup"><span data-stu-id="f27a2-120">Name</span></span>       | <span data-ttu-id="f27a2-121">类型</span><span class="sxs-lookup"><span data-stu-id="f27a2-121">Type</span></span> | <span data-ttu-id="f27a2-122">说明</span><span class="sxs-lookup"><span data-stu-id="f27a2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f27a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f27a2-123">Authorization</span></span>  | <span data-ttu-id="f27a2-124">string</span><span class="sxs-lookup"><span data-stu-id="f27a2-124">string</span></span>  | <span data-ttu-id="f27a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f27a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f27a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f27a2-127">Request body</span></span>
<span data-ttu-id="f27a2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f27a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f27a2-129">响应</span><span class="sxs-lookup"><span data-stu-id="f27a2-129">Response</span></span>

<span data-ttu-id="f27a2-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f27a2-130">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f27a2-131">示例</span><span class="sxs-lookup"><span data-stu-id="f27a2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f27a2-132">请求</span><span class="sxs-lookup"><span data-stu-id="f27a2-132">Request</span></span>
<span data-ttu-id="f27a2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f27a2-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="f27a2-134">响应</span><span class="sxs-lookup"><span data-stu-id="f27a2-134">Response</span></span>
<span data-ttu-id="f27a2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f27a2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
