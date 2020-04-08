---
title: 更新 unifiedRoleAssignmentMultiple
description: 更新新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e6901065e07fc286ace312b1ad558ba4e7e6a882
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181316"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="eff92-103">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="eff92-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="eff92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eff92-105">更新现有的[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eff92-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="eff92-106">使用此项可在 Microsoft Intune 中更新角色分配。</span><span class="sxs-lookup"><span data-stu-id="eff92-106">Use this to update role assignments in Microsoft Intune.</span></span> <span data-ttu-id="eff92-107">请注意， [unifiedRoleAssignment](../resources/unifiedroleassignment.md)不支持 update。</span><span class="sxs-lookup"><span data-stu-id="eff92-107">Note that [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="eff92-108">权限</span><span class="sxs-lookup"><span data-stu-id="eff92-108">Permissions</span></span>

<span data-ttu-id="eff92-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eff92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eff92-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eff92-111">Permission type</span></span> | <span data-ttu-id="eff92-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eff92-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="eff92-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eff92-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eff92-114">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="eff92-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="eff92-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eff92-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eff92-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eff92-116">Not supported.</span></span> |
| <span data-ttu-id="eff92-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eff92-117">Application</span></span> | <span data-ttu-id="eff92-118">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="eff92-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="eff92-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eff92-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="eff92-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eff92-120">Request headers</span></span>

| <span data-ttu-id="eff92-121">名称</span><span class="sxs-lookup"><span data-stu-id="eff92-121">Name</span></span> | <span data-ttu-id="eff92-122">说明</span><span class="sxs-lookup"><span data-stu-id="eff92-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="eff92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eff92-123">Authorization</span></span> | <span data-ttu-id="eff92-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eff92-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eff92-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="eff92-126">Content-type</span></span> | <span data-ttu-id="eff92-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="eff92-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eff92-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="eff92-129">Request body</span></span>

<span data-ttu-id="eff92-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="eff92-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="eff92-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="eff92-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eff92-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="eff92-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="eff92-133">响应</span><span class="sxs-lookup"><span data-stu-id="eff92-133">Response</span></span>

<span data-ttu-id="eff92-134">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eff92-134">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eff92-135">示例</span><span class="sxs-lookup"><span data-stu-id="eff92-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="eff92-136">请求</span><span class="sxs-lookup"><span data-stu-id="eff92-136">Request</span></span>

<span data-ttu-id="eff92-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eff92-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eff92-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="eff92-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
Content-type: application/json

{ 
    "principalIds": ["0aeec2c1-fee7-4e02-b534-6f920d25b300", "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"]
}
```
# <a name="c"></a>[<span data-ttu-id="eff92-139">C#</span><span class="sxs-lookup"><span data-stu-id="eff92-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eff92-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eff92-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eff92-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eff92-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eff92-142">响应</span><span class="sxs-lookup"><span data-stu-id="eff92-142">Response</span></span>

<span data-ttu-id="eff92-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eff92-143">The following is an example of the response.</span></span>
> <span data-ttu-id="eff92-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eff92-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 204 OK

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
