---
title: 创建 userSource
description: 创建新的 userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0534acf5e440105f3f423ce3d96d98db98d093f0
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872518"
---
# <a name="create-usersource"></a><span data-ttu-id="15be7-103">创建 userSource</span><span class="sxs-lookup"><span data-stu-id="15be7-103">Create userSource</span></span>

<span data-ttu-id="15be7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15be7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15be7-105">创建新的 [userSource](../resources/usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="15be7-105">Create a new [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="15be7-106">权限</span><span class="sxs-lookup"><span data-stu-id="15be7-106">Permissions</span></span>

<span data-ttu-id="15be7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15be7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15be7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="15be7-109">Permission type</span></span>|<span data-ttu-id="15be7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15be7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15be7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15be7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15be7-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="15be7-112">User.Read</span></span>|
|<span data-ttu-id="15be7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15be7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15be7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="15be7-114">Not supported.</span></span>|
|<span data-ttu-id="15be7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="15be7-115">Application</span></span>|<span data-ttu-id="15be7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="15be7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15be7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15be7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="15be7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="15be7-118">Request headers</span></span>

|<span data-ttu-id="15be7-119">名称</span><span class="sxs-lookup"><span data-stu-id="15be7-119">Name</span></span>|<span data-ttu-id="15be7-120">说明</span><span class="sxs-lookup"><span data-stu-id="15be7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="15be7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="15be7-121">Authorization</span></span>|<span data-ttu-id="15be7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15be7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="15be7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15be7-124">Content-Type</span></span>|<span data-ttu-id="15be7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="15be7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15be7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="15be7-127">Request body</span></span>

<span data-ttu-id="15be7-128">在请求正文中，提供 [userSource](../resources/usersource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15be7-128">In the request body, supply a JSON representation of the [userSource](../resources/usersource.md) object.</span></span>

<span data-ttu-id="15be7-129">下表显示创建 [userSource](../resources/usersource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="15be7-129">The following table shows the properties that are required when you create the [userSource](../resources/usersource.md).</span></span>

|<span data-ttu-id="15be7-130">属性</span><span class="sxs-lookup"><span data-stu-id="15be7-130">Property</span></span>|<span data-ttu-id="15be7-131">类型</span><span class="sxs-lookup"><span data-stu-id="15be7-131">Type</span></span>|<span data-ttu-id="15be7-132">Description</span><span class="sxs-lookup"><span data-stu-id="15be7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15be7-133">email</span><span class="sxs-lookup"><span data-stu-id="15be7-133">email</span></span>|<span data-ttu-id="15be7-134">String</span><span class="sxs-lookup"><span data-stu-id="15be7-134">String</span></span>|<span data-ttu-id="15be7-135">用户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="15be7-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="15be7-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="15be7-136">includedSources</span></span>|<span data-ttu-id="15be7-137">sourceType</span><span class="sxs-lookup"><span data-stu-id="15be7-137">sourceType</span></span>|<span data-ttu-id="15be7-138">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="15be7-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="15be7-139">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="15be7-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="15be7-140">响应</span><span class="sxs-lookup"><span data-stu-id="15be7-140">Response</span></span>

<span data-ttu-id="15be7-141">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [userSource](../resources/usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="15be7-141">If successful, this method returns a `201 Created` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15be7-142">示例</span><span class="sxs-lookup"><span data-stu-id="15be7-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15be7-143">请求</span><span class="sxs-lookup"><span data-stu-id="15be7-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="15be7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="15be7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
Content-Type: application/json
Content-length: 233

{
    "email":"megan@contoso.com",
    "includedSources":"mailbox, site"
}
```
# <a name="c"></a>[<span data-ttu-id="15be7-145">C#</span><span class="sxs-lookup"><span data-stu-id="15be7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15be7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15be7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15be7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15be7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15be7-148">Java</span><span class="sxs-lookup"><span data-stu-id="15be7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15be7-149">响应</span><span class="sxs-lookup"><span data-stu-id="15be7-149">Response</span></span>

<span data-ttu-id="15be7-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="15be7-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('45454331323337443946343043464239')/userSources/$entity",
    "displayName": "Megan Bowen",
    "createdDateTime": "2020-11-06T16:09:08.4905571Z",
    "id": "34383036-3741-4545-3242-373530353435",
    "email": "megan@contoso.com",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
