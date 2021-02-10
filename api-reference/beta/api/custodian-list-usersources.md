---
title: 列出 userSources
description: 获取 userSource 对象及其属性的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 2812fe2bfbcd6540462122dcfcaddaee8c54ca9b
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176575"
---
# <a name="list-usersources"></a><span data-ttu-id="ed8b1-103">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="ed8b1-103">List userSources</span></span>

<span data-ttu-id="ed8b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed8b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed8b1-105">获取 [userSource 对象](../resources/usersource.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-105">Get a list of the [userSource](../resources/usersource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed8b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed8b1-106">Permissions</span></span>

<span data-ttu-id="ed8b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed8b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed8b1-109">Permission type</span></span>|<span data-ttu-id="ed8b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed8b1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed8b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed8b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed8b1-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="ed8b1-112">User.Read</span></span>|
|<span data-ttu-id="ed8b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed8b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed8b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-114">Not supported.</span></span>|
|<span data-ttu-id="ed8b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed8b1-115">Application</span></span>|<span data-ttu-id="ed8b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed8b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed8b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed8b1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed8b1-118">Optional query parameters</span></span>

<span data-ttu-id="ed8b1-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ed8b1-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed8b1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed8b1-121">Request headers</span></span>

|<span data-ttu-id="ed8b1-122">名称</span><span class="sxs-lookup"><span data-stu-id="ed8b1-122">Name</span></span>|<span data-ttu-id="ed8b1-123">说明</span><span class="sxs-lookup"><span data-stu-id="ed8b1-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed8b1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed8b1-124">Authorization</span></span>|<span data-ttu-id="ed8b1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed8b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed8b1-127">Request body</span></span>

<span data-ttu-id="ed8b1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed8b1-129">响应</span><span class="sxs-lookup"><span data-stu-id="ed8b1-129">Response</span></span>

<span data-ttu-id="ed8b1-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [userSource](../resources/usersource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-130">If successful, this method returns a `200 OK` response code and a collection of [userSource](../resources/usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed8b1-131">示例</span><span class="sxs-lookup"><span data-stu-id="ed8b1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed8b1-132">请求</span><span class="sxs-lookup"><span data-stu-id="ed8b1-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed8b1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed8b1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
```
# <a name="c"></a>[<span data-ttu-id="ed8b1-134">C#</span><span class="sxs-lookup"><span data-stu-id="ed8b1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed8b1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed8b1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed8b1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed8b1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed8b1-137">Java</span><span class="sxs-lookup"><span data-stu-id="ed8b1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed8b1-138">响应</span><span class="sxs-lookup"><span data-stu-id="ed8b1-138">Response</span></span>

<span data-ttu-id="ed8b1-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed8b1-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/userSources",
    "value": [
        {
            "displayName": "Megan Bowen",
            "createdDateTime": "2020-08-21T13:20:01.3430206Z",
            "id": "46384443-4137-3032-3437-363939433735",
            "email": "megan@contoso.com",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "Adele Vance"
                }
            }
        }
    ]
}
```
