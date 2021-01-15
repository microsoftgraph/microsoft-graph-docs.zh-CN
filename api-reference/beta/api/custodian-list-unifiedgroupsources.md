---
title: 列出 unifiedGroupSources
description: 获取 unifiedGroupSource 对象及其属性的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 901006dc63aec6920e9183b632937b9651884d6b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872581"
---
# <a name="list-unifiedgroupsources"></a><span data-ttu-id="ec97b-103">列出 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="ec97b-103">List unifiedGroupSources</span></span>

<span data-ttu-id="ec97b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec97b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec97b-105">获取 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="ec97b-105">Get a list of the [unifiedGroupSource](../resources/unifiedgroupsource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec97b-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec97b-106">Permissions</span></span>

<span data-ttu-id="ec97b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec97b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec97b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec97b-109">Permission type</span></span>|<span data-ttu-id="ec97b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec97b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec97b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec97b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec97b-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="ec97b-112">User.Read</span></span>|
|<span data-ttu-id="ec97b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec97b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec97b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec97b-114">Not supported.</span></span>|
|<span data-ttu-id="ec97b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec97b-115">Application</span></span>|<span data-ttu-id="ec97b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec97b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec97b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec97b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec97b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec97b-118">Optional query parameters</span></span>

<span data-ttu-id="ec97b-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ec97b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ec97b-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ec97b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec97b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec97b-121">Request headers</span></span>

|<span data-ttu-id="ec97b-122">名称</span><span class="sxs-lookup"><span data-stu-id="ec97b-122">Name</span></span>|<span data-ttu-id="ec97b-123">说明</span><span class="sxs-lookup"><span data-stu-id="ec97b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec97b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec97b-124">Authorization</span></span>|<span data-ttu-id="ec97b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec97b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec97b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec97b-127">Request body</span></span>

<span data-ttu-id="ec97b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec97b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec97b-129">响应</span><span class="sxs-lookup"><span data-stu-id="ec97b-129">Response</span></span>

<span data-ttu-id="ec97b-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ec97b-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedGroupSource](../resources/unifiedgroupsource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec97b-131">示例</span><span class="sxs-lookup"><span data-stu-id="ec97b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec97b-132">请求</span><span class="sxs-lookup"><span data-stu-id="ec97b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ec97b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec97b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedgroupsource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```
# <a name="c"></a>[<span data-ttu-id="ec97b-134">C#</span><span class="sxs-lookup"><span data-stu-id="ec97b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec97b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec97b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec97b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec97b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec97b-137">Java</span><span class="sxs-lookup"><span data-stu-id="ec97b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec97b-138">响应</span><span class="sxs-lookup"><span data-stu-id="ec97b-138">Response</span></span>

<span data-ttu-id="ec97b-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ec97b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedGroupSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "Megan Bowen"
                }
            }
        }
    ]
}
```
