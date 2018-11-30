---
title: 列出 directoryRole
description: 列出租户中激活的目录角色。
ms.openlocfilehash: ef43a0b016aadccd4a92a53672a18b7fe74ec154
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010407"
---
# <a name="list-directoryroles"></a><span data-ttu-id="1f00d-103">列出 directoryRole</span><span class="sxs-lookup"><span data-stu-id="1f00d-103">List directoryRoles</span></span>

<span data-ttu-id="1f00d-104">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="1f00d-104">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f00d-105">权限</span><span class="sxs-lookup"><span data-stu-id="1f00d-105">Permissions</span></span>
<span data-ttu-id="1f00d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f00d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f00d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f00d-108">Permission type</span></span>      | <span data-ttu-id="1f00d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f00d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f00d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f00d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f00d-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f00d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1f00d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f00d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f00d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f00d-113">Not supported.</span></span>    |
|<span data-ttu-id="1f00d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f00d-114">Application</span></span> | <span data-ttu-id="1f00d-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f00d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f00d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f00d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f00d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1f00d-117">Optional query parameters</span></span>
<span data-ttu-id="1f00d-118">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="1f00d-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f00d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f00d-119">Request headers</span></span>
| <span data-ttu-id="1f00d-120">名称</span><span class="sxs-lookup"><span data-stu-id="1f00d-120">Name</span></span>       | <span data-ttu-id="1f00d-121">类型</span><span class="sxs-lookup"><span data-stu-id="1f00d-121">Type</span></span> | <span data-ttu-id="1f00d-122">说明</span><span class="sxs-lookup"><span data-stu-id="1f00d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f00d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f00d-123">Authorization</span></span>  | <span data-ttu-id="1f00d-124">string</span><span class="sxs-lookup"><span data-stu-id="1f00d-124">string</span></span>  | <span data-ttu-id="1f00d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f00d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f00d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f00d-127">Request body</span></span>
<span data-ttu-id="1f00d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f00d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f00d-129">响应</span><span class="sxs-lookup"><span data-stu-id="1f00d-129">Response</span></span>

<span data-ttu-id="1f00d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1f00d-130">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f00d-131">示例</span><span class="sxs-lookup"><span data-stu-id="1f00d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f00d-132">请求</span><span class="sxs-lookup"><span data-stu-id="1f00d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="1f00d-133">响应</span><span class="sxs-lookup"><span data-stu-id="1f00d-133">Response</span></span>
<span data-ttu-id="1f00d-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f00d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
