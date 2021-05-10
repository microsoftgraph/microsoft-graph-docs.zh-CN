---
title: 列出 effectiveRules
description: 从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ce8a5889cb395c18f5995746f406507ade5e4d7
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299152"
---
# <a name="list-effectiverules"></a><span data-ttu-id="b52a6-103">列出 effectiveRules</span><span class="sxs-lookup"><span data-stu-id="b52a6-103">List effectiveRules</span></span>
<span data-ttu-id="b52a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b52a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b52a6-105">从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。</span><span class="sxs-lookup"><span data-stu-id="b52a6-105">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b52a6-106">权限</span><span class="sxs-lookup"><span data-stu-id="b52a6-106">Permissions</span></span>
<span data-ttu-id="b52a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b52a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52a6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b52a6-109">Permission type</span></span>|<span data-ttu-id="b52a6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b52a6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b52a6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b52a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b52a6-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b52a6-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="b52a6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b52a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b52a6-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b52a6-114">Not supported</span></span>|
|<span data-ttu-id="b52a6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b52a6-115">Application</span></span>|<span data-ttu-id="b52a6-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b52a6-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="b52a6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b52a6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b52a6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b52a6-118">Optional query parameters</span></span>
<span data-ttu-id="b52a6-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b52a6-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b52a6-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b52a6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b52a6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b52a6-121">Request headers</span></span>
|<span data-ttu-id="b52a6-122">名称</span><span class="sxs-lookup"><span data-stu-id="b52a6-122">Name</span></span>|<span data-ttu-id="b52a6-123">说明</span><span class="sxs-lookup"><span data-stu-id="b52a6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b52a6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b52a6-124">Authorization</span></span>|<span data-ttu-id="b52a6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b52a6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b52a6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b52a6-127">Request body</span></span>
<span data-ttu-id="b52a6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b52a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b52a6-129">响应</span><span class="sxs-lookup"><span data-stu-id="b52a6-129">Response</span></span>

<span data-ttu-id="b52a6-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b52a6-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b52a6-131">示例</span><span class="sxs-lookup"><span data-stu-id="b52a6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b52a6-132">请求</span><span class="sxs-lookup"><span data-stu-id="b52a6-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/effectiveRules
```


### <a name="response"></a><span data-ttu-id="b52a6-133">响应</span><span class="sxs-lookup"><span data-stu-id="b52a6-133">Response</span></span>
<span data-ttu-id="b52a6-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b52a6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyRule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
      "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
      }
    }
  ]
}
```

