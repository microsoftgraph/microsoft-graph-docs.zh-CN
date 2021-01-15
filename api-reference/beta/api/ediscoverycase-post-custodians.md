---
title: 创建保管人
description: 创建新的保管人对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: e4883c75919535bc68d4f2559e920b467344a2a7
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873652"
---
# <a name="create-custodian"></a><span data-ttu-id="ebee4-103">创建保管人</span><span class="sxs-lookup"><span data-stu-id="ebee4-103">Create custodian</span></span>

<span data-ttu-id="ebee4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebee4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebee4-105">创建新的保管 [人](../resources/custodian.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebee4-105">Create a new [custodian](../resources/custodian.md) object.</span></span> <span data-ttu-id="ebee4-106">创建保管人对象后，你需要创建保管人 [的用户来源](../resources/usersource.md) 以引用其邮箱和 OneDrive for Business 网站。</span><span class="sxs-lookup"><span data-stu-id="ebee4-106">After the custodian object is created, you will need to create the custodian's [userSource](../resources/usersource.md) to reference their mailbox and OneDrive for Business site.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebee4-107">权限</span><span class="sxs-lookup"><span data-stu-id="ebee4-107">Permissions</span></span>

<span data-ttu-id="ebee4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebee4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebee4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebee4-110">Permission type</span></span>|<span data-ttu-id="ebee4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebee4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebee4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebee4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebee4-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="ebee4-113">User.Read</span></span>|
|<span data-ttu-id="ebee4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebee4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebee4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebee4-115">Not supported.</span></span>|
|<span data-ttu-id="ebee4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebee4-116">Application</span></span>|<span data-ttu-id="ebee4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebee4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebee4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebee4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a><span data-ttu-id="ebee4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebee4-119">Request headers</span></span>

|<span data-ttu-id="ebee4-120">名称</span><span class="sxs-lookup"><span data-stu-id="ebee4-120">Name</span></span>|<span data-ttu-id="ebee4-121">说明</span><span class="sxs-lookup"><span data-stu-id="ebee4-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ebee4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebee4-122">Authorization</span></span>|<span data-ttu-id="ebee4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebee4-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ebee4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebee4-125">Content-Type</span></span>|<span data-ttu-id="ebee4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ebee4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebee4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebee4-128">Request body</span></span>

<span data-ttu-id="ebee4-129">在请求正文中，提供保管人对象的 JSON [表示](../resources/custodian.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="ebee4-129">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="ebee4-130">下表显示创建保管人时所需的 [属性](../resources/custodian.md)。</span><span class="sxs-lookup"><span data-stu-id="ebee4-130">The following table shows the properties that are required when you create the [custodian](../resources/custodian.md).</span></span>

|<span data-ttu-id="ebee4-131">属性</span><span class="sxs-lookup"><span data-stu-id="ebee4-131">Property</span></span>|<span data-ttu-id="ebee4-132">类型</span><span class="sxs-lookup"><span data-stu-id="ebee4-132">Type</span></span>|<span data-ttu-id="ebee4-133">Description</span><span class="sxs-lookup"><span data-stu-id="ebee4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebee4-134">email</span><span class="sxs-lookup"><span data-stu-id="ebee4-134">email</span></span>|<span data-ttu-id="ebee4-135">String</span><span class="sxs-lookup"><span data-stu-id="ebee4-135">String</span></span>|<span data-ttu-id="ebee4-136">保管人的主 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="ebee4-136">Custodian's primary SMTP address.</span></span> <span data-ttu-id="ebee4-137">必需。</span><span class="sxs-lookup"><span data-stu-id="ebee4-137">Required.</span></span>|
|<span data-ttu-id="ebee4-138">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="ebee4-138">applyHoldToSources</span></span>|<span data-ttu-id="ebee4-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebee4-139">Boolean</span></span>|<span data-ttu-id="ebee4-140">指示是否将保留应用于保管人的来源 (邮箱、网站或 Teams) 。</span><span class="sxs-lookup"><span data-stu-id="ebee4-140">Indicates whether a hold is applied to the custodian's sources (such as mailboxes, sites, or Teams).</span></span>|

## <a name="response"></a><span data-ttu-id="ebee4-141">响应</span><span class="sxs-lookup"><span data-stu-id="ebee4-141">Response</span></span>

<span data-ttu-id="ebee4-142">如果成功，此方法在响应 `201 Created` 正文中返回响应代码[](../resources/custodian.md)和保管人对象。</span><span class="sxs-lookup"><span data-stu-id="ebee4-142">If successful, this method returns a `201 Created` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebee4-143">示例</span><span class="sxs-lookup"><span data-stu-id="ebee4-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebee4-144">请求</span><span class="sxs-lookup"><span data-stu-id="ebee4-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ebee4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebee4-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ebee4-146">C#</span><span class="sxs-lookup"><span data-stu-id="ebee4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-custodian-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebee4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebee4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-custodian-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebee4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebee4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-custodian-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebee4-149">Java</span><span class="sxs-lookup"><span data-stu-id="ebee4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-custodian-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ebee4-150">响应</span><span class="sxs-lookup"><span data-stu-id="ebee4-150">Response</span></span>

<span data-ttu-id="ebee4-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ebee4-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
