---
title: 创建 activityBasedTimeoutPolicy
description: 创建新的 activityBasedTimeoutPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b0c9227b363f4f3693fe56e057f66a51498b3fb5
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227797"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="90465-103">创建 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="90465-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="90465-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90465-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="90465-105">创建新的[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90465-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90465-106">权限</span><span class="sxs-lookup"><span data-stu-id="90465-106">Permissions</span></span>

<span data-ttu-id="90465-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90465-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90465-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90465-109">Permission type</span></span>                        | <span data-ttu-id="90465-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90465-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90465-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90465-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90465-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="90465-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="90465-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90465-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90465-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90465-114">Not supported.</span></span> |
| <span data-ttu-id="90465-115">Application</span><span class="sxs-lookup"><span data-stu-id="90465-115">Application</span></span>                            | <span data-ttu-id="90465-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="90465-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="90465-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90465-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="90465-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="90465-118">Request headers</span></span>

| <span data-ttu-id="90465-119">名称</span><span class="sxs-lookup"><span data-stu-id="90465-119">Name</span></span>          | <span data-ttu-id="90465-120">说明</span><span class="sxs-lookup"><span data-stu-id="90465-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="90465-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90465-121">Authorization</span></span> | <span data-ttu-id="90465-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90465-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90465-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="90465-124">Content-type</span></span> | <span data-ttu-id="90465-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="90465-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90465-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="90465-127">Request body</span></span>

<span data-ttu-id="90465-128">在请求正文中，提供[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90465-128">In the request body, supply a JSON representation of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="90465-129">响应</span><span class="sxs-lookup"><span data-stu-id="90465-129">Response</span></span>

<span data-ttu-id="90465-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90465-130">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90465-131">示例</span><span class="sxs-lookup"><span data-stu-id="90465-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90465-132">请求</span><span class="sxs-lookup"><span data-stu-id="90465-132">Request</span></span>

<span data-ttu-id="90465-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="90465-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="90465-134">响应</span><span class="sxs-lookup"><span data-stu-id="90465-134">Response</span></span>

<span data-ttu-id="90465-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="90465-135">The following is an example of the response.</span></span>

> <span data-ttu-id="90465-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="90465-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
