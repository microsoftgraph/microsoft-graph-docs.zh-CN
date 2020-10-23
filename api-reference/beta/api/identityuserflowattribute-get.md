---
title: 获取 identityUserFlowAttribute
description: 检索 identityUserFlowAttribute 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8d1d60a318ebe3962af0077b367b334d37420a4
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742348"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="3f564-103">获取 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="3f564-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="3f564-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f564-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f564-105">检索 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f564-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f564-106">权限</span><span class="sxs-lookup"><span data-stu-id="3f564-106">Permissions</span></span>

<span data-ttu-id="3f564-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f564-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f564-109">Permission type</span></span>      | <span data-ttu-id="3f564-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f564-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f564-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f564-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f564-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="3f564-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3f564-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f564-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3f564-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f564-114">Not supported.</span></span>|
|<span data-ttu-id="3f564-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f564-115">Application</span></span>|<span data-ttu-id="3f564-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="3f564-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3f564-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="3f564-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3f564-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3f564-118">Global administrator</span></span>
* <span data-ttu-id="3f564-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="3f564-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3f564-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f564-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3f564-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f564-121">Request headers</span></span>

|<span data-ttu-id="3f564-122">名称</span><span class="sxs-lookup"><span data-stu-id="3f564-122">Name</span></span>|<span data-ttu-id="3f564-123">说明</span><span class="sxs-lookup"><span data-stu-id="3f564-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3f564-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f564-124">Authorization</span></span>|<span data-ttu-id="3f564-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f564-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f564-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f564-127">Request body</span></span>

<span data-ttu-id="3f564-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f564-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f564-129">响应</span><span class="sxs-lookup"><span data-stu-id="3f564-129">Response</span></span>

<span data-ttu-id="3f564-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [IDENTITYUSERFLOWATTRIBUTE](../resources/identityuserflowattribute.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f564-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f564-131">示例</span><span class="sxs-lookup"><span data-stu-id="3f564-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3f564-132">请求</span><span class="sxs-lookup"><span data-stu-id="3f564-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```

### <a name="response"></a><span data-ttu-id="3f564-133">响应</span><span class="sxs-lookup"><span data-stu-id="3f564-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "City",
    "displayName": "City",
    "description": "Your city",
    "userFlowAttributeType": "builtIn",
    "dataType": "string"
}
```
