---
title: 列出 identityUserFlowAttributes
description: 检索 identityUserFlowAttribute 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c5a6aa380f1f8dfea25de5d15fb29e04ec3e0e9c
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742359"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="68a4b-103">列出 identityUserFlowAttributes</span><span class="sxs-lookup"><span data-stu-id="68a4b-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="68a4b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68a4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68a4b-105">检索 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="68a4b-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="68a4b-106">权限</span><span class="sxs-lookup"><span data-stu-id="68a4b-106">Permissions</span></span>

<span data-ttu-id="68a4b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68a4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68a4b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="68a4b-109">Permission type</span></span>      | <span data-ttu-id="68a4b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68a4b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68a4b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68a4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68a4b-112">IdentityUserFlow、IdentityUserflow 和所有</span><span class="sxs-lookup"><span data-stu-id="68a4b-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="68a4b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68a4b-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="68a4b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="68a4b-114">Not supported.</span></span>|
|<span data-ttu-id="68a4b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="68a4b-115">Application</span></span>|<span data-ttu-id="68a4b-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="68a4b-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="68a4b-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="68a4b-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="68a4b-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="68a4b-118">Global administrator</span></span>
* <span data-ttu-id="68a4b-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="68a4b-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="68a4b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68a4b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="68a4b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="68a4b-121">Request headers</span></span>

|<span data-ttu-id="68a4b-122">名称</span><span class="sxs-lookup"><span data-stu-id="68a4b-122">Name</span></span>|<span data-ttu-id="68a4b-123">说明</span><span class="sxs-lookup"><span data-stu-id="68a4b-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="68a4b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="68a4b-124">Authorization</span></span>|<span data-ttu-id="68a4b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68a4b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68a4b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="68a4b-127">Request body</span></span>

<span data-ttu-id="68a4b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68a4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68a4b-129">响应</span><span class="sxs-lookup"><span data-stu-id="68a4b-129">Response</span></span>

<span data-ttu-id="68a4b-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  对象集合。</span><span class="sxs-lookup"><span data-stu-id="68a4b-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68a4b-131">示例</span><span class="sxs-lookup"><span data-stu-id="68a4b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="68a4b-132">请求</span><span class="sxs-lookup"><span data-stu-id="68a4b-132">Request</span></span>

<span data-ttu-id="68a4b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="68a4b-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes
```

### <a name="response"></a><span data-ttu-id="68a4b-134">响应</span><span class="sxs-lookup"><span data-stu-id="68a4b-134">Response</span></span>

<span data-ttu-id="68a4b-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="68a4b-135">The following is an example of the response.</span></span>

<span data-ttu-id="68a4b-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="68a4b-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
