---
title: 获取 connectedOrganization
description: 检索 connectedorganization 对象的属性和关系。
author: markwahl-msft
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: a5dbf59c2202076749948b8f908d4f3b18937fce
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510001"
---
# <a name="get-connectedorganization"></a><span data-ttu-id="f85ab-103">获取 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="f85ab-103">Get connectedOrganization</span></span>

<span data-ttu-id="f85ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f85ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f85ab-105">检索[connectedOrganization](../resources/connectedorganization.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f85ab-105">Retrieve the properties and relationships of a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f85ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="f85ab-106">Permissions</span></span>

<span data-ttu-id="f85ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f85ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f85ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f85ab-109">Permission type</span></span>|<span data-ttu-id="f85ab-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f85ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="f85ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f85ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f85ab-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="f85ab-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f85ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f85ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f85ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f85ab-114">Not supported.</span></span> |
| <span data-ttu-id="f85ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f85ab-115">Application</span></span>                            | <span data-ttu-id="f85ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f85ab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f85ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f85ab-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f85ab-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f85ab-118">Optional query parameters</span></span>

<span data-ttu-id="f85ab-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f85ab-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f85ab-120">例如，若要仅检索标识源，请添加 `$select=identitySources` 。</span><span class="sxs-lookup"><span data-stu-id="f85ab-120">For example, to retrieve only the identity sources, add `$select=identitySources`.</span></span> <span data-ttu-id="f85ab-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f85ab-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f85ab-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f85ab-122">Request headers</span></span>

|<span data-ttu-id="f85ab-123">名称</span><span class="sxs-lookup"><span data-stu-id="f85ab-123">Name</span></span>|<span data-ttu-id="f85ab-124">说明</span><span class="sxs-lookup"><span data-stu-id="f85ab-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f85ab-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f85ab-125">Authorization</span></span>|<span data-ttu-id="f85ab-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f85ab-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f85ab-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f85ab-128">Request body</span></span>

<span data-ttu-id="f85ab-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f85ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f85ab-130">响应</span><span class="sxs-lookup"><span data-stu-id="f85ab-130">Response</span></span>

<span data-ttu-id="f85ab-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[connectedOrganization](../resources/connectedorganization.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f85ab-131">If successful, this method returns a `200 OK` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f85ab-132">示例</span><span class="sxs-lookup"><span data-stu-id="f85ab-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f85ab-133">请求</span><span class="sxs-lookup"><span data-stu-id="f85ab-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectedorganization"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

### <a name="response"></a><span data-ttu-id="f85ab-134">响应</span><span class="sxs-lookup"><span data-stu-id="f85ab-134">Response</span></span>

<span data-ttu-id="f85ab-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f85ab-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f",
  "displayName": "Wingtip Toys",
  "description": "Wingtip Toys",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-05-13T15:18:04.81Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-05-13T15:18:04.81Z",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "bf85dc9d-cb43-44a4-80c4-469e8c58249e",
      "displayName": "Wingtip Toys Co"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
