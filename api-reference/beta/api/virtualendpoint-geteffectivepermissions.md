---
title: virtualEndpoint：getEffectivePermissions
description: '**GetEffectivePermissions 是一个函数，可重试当前经过身份验证的用户的有效权限，这有助于 UX 隐藏或禁用当前用户无权访问的内容。**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e87deb3bafbcd1ac28a1d95209f62017d7593e6c
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714345"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="31392-103">virtualEndpoint：getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="31392-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="31392-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31392-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31392-105">查看当前经过身份验证的用户的有效权限。</span><span class="sxs-lookup"><span data-stu-id="31392-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="31392-106">GetEffectivePermissions 是一个函数，可重试当前经过身份验证的用户的有效权限，这有助于 UX 隐藏或禁用当前用户无权访问的内容。</span><span class="sxs-lookup"><span data-stu-id="31392-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="31392-107">权限</span><span class="sxs-lookup"><span data-stu-id="31392-107">Permissions</span></span>

<span data-ttu-id="31392-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31392-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31392-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="31392-110">Permission type</span></span>|<span data-ttu-id="31392-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31392-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31392-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31392-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31392-113">CloudPC.ReadWrite.All、CloudPC.Read.All</span><span class="sxs-lookup"><span data-stu-id="31392-113">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="31392-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31392-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31392-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31392-115">Not supported.</span></span>|
|<span data-ttu-id="31392-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="31392-116">Application</span></span>| <span data-ttu-id="31392-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="31392-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31392-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31392-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="31392-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="31392-119">Request headers</span></span>

| <span data-ttu-id="31392-120">名称</span><span class="sxs-lookup"><span data-stu-id="31392-120">Name</span></span>          | <span data-ttu-id="31392-121">说明</span><span class="sxs-lookup"><span data-stu-id="31392-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="31392-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31392-122">Authorization</span></span> | <span data-ttu-id="31392-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31392-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31392-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="31392-125">Request body</span></span>

<span data-ttu-id="31392-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31392-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31392-127">响应</span><span class="sxs-lookup"><span data-stu-id="31392-127">Response</span></span>

<span data-ttu-id="31392-128">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="31392-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="31392-129">如果用户具有完全权限，则响应为 `["*"]` 。</span><span class="sxs-lookup"><span data-stu-id="31392-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="31392-130">示例</span><span class="sxs-lookup"><span data-stu-id="31392-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31392-131">请求</span><span class="sxs-lookup"><span data-stu-id="31392-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="31392-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="31392-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```
# <a name="c"></a>[<span data-ttu-id="31392-133">C#</span><span class="sxs-lookup"><span data-stu-id="31392-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/virtualendpoint-geteffectivepermissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31392-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31392-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/virtualendpoint-geteffectivepermissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31392-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31392-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/virtualendpoint-geteffectivepermissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31392-136">Java</span><span class="sxs-lookup"><span data-stu-id="31392-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/virtualendpoint-geteffectivepermissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31392-137">响应</span><span class="sxs-lookup"><span data-stu-id="31392-137">Response</span></span>

<span data-ttu-id="31392-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="31392-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      "Microsoft.CloudPC/CloudPCs/Read"
   ]
}
```
