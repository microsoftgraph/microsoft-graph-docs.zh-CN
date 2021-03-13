---
title: 创建 legalHold userSource
description: 创建新的 legalHold userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 266ea3603050f34ad77003b9052189abba56baaa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772974"
---
# <a name="create-legalhold-usersource"></a><span data-ttu-id="450f1-103">创建 legalHold userSource</span><span class="sxs-lookup"><span data-stu-id="450f1-103">Create legalHold userSource</span></span>

<span data-ttu-id="450f1-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="450f1-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="450f1-105">将 userSource 添加到 legalHold 对象。</span><span class="sxs-lookup"><span data-stu-id="450f1-105">Adds a userSource to a legalHold object.</span></span>

## <a name="permissions"></a><span data-ttu-id="450f1-106">权限</span><span class="sxs-lookup"><span data-stu-id="450f1-106">Permissions</span></span>

<span data-ttu-id="450f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="450f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="450f1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="450f1-109">Permission type</span></span>|<span data-ttu-id="450f1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="450f1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="450f1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="450f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="450f1-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="450f1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="450f1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="450f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="450f1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="450f1-114">Not supported.</span></span>|
|<span data-ttu-id="450f1-115">Application</span><span class="sxs-lookup"><span data-stu-id="450f1-115">Application</span></span>|<span data-ttu-id="450f1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="450f1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="450f1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="450f1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="450f1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="450f1-118">Request headers</span></span>

|<span data-ttu-id="450f1-119">名称</span><span class="sxs-lookup"><span data-stu-id="450f1-119">Name</span></span>|<span data-ttu-id="450f1-120">说明</span><span class="sxs-lookup"><span data-stu-id="450f1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="450f1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="450f1-121">Authorization</span></span>|<span data-ttu-id="450f1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="450f1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="450f1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="450f1-124">Content-Type</span></span>|<span data-ttu-id="450f1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="450f1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="450f1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="450f1-127">Request body</span></span>

<span data-ttu-id="450f1-128">在请求正文中，提供 [userSource](../resources/ediscovery-usersource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="450f1-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="450f1-129">下表显示创建 [userSource](../resources/ediscovery-usersource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="450f1-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="450f1-130">属性</span><span class="sxs-lookup"><span data-stu-id="450f1-130">Property</span></span>|<span data-ttu-id="450f1-131">类型</span><span class="sxs-lookup"><span data-stu-id="450f1-131">Type</span></span>|<span data-ttu-id="450f1-132">说明</span><span class="sxs-lookup"><span data-stu-id="450f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="450f1-133">email</span><span class="sxs-lookup"><span data-stu-id="450f1-133">email</span></span>|<span data-ttu-id="450f1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="450f1-134">String</span></span>|<span data-ttu-id="450f1-135">用户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="450f1-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="450f1-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="450f1-136">includedSources</span></span>|<span data-ttu-id="450f1-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="450f1-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="450f1-138">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="450f1-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="450f1-139">此值必须为 `mailbox` ， `site` 目前不支持 legalHolds。</span><span class="sxs-lookup"><span data-stu-id="450f1-139">This value must be `mailbox`, `site` is not supported for legalHolds at this time.</span></span>|

## <a name="response"></a><span data-ttu-id="450f1-140">响应</span><span class="sxs-lookup"><span data-stu-id="450f1-140">Response</span></span>

<span data-ttu-id="450f1-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="450f1-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="450f1-142">示例</span><span class="sxs-lookup"><span data-stu-id="450f1-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="450f1-143">请求</span><span class="sxs-lookup"><span data-stu-id="450f1-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="450f1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="450f1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources
Content-Type: application/json
Content-length: 208

{
  "email": "adelev@contoso.com",
  "includedSources": "mailbox"
}
```
# <a name="c"></a>[<span data-ttu-id="450f1-145">C#</span><span class="sxs-lookup"><span data-stu-id="450f1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="450f1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="450f1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="450f1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="450f1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="450f1-148">Java</span><span class="sxs-lookup"><span data-stu-id="450f1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="450f1-149">响应</span><span class="sxs-lookup"><span data-stu-id="450f1-149">Response</span></span>

<span data-ttu-id="450f1-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="450f1-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalholds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-12-28T20:08:57.857Z",
            "id": "2192ca40-8ea2-410e-ba3b-ec8ae873be6b",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "EDiscovery admin"
                }
            }
        }
    ]
}
```
