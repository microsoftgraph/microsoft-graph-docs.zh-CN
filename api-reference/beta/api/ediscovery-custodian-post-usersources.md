---
title: 创建保管人 userSource
description: 创建新的保管人 userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 040c4178a269998117e55e86016a4683c5293a2e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446055"
---
# <a name="create-custodian-usersource"></a><span data-ttu-id="d4e41-103">创建保管人 userSource</span><span class="sxs-lookup"><span data-stu-id="d4e41-103">Create custodian userSource</span></span>

<span data-ttu-id="d4e41-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d4e41-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e41-105">创建新的保管人 [userSource](../resources/ediscovery-usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4e41-105">Create a new custodian [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4e41-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d4e41-106">Permissions</span></span>

<span data-ttu-id="d4e41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4e41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e41-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4e41-109">Permission type</span></span>|<span data-ttu-id="d4e41-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4e41-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e41-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4e41-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e41-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e41-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e41-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4e41-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e41-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4e41-114">Not supported.</span></span>|
|<span data-ttu-id="d4e41-115">Application</span><span class="sxs-lookup"><span data-stu-id="d4e41-115">Application</span></span>|<span data-ttu-id="d4e41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4e41-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e41-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4e41-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="d4e41-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4e41-118">Request headers</span></span>

|<span data-ttu-id="d4e41-119">名称</span><span class="sxs-lookup"><span data-stu-id="d4e41-119">Name</span></span>|<span data-ttu-id="d4e41-120">说明</span><span class="sxs-lookup"><span data-stu-id="d4e41-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4e41-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4e41-121">Authorization</span></span>|<span data-ttu-id="d4e41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4e41-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d4e41-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4e41-124">Content-Type</span></span>|<span data-ttu-id="d4e41-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d4e41-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e41-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4e41-127">Request body</span></span>

<span data-ttu-id="d4e41-128">在请求正文中，提供 [userSource](../resources/ediscovery-usersource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4e41-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="d4e41-129">下表显示创建 [userSource](../resources/ediscovery-usersource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4e41-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="d4e41-130">属性</span><span class="sxs-lookup"><span data-stu-id="d4e41-130">Property</span></span>|<span data-ttu-id="d4e41-131">类型</span><span class="sxs-lookup"><span data-stu-id="d4e41-131">Type</span></span>|<span data-ttu-id="d4e41-132">说明</span><span class="sxs-lookup"><span data-stu-id="d4e41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e41-133">email</span><span class="sxs-lookup"><span data-stu-id="d4e41-133">email</span></span>|<span data-ttu-id="d4e41-134">String</span><span class="sxs-lookup"><span data-stu-id="d4e41-134">String</span></span>|<span data-ttu-id="d4e41-135">用户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="d4e41-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="d4e41-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="d4e41-136">includedSources</span></span>|<span data-ttu-id="d4e41-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="d4e41-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="d4e41-138">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="d4e41-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="d4e41-139">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="d4e41-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="d4e41-140">响应</span><span class="sxs-lookup"><span data-stu-id="d4e41-140">Response</span></span>

<span data-ttu-id="d4e41-141">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4e41-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4e41-142">示例</span><span class="sxs-lookup"><span data-stu-id="d4e41-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4e41-143">请求</span><span class="sxs-lookup"><span data-stu-id="d4e41-143">Request</span></span>

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

---

### <a name="response"></a><span data-ttu-id="d4e41-144">响应</span><span class="sxs-lookup"><span data-stu-id="d4e41-144">Response</span></span>

<span data-ttu-id="d4e41-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d4e41-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
