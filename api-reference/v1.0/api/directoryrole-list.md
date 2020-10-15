---
title: 列出 directoryRoles
description: 列出租户中激活的目录角色。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e2919c242bb8ee50387daac2f3ce52f1e58018f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458589"
---
# <a name="list-directoryroles"></a><span data-ttu-id="cec94-103">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="cec94-103">List directoryRoles</span></span>

<span data-ttu-id="cec94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cec94-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cec94-105">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="cec94-105">List the directory roles that are activated in the tenant.</span></span>

<span data-ttu-id="cec94-106">此操作仅返回已激活的角色。</span><span class="sxs-lookup"><span data-stu-id="cec94-106">This operation only returns roles that have been activated.</span></span> <span data-ttu-id="cec94-107">当管理员使用 [激活 directoryRole](directoryrole-post-directoryroles.md) API 激活角色时，角色即被激活。</span><span class="sxs-lookup"><span data-stu-id="cec94-107">A role becomes activated when an admin activates the role using the [Activate directoryRole](directoryrole-post-directoryroles.md) API.</span></span> <span data-ttu-id="cec94-108">最初并不激活所有内置角色。</span><span class="sxs-lookup"><span data-stu-id="cec94-108">Not all built-in roles are initially activated.</span></span> 

<span data-ttu-id="cec94-109">使用 Azure 门户分配角色时，将代表管理员隐式完成角色激活步骤。</span><span class="sxs-lookup"><span data-stu-id="cec94-109">When assigning a role using the Azure portal, the role activation step is implicitly done on the admin's behalf.</span></span> <span data-ttu-id="cec94-110">若要获取 Azure AD 中可用角色的完整列表，请使用 [List directoryroletemplate](directoryroletemplate-list.md)。</span><span class="sxs-lookup"><span data-stu-id="cec94-110">To get the full list of roles that are available in Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cec94-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="cec94-111">Permissions</span></span>
<span data-ttu-id="cec94-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cec94-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cec94-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="cec94-114">Permission type</span></span>      | <span data-ttu-id="cec94-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cec94-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cec94-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cec94-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cec94-117">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="cec94-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cec94-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cec94-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cec94-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cec94-119">Not supported.</span></span>    |
|<span data-ttu-id="cec94-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="cec94-120">Application</span></span> | <span data-ttu-id="cec94-121">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="cec94-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cec94-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cec94-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cec94-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cec94-123">Optional query parameters</span></span>
<span data-ttu-id="cec94-124">此方法**不**支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="cec94-124">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cec94-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="cec94-125">Request headers</span></span>
| <span data-ttu-id="cec94-126">名称</span><span class="sxs-lookup"><span data-stu-id="cec94-126">Name</span></span>       | <span data-ttu-id="cec94-127">说明</span><span class="sxs-lookup"><span data-stu-id="cec94-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cec94-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cec94-128">Authorization</span></span>  | <span data-ttu-id="cec94-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cec94-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cec94-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="cec94-131">Request body</span></span>
<span data-ttu-id="cec94-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cec94-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cec94-133">响应</span><span class="sxs-lookup"><span data-stu-id="cec94-133">Response</span></span>

<span data-ttu-id="cec94-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [directoryRole](../resources/directoryrole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cec94-134">If successful, this method returns a `200 OK` response code and a collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cec94-135">示例</span><span class="sxs-lookup"><span data-stu-id="cec94-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cec94-136">请求</span><span class="sxs-lookup"><span data-stu-id="cec94-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cec94-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cec94-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="cec94-138">C#</span><span class="sxs-lookup"><span data-stu-id="cec94-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cec94-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cec94-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cec94-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cec94-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cec94-141">Java</span><span class="sxs-lookup"><span data-stu-id="cec94-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cec94-142">响应</span><span class="sxs-lookup"><span data-stu-id="cec94-142">Response</span></span>
<span data-ttu-id="cec94-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cec94-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
