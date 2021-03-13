---
title: 创建 legalHold
description: 创建新的 legalHold 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a48774cd3613b2b2cdbcb376d5ffe9781a786c79
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773849"
---
# <a name="create-legalhold"></a><span data-ttu-id="10079-103">创建 legalHold</span><span class="sxs-lookup"><span data-stu-id="10079-103">Create legalHold</span></span>

<span data-ttu-id="10079-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="10079-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10079-105">创建新的 [legalHold](../resources/ediscovery-legalhold.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10079-105">Create a new [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10079-106">权限</span><span class="sxs-lookup"><span data-stu-id="10079-106">Permissions</span></span>

<span data-ttu-id="10079-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10079-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10079-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="10079-109">Permission type</span></span>|<span data-ttu-id="10079-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10079-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10079-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10079-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10079-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10079-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="10079-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10079-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10079-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="10079-114">Not supported.</span></span>|
|<span data-ttu-id="10079-115">Application</span><span class="sxs-lookup"><span data-stu-id="10079-115">Application</span></span>|<span data-ttu-id="10079-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10079-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10079-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10079-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds
```

## <a name="request-headers"></a><span data-ttu-id="10079-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="10079-118">Request headers</span></span>

|<span data-ttu-id="10079-119">名称</span><span class="sxs-lookup"><span data-stu-id="10079-119">Name</span></span>|<span data-ttu-id="10079-120">说明</span><span class="sxs-lookup"><span data-stu-id="10079-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="10079-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="10079-121">Authorization</span></span>|<span data-ttu-id="10079-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10079-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="10079-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10079-124">Content-Type</span></span>|<span data-ttu-id="10079-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="10079-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10079-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10079-127">Request body</span></span>

<span data-ttu-id="10079-128">在请求正文中，提供 [legalHold](../resources/ediscovery-legalhold.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10079-128">In the request body, supply a JSON representation of the [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

<span data-ttu-id="10079-129">下表显示创建 [legalHold](../resources/ediscovery-legalhold.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="10079-129">The following table shows the properties that are required when you create the [legalHold](../resources/ediscovery-legalhold.md).</span></span>

|<span data-ttu-id="10079-130">属性</span><span class="sxs-lookup"><span data-stu-id="10079-130">Property</span></span>|<span data-ttu-id="10079-131">类型</span><span class="sxs-lookup"><span data-stu-id="10079-131">Type</span></span>|<span data-ttu-id="10079-132">说明</span><span class="sxs-lookup"><span data-stu-id="10079-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10079-133">displayName</span><span class="sxs-lookup"><span data-stu-id="10079-133">displayName</span></span>|<span data-ttu-id="10079-134">字符串</span><span class="sxs-lookup"><span data-stu-id="10079-134">String</span></span>| <span data-ttu-id="10079-135">法定显示名称的保留项。</span><span class="sxs-lookup"><span data-stu-id="10079-135">The display name of the legal hold.</span></span> |

## <a name="response"></a><span data-ttu-id="10079-136">响应</span><span class="sxs-lookup"><span data-stu-id="10079-136">Response</span></span>

<span data-ttu-id="10079-137">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10079-137">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10079-138">示例</span><span class="sxs-lookup"><span data-stu-id="10079-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10079-139">请求</span><span class="sxs-lookup"><span data-stu-id="10079-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="10079-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="10079-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_legalhold_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds
Content-Type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="10079-141">C#</span><span class="sxs-lookup"><span data-stu-id="10079-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-legalhold-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10079-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10079-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-legalhold-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10079-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10079-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-legalhold-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10079-144">Java</span><span class="sxs-lookup"><span data-stu-id="10079-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-legalhold-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10079-145">响应</span><span class="sxs-lookup"><span data-stu-id="10079-145">Response</span></span>

<span data-ttu-id="10079-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="10079-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "700cd868-d868-700c-68d8-0c7068d80c70",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
