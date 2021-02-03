---
title: cloudPcOnPremisesConnection： updateAdDomainPassword
description: 为成功的 onPremisesConnection 更新 AD 域密码。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b43179d906d8fa14e961cd097b21a43605576893
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092311"
---
# <a name="cloudpconpremisesconnection-updateaddomainpassword"></a><span data-ttu-id="bd879-103">cloudPcOnPremisesConnection： updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="bd879-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span></span>
<span data-ttu-id="bd879-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd879-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd879-105">更新 [onPremisesConnection](../resources/cloudpconpremisesconnection.md)的 Active Directory 域密码。</span><span class="sxs-lookup"><span data-stu-id="bd879-105">Update Active Directory domain password for an [onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="bd879-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd879-106">Permissions</span></span>
<span data-ttu-id="bd879-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd879-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd879-109">Permission type</span></span>|<span data-ttu-id="bd879-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd879-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd879-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd879-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd879-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd879-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="bd879-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd879-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd879-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd879-114">Not supported.</span></span>|
|<span data-ttu-id="bd879-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd879-115">Application</span></span>|<span data-ttu-id="bd879-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd879-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd879-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd879-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
```

## <a name="request-headers"></a><span data-ttu-id="bd879-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd879-118">Request headers</span></span>
|<span data-ttu-id="bd879-119">名称</span><span class="sxs-lookup"><span data-stu-id="bd879-119">Name</span></span>|<span data-ttu-id="bd879-120">说明</span><span class="sxs-lookup"><span data-stu-id="bd879-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bd879-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd879-121">Authorization</span></span>|<span data-ttu-id="bd879-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd879-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bd879-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd879-124">Content-Type</span></span>|<span data-ttu-id="bd879-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bd879-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd879-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd879-127">Request body</span></span>
<span data-ttu-id="bd879-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd879-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bd879-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="bd879-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bd879-130">参数</span><span class="sxs-lookup"><span data-stu-id="bd879-130">Parameter</span></span>|<span data-ttu-id="bd879-131">类型</span><span class="sxs-lookup"><span data-stu-id="bd879-131">Type</span></span>|<span data-ttu-id="bd879-132">Description</span><span class="sxs-lookup"><span data-stu-id="bd879-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd879-133">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="bd879-133">adDomainPassword</span></span>|<span data-ttu-id="bd879-134">String</span><span class="sxs-lookup"><span data-stu-id="bd879-134">String</span></span>|<span data-ttu-id="bd879-135">与 adDomainUsername 关联的密码</span><span class="sxs-lookup"><span data-stu-id="bd879-135">The password associated with adDomainUsername</span></span>|



## <a name="response"></a><span data-ttu-id="bd879-136">响应</span><span class="sxs-lookup"><span data-stu-id="bd879-136">Response</span></span>

<span data-ttu-id="bd879-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bd879-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bd879-138">示例</span><span class="sxs-lookup"><span data-stu-id="bd879-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd879-139">请求</span><span class="sxs-lookup"><span data-stu-id="bd879-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bd879-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd879-140">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="bd879-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd879-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-updateaddomainpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd879-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd879-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-updateaddomainpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bd879-143">响应</span><span class="sxs-lookup"><span data-stu-id="bd879-143">Response</span></span>
<span data-ttu-id="bd879-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bd879-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
