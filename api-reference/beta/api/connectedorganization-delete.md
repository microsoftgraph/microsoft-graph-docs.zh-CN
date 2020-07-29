---
title: 删除 connectedOrganization
description: 删除 connectedOrganization。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f91652b8f7ec479892c6f19d9804b39b521fe58
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510005"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="1b3ef-103">删除 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="1b3ef-103">Delete connectedOrganization</span></span>

<span data-ttu-id="1b3ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b3ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b3ef-105">删除[connectedOrganization](../resources/connectedorganization.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b3ef-106">权限</span><span class="sxs-lookup"><span data-stu-id="1b3ef-106">Permissions</span></span>

<span data-ttu-id="1b3ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b3ef-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b3ef-109">Permission type</span></span>|<span data-ttu-id="1b3ef-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1b3ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="1b3ef-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b3ef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b3ef-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b3ef-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1b3ef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b3ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b3ef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-114">Not supported.</span></span> |
| <span data-ttu-id="1b3ef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b3ef-115">Application</span></span>                            | <span data-ttu-id="1b3ef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b3ef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b3ef-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1b3ef-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b3ef-118">Request headers</span></span>
|<span data-ttu-id="1b3ef-119">名称</span><span class="sxs-lookup"><span data-stu-id="1b3ef-119">Name</span></span>|<span data-ttu-id="1b3ef-120">说明</span><span class="sxs-lookup"><span data-stu-id="1b3ef-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b3ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b3ef-121">Authorization</span></span>|<span data-ttu-id="1b3ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b3ef-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b3ef-124">Request body</span></span>
<span data-ttu-id="1b3ef-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b3ef-126">响应</span><span class="sxs-lookup"><span data-stu-id="1b3ef-126">Response</span></span>

<span data-ttu-id="1b3ef-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1b3ef-128">示例</span><span class="sxs-lookup"><span data-stu-id="1b3ef-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b3ef-129">请求</span><span class="sxs-lookup"><span data-stu-id="1b3ef-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```


### <a name="response"></a><span data-ttu-id="1b3ef-130">响应</span><span class="sxs-lookup"><span data-stu-id="1b3ef-130">Response</span></span>
<span data-ttu-id="1b3ef-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b3ef-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
