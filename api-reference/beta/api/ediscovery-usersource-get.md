---
title: 获取 userSource
description: 读取 userSource 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 01ad2f83682ac786f35f423fa387293face51114
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515987"
---
# <a name="get-usersource"></a><span data-ttu-id="aee5a-103">获取 userSource</span><span class="sxs-lookup"><span data-stu-id="aee5a-103">Get userSource</span></span>

<span data-ttu-id="aee5a-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="aee5a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aee5a-105">读取 [userSource](../resources/ediscovery-usersource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aee5a-105">Read the properties and relationships of a [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aee5a-106">权限</span><span class="sxs-lookup"><span data-stu-id="aee5a-106">Permissions</span></span>

<span data-ttu-id="aee5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aee5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee5a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aee5a-109">Permission type</span></span>|<span data-ttu-id="aee5a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aee5a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee5a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aee5a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aee5a-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee5a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="aee5a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aee5a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee5a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aee5a-114">Not supported.</span></span>|
|<span data-ttu-id="aee5a-115">Application</span><span class="sxs-lookup"><span data-stu-id="aee5a-115">Application</span></span>|<span data-ttu-id="aee5a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aee5a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee5a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aee5a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aee5a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aee5a-118">Optional query parameters</span></span>

<span data-ttu-id="aee5a-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aee5a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="aee5a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="aee5a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aee5a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="aee5a-121">Request headers</span></span>

|<span data-ttu-id="aee5a-122">名称</span><span class="sxs-lookup"><span data-stu-id="aee5a-122">Name</span></span>|<span data-ttu-id="aee5a-123">说明</span><span class="sxs-lookup"><span data-stu-id="aee5a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aee5a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aee5a-124">Authorization</span></span>|<span data-ttu-id="aee5a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aee5a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee5a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aee5a-127">Request body</span></span>

<span data-ttu-id="aee5a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aee5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aee5a-129">响应</span><span class="sxs-lookup"><span data-stu-id="aee5a-129">Response</span></span>

<span data-ttu-id="aee5a-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aee5a-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aee5a-131">示例</span><span class="sxs-lookup"><span data-stu-id="aee5a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aee5a-132">请求</span><span class="sxs-lookup"><span data-stu-id="aee5a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aee5a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aee5a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="aee5a-134">C#</span><span class="sxs-lookup"><span data-stu-id="aee5a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aee5a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aee5a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aee5a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aee5a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aee5a-137">Java</span><span class="sxs-lookup"><span data-stu-id="aee5a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aee5a-138">响应</span><span class="sxs-lookup"><span data-stu-id="aee5a-138">Response</span></span>

<span data-ttu-id="aee5a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aee5a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/userSources",
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
```
