---
title: cloudPcOnPremisesConnection：updateAdDomainPassword
description: 为成功的 onPremisesConnection 更新 AD 域密码。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6a7420574c8dc1a4231f9854a10b76b7291b3ad4
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546831"
---
# <a name="cloudpconpremisesconnection-updateaddomainpassword"></a><span data-ttu-id="9d994-103">cloudPcOnPremisesConnection：updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="9d994-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span></span>
<span data-ttu-id="9d994-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d994-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d994-105">更新 [onPremisesConnection](../resources/cloudpconpremisesconnection.md)的 Active Directory 域密码。</span><span class="sxs-lookup"><span data-stu-id="9d994-105">Update Active Directory domain password for an [onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="9d994-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d994-106">Permissions</span></span>
<span data-ttu-id="9d994-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d994-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d994-109">Permission type</span></span>|<span data-ttu-id="9d994-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d994-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d994-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d994-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d994-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d994-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9d994-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d994-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d994-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d994-114">Not supported.</span></span>|
|<span data-ttu-id="9d994-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d994-115">Application</span></span>|<span data-ttu-id="9d994-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d994-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d994-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d994-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
```

## <a name="request-headers"></a><span data-ttu-id="9d994-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d994-118">Request headers</span></span>
|<span data-ttu-id="9d994-119">名称</span><span class="sxs-lookup"><span data-stu-id="9d994-119">Name</span></span>|<span data-ttu-id="9d994-120">说明</span><span class="sxs-lookup"><span data-stu-id="9d994-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9d994-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d994-121">Authorization</span></span>|<span data-ttu-id="9d994-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d994-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9d994-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d994-124">Content-Type</span></span>|<span data-ttu-id="9d994-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9d994-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d994-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d994-127">Request body</span></span>
<span data-ttu-id="9d994-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d994-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9d994-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9d994-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9d994-130">参数</span><span class="sxs-lookup"><span data-stu-id="9d994-130">Parameter</span></span>|<span data-ttu-id="9d994-131">类型</span><span class="sxs-lookup"><span data-stu-id="9d994-131">Type</span></span>|<span data-ttu-id="9d994-132">说明</span><span class="sxs-lookup"><span data-stu-id="9d994-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d994-133">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="9d994-133">adDomainPassword</span></span>|<span data-ttu-id="9d994-134">String</span><span class="sxs-lookup"><span data-stu-id="9d994-134">String</span></span>|<span data-ttu-id="9d994-135">与 adDomainUsername 关联的密码</span><span class="sxs-lookup"><span data-stu-id="9d994-135">The password associated with adDomainUsername</span></span>|



## <a name="response"></a><span data-ttu-id="9d994-136">响应</span><span class="sxs-lookup"><span data-stu-id="9d994-136">Response</span></span>

<span data-ttu-id="9d994-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9d994-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9d994-138">示例</span><span class="sxs-lookup"><span data-stu-id="9d994-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d994-139">请求</span><span class="sxs-lookup"><span data-stu-id="9d994-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9d994-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d994-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_updateaddomainpassword"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
Content-Type: application/json
Content-length: 36

{
  "adDomainPassword": "AdDomainPassword value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="9d994-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d994-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-updateaddomainpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d994-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d994-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-updateaddomainpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9d994-143">响应</span><span class="sxs-lookup"><span data-stu-id="9d994-143">Response</span></span>
<span data-ttu-id="9d994-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9d994-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
