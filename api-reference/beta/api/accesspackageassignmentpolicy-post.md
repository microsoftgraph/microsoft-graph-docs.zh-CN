---
title: 创建 accessPackageAssignmentPolicy
description: 使用此 API 创建新的 accessPackageAssignmentPolicy。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 280a532c2d0047fecb0085f88b73c92c30a4867f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935249"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="7cc03-103">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="7cc03-103">Create accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cc03-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，使用此 API 创建新的[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7cc03-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), use this API to create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cc03-105">权限</span><span class="sxs-lookup"><span data-stu-id="7cc03-105">Permissions</span></span>

<span data-ttu-id="7cc03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cc03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7cc03-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cc03-108">Permission type</span></span>                        | <span data-ttu-id="7cc03-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cc03-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7cc03-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cc03-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7cc03-111">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="7cc03-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="7cc03-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cc03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cc03-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cc03-113">Not supported.</span></span> |
| <span data-ttu-id="7cc03-114">Application</span><span class="sxs-lookup"><span data-stu-id="7cc03-114">Application</span></span>                            | <span data-ttu-id="7cc03-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cc03-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cc03-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cc03-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7cc03-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cc03-117">Request headers</span></span>

| <span data-ttu-id="7cc03-118">名称</span><span class="sxs-lookup"><span data-stu-id="7cc03-118">Name</span></span>          | <span data-ttu-id="7cc03-119">说明</span><span class="sxs-lookup"><span data-stu-id="7cc03-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7cc03-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cc03-120">Authorization</span></span> | <span data-ttu-id="7cc03-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="7cc03-121">Bearer \{token\}.</span></span> <span data-ttu-id="7cc03-122">必填。</span><span class="sxs-lookup"><span data-stu-id="7cc03-122">Required.</span></span> |
| <span data-ttu-id="7cc03-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7cc03-123">Content-Type</span></span>  | <span data-ttu-id="7cc03-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7cc03-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7cc03-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cc03-125">Request body</span></span>

<span data-ttu-id="7cc03-126">在请求正文中，提供[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cc03-126">In the request body, supply a JSON representation of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7cc03-127">响应</span><span class="sxs-lookup"><span data-stu-id="7cc03-127">Response</span></span>

<span data-ttu-id="7cc03-128">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7cc03-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7cc03-129">示例</span><span class="sxs-lookup"><span data-stu-id="7cc03-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7cc03-130">请求</span><span class="sxs-lookup"><span data-stu-id="7cc03-130">Request</span></span>

<span data-ttu-id="7cc03-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7cc03-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="7cc03-132">响应</span><span class="sxs-lookup"><span data-stu-id="7cc03-132">Response</span></span>

<span data-ttu-id="7cc03-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7cc03-133">The following is an example of the response.</span></span>

> <span data-ttu-id="7cc03-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7cc03-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
