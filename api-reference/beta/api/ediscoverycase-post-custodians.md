---
title: 创建保管人
description: 创建新的保管人对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: e5472f9c3ff80a1e1fb127ebddc566880e2056aa
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659523"
---
# <a name="create-custodian"></a><span data-ttu-id="68ae2-103">创建保管人</span><span class="sxs-lookup"><span data-stu-id="68ae2-103">Create custodian</span></span>

<span data-ttu-id="68ae2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68ae2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68ae2-105">创建新的保管 [人](../resources/custodian.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68ae2-105">Create a new [custodian](../resources/custodian.md) object.</span></span> <span data-ttu-id="68ae2-106">创建保管人对象后，你需要创建保管人 [的用户来源](../resources/usersource.md) 以引用其邮箱和 OneDrive for Business 网站。</span><span class="sxs-lookup"><span data-stu-id="68ae2-106">After the custodian object is created, you will need to create the custodian's [userSource](../resources/usersource.md) to reference their mailbox and OneDrive for Business site.</span></span>

## <a name="permissions"></a><span data-ttu-id="68ae2-107">权限</span><span class="sxs-lookup"><span data-stu-id="68ae2-107">Permissions</span></span>

<span data-ttu-id="68ae2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68ae2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68ae2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="68ae2-110">Permission type</span></span>|<span data-ttu-id="68ae2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="68ae2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68ae2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68ae2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68ae2-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="68ae2-113">User.Read</span></span>|
|<span data-ttu-id="68ae2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68ae2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68ae2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="68ae2-115">Not supported.</span></span>|
|<span data-ttu-id="68ae2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="68ae2-116">Application</span></span>|<span data-ttu-id="68ae2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="68ae2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68ae2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68ae2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a><span data-ttu-id="68ae2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="68ae2-119">Request headers</span></span>

|<span data-ttu-id="68ae2-120">名称</span><span class="sxs-lookup"><span data-stu-id="68ae2-120">Name</span></span>|<span data-ttu-id="68ae2-121">说明</span><span class="sxs-lookup"><span data-stu-id="68ae2-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="68ae2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68ae2-122">Authorization</span></span>|<span data-ttu-id="68ae2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68ae2-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="68ae2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68ae2-125">Content-Type</span></span>|<span data-ttu-id="68ae2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="68ae2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68ae2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="68ae2-128">Request body</span></span>

<span data-ttu-id="68ae2-129">在请求正文中，提供保管人对象的 JSON [表示](../resources/custodian.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="68ae2-129">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="68ae2-130">下表显示创建保管人时所需的 [属性](../resources/custodian.md)。</span><span class="sxs-lookup"><span data-stu-id="68ae2-130">The following table shows the properties that are required when you create the [custodian](../resources/custodian.md).</span></span>

|<span data-ttu-id="68ae2-131">属性</span><span class="sxs-lookup"><span data-stu-id="68ae2-131">Property</span></span>|<span data-ttu-id="68ae2-132">类型</span><span class="sxs-lookup"><span data-stu-id="68ae2-132">Type</span></span>|<span data-ttu-id="68ae2-133">说明</span><span class="sxs-lookup"><span data-stu-id="68ae2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68ae2-134">email</span><span class="sxs-lookup"><span data-stu-id="68ae2-134">email</span></span>|<span data-ttu-id="68ae2-135">String</span><span class="sxs-lookup"><span data-stu-id="68ae2-135">String</span></span>|<span data-ttu-id="68ae2-136">保管人的主 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="68ae2-136">Custodian's primary SMTP address.</span></span> <span data-ttu-id="68ae2-137">必填。</span><span class="sxs-lookup"><span data-stu-id="68ae2-137">Required.</span></span>|
|<span data-ttu-id="68ae2-138">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="68ae2-138">applyHoldToSources</span></span>|<span data-ttu-id="68ae2-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="68ae2-139">Boolean</span></span>|<span data-ttu-id="68ae2-140">指示是否将保留应用于保管人的来源 (邮箱、网站或 Teams) 。</span><span class="sxs-lookup"><span data-stu-id="68ae2-140">Indicates whether a hold is applied to the custodian's sources (such as mailboxes, sites, or Teams).</span></span>|

## <a name="response"></a><span data-ttu-id="68ae2-141">响应</span><span class="sxs-lookup"><span data-stu-id="68ae2-141">Response</span></span>

<span data-ttu-id="68ae2-142">如果成功，此方法在响应 `201 Created` 正文中返回响应代码[](../resources/custodian.md)和保管人对象。</span><span class="sxs-lookup"><span data-stu-id="68ae2-142">If successful, this method returns a `201 Created` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68ae2-143">示例</span><span class="sxs-lookup"><span data-stu-id="68ae2-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68ae2-144">请求</span><span class="sxs-lookup"><span data-stu-id="68ae2-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="68ae2-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="68ae2-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_custodian_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
Content-Type: application/json
Content-length: 279

{
    "email":"AdeleV@contoso.com",
    "applyHoldToSources":"true"
}
```
# <a name="c"></a>[<span data-ttu-id="68ae2-146">C#</span><span class="sxs-lookup"><span data-stu-id="68ae2-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-custodian-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68ae2-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68ae2-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-custodian-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68ae2-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68ae2-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-custodian-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68ae2-149">Java</span><span class="sxs-lookup"><span data-stu-id="68ae2-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-custodian-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68ae2-150">响应</span><span class="sxs-lookup"><span data-stu-id="68ae2-150">Response</span></span>

<span data-ttu-id="68ae2-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="68ae2-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:47:01.7724531Z",
    "lastModifiedDateTime": "2020-10-30T20:47:02.2512381Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45353243323138344430413038363846",
    "displayName": "Adele Vance"
}
```
