---
title: 获取 userSource
description: 读取 userSource 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 653c5d45286cfd860dff1397b5ecb65fe23bd992
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597578"
---
# <a name="get-usersource"></a><span data-ttu-id="e2454-103">获取 userSource</span><span class="sxs-lookup"><span data-stu-id="e2454-103">Get userSource</span></span>

<span data-ttu-id="e2454-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2454-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2454-105">读取 [userSource](../resources/usersource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2454-105">Read the properties and relationships of a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2454-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2454-106">Permissions</span></span>

<span data-ttu-id="e2454-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2454-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2454-109">Permission type</span></span>|<span data-ttu-id="e2454-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e2454-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2454-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2454-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2454-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="e2454-112">User.Read</span></span>|
|<span data-ttu-id="e2454-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2454-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2454-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2454-114">Not supported.</span></span>|
|<span data-ttu-id="e2454-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2454-115">Application</span></span>|<span data-ttu-id="e2454-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2454-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2454-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2454-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2454-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2454-118">Optional query parameters</span></span>

<span data-ttu-id="e2454-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2454-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e2454-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e2454-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2454-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2454-121">Request headers</span></span>

|<span data-ttu-id="e2454-122">名称</span><span class="sxs-lookup"><span data-stu-id="e2454-122">Name</span></span>|<span data-ttu-id="e2454-123">说明</span><span class="sxs-lookup"><span data-stu-id="e2454-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e2454-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2454-124">Authorization</span></span>|<span data-ttu-id="e2454-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2454-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2454-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2454-127">Request body</span></span>

<span data-ttu-id="e2454-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2454-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2454-129">响应</span><span class="sxs-lookup"><span data-stu-id="e2454-129">Response</span></span>

<span data-ttu-id="e2454-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [userSource](../resources/usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2454-130">If successful, this method returns a `200 OK` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2454-131">示例</span><span class="sxs-lookup"><span data-stu-id="e2454-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2454-132">请求</span><span class="sxs-lookup"><span data-stu-id="e2454-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```

### <a name="response"></a><span data-ttu-id="e2454-133">响应</span><span class="sxs-lookup"><span data-stu-id="e2454-133">Response</span></span>

<span data-ttu-id="e2454-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2454-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
