---
title: 创建 legalHold userSource
description: 创建新的 legalHold userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 92652621016d25d2c712ccdd87b730d7f94d576d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446038"
---
# <a name="create-legalhold-usersource"></a><span data-ttu-id="ae6a4-103">创建 legalHold userSource</span><span class="sxs-lookup"><span data-stu-id="ae6a4-103">Create legalHold userSource</span></span>

<span data-ttu-id="ae6a4-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ae6a4-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae6a4-105">将 userSource 添加到 legalHold 对象。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-105">Adds a userSource to a legalHold object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae6a4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ae6a4-106">Permissions</span></span>

<span data-ttu-id="ae6a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae6a4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae6a4-109">Permission type</span></span>|<span data-ttu-id="ae6a4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae6a4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae6a4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae6a4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ae6a4-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6a4-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ae6a4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae6a4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae6a4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-114">Not supported.</span></span>|
|<span data-ttu-id="ae6a4-115">Application</span><span class="sxs-lookup"><span data-stu-id="ae6a4-115">Application</span></span>|<span data-ttu-id="ae6a4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae6a4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae6a4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="ae6a4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae6a4-118">Request headers</span></span>

|<span data-ttu-id="ae6a4-119">名称</span><span class="sxs-lookup"><span data-stu-id="ae6a4-119">Name</span></span>|<span data-ttu-id="ae6a4-120">说明</span><span class="sxs-lookup"><span data-stu-id="ae6a4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ae6a4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae6a4-121">Authorization</span></span>|<span data-ttu-id="ae6a4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ae6a4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae6a4-124">Content-Type</span></span>|<span data-ttu-id="ae6a4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ae6a4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae6a4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae6a4-127">Request body</span></span>

<span data-ttu-id="ae6a4-128">在请求正文中，提供 [userSource](../resources/ediscovery-usersource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="ae6a4-129">下表显示创建 [userSource](../resources/ediscovery-usersource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="ae6a4-130">属性</span><span class="sxs-lookup"><span data-stu-id="ae6a4-130">Property</span></span>|<span data-ttu-id="ae6a4-131">类型</span><span class="sxs-lookup"><span data-stu-id="ae6a4-131">Type</span></span>|<span data-ttu-id="ae6a4-132">说明</span><span class="sxs-lookup"><span data-stu-id="ae6a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae6a4-133">email</span><span class="sxs-lookup"><span data-stu-id="ae6a4-133">email</span></span>|<span data-ttu-id="ae6a4-134">String</span><span class="sxs-lookup"><span data-stu-id="ae6a4-134">String</span></span>|<span data-ttu-id="ae6a4-135">用户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="ae6a4-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="ae6a4-136">includedSources</span></span>|<span data-ttu-id="ae6a4-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="ae6a4-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="ae6a4-138">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="ae6a4-139">目前 `mailbox` `site` ，legalHolds 不支持此值。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-139">This value must be `mailbox`, `site` is not supported for legalHolds at this time.</span></span>|

## <a name="response"></a><span data-ttu-id="ae6a4-140">响应</span><span class="sxs-lookup"><span data-stu-id="ae6a4-140">Response</span></span>

<span data-ttu-id="ae6a4-141">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae6a4-142">示例</span><span class="sxs-lookup"><span data-stu-id="ae6a4-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae6a4-143">请求</span><span class="sxs-lookup"><span data-stu-id="ae6a4-143">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="ae6a4-144">响应</span><span class="sxs-lookup"><span data-stu-id="ae6a4-144">Response</span></span>

<span data-ttu-id="ae6a4-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ae6a4-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
