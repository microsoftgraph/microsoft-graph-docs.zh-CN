---
title: 创建 delegatedPermissionClassification
description: 通过将 delegatedPermissionClassification 添加到 API 的服务主体来对权限进行分类。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 22512ad7a61d528d22535156c1ac882b73950f72
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377211"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="471e1-103">创建 delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="471e1-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="471e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="471e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="471e1-105">通过将 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 添加到代表 API 的 [servicePrincipal](../resources/servicePrincipal.md) 来对委派权限进行分类。</span><span class="sxs-lookup"><span data-stu-id="471e1-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="471e1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="471e1-106">Permissions</span></span>

<span data-ttu-id="471e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="471e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="471e1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="471e1-109">Permission type</span></span>      | <span data-ttu-id="471e1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="471e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="471e1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="471e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="471e1-112">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="471e1-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="471e1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="471e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="471e1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="471e1-114">Not supported.</span></span>    |
|<span data-ttu-id="471e1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="471e1-115">Application</span></span> | <span data-ttu-id="471e1-116">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="471e1-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="471e1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="471e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="471e1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="471e1-118">Request headers</span></span>

| <span data-ttu-id="471e1-119">名称</span><span class="sxs-lookup"><span data-stu-id="471e1-119">Name</span></span>       | <span data-ttu-id="471e1-120">说明</span><span class="sxs-lookup"><span data-stu-id="471e1-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="471e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="471e1-121">Authorization</span></span> | <span data-ttu-id="471e1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="471e1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="471e1-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="471e1-124">Content-type</span></span> | <span data-ttu-id="471e1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="471e1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="471e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="471e1-127">Request body</span></span>

<span data-ttu-id="471e1-128">在请求正文中，提供 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="471e1-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="471e1-129">响应</span><span class="sxs-lookup"><span data-stu-id="471e1-129">Response</span></span>

<span data-ttu-id="471e1-130">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="471e1-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="471e1-131">示例</span><span class="sxs-lookup"><span data-stu-id="471e1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="471e1-132">请求</span><span class="sxs-lookup"><span data-stu-id="471e1-132">Request</span></span>

<span data-ttu-id="471e1-133">在以下示例中，委派权限 "User. Read" 被分类为 "low"。</span><span class="sxs-lookup"><span data-stu-id="471e1-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```

### <a name="response"></a><span data-ttu-id="471e1-134">响应</span><span class="sxs-lookup"><span data-stu-id="471e1-134">Response</span></span>

<span data-ttu-id="471e1-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="471e1-135">The following is an example of the response.</span></span>

> <span data-ttu-id="471e1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="471e1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
