---
title: 获取 userSource
description: 读取 userSource 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0707ca76db4fd63d3fba2cfc9dbb72ba2278817c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873015"
---
# <a name="get-usersource"></a><span data-ttu-id="19edd-103">获取 userSource</span><span class="sxs-lookup"><span data-stu-id="19edd-103">Get userSource</span></span>

<span data-ttu-id="19edd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19edd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19edd-105">读取 [userSource](../resources/usersource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19edd-105">Read the properties and relationships of a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19edd-106">权限</span><span class="sxs-lookup"><span data-stu-id="19edd-106">Permissions</span></span>

<span data-ttu-id="19edd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19edd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="19edd-109">Permission type</span></span>|<span data-ttu-id="19edd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19edd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19edd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19edd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19edd-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="19edd-112">User.Read</span></span>|
|<span data-ttu-id="19edd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19edd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19edd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="19edd-114">Not supported.</span></span>|
|<span data-ttu-id="19edd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="19edd-115">Application</span></span>|<span data-ttu-id="19edd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19edd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19edd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19edd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19edd-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19edd-118">Optional query parameters</span></span>

<span data-ttu-id="19edd-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19edd-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="19edd-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="19edd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="19edd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="19edd-121">Request headers</span></span>

|<span data-ttu-id="19edd-122">名称</span><span class="sxs-lookup"><span data-stu-id="19edd-122">Name</span></span>|<span data-ttu-id="19edd-123">说明</span><span class="sxs-lookup"><span data-stu-id="19edd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="19edd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="19edd-124">Authorization</span></span>|<span data-ttu-id="19edd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19edd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19edd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19edd-127">Request body</span></span>

<span data-ttu-id="19edd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19edd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19edd-129">响应</span><span class="sxs-lookup"><span data-stu-id="19edd-129">Response</span></span>

<span data-ttu-id="19edd-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [userSource](../resources/usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19edd-130">If successful, this method returns a `200 OK` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19edd-131">示例</span><span class="sxs-lookup"><span data-stu-id="19edd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19edd-132">请求</span><span class="sxs-lookup"><span data-stu-id="19edd-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```

### <a name="response"></a><span data-ttu-id="19edd-133">响应</span><span class="sxs-lookup"><span data-stu-id="19edd-133">Response</span></span>

<span data-ttu-id="19edd-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="19edd-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
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
