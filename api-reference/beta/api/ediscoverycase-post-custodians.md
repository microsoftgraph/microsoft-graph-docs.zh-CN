---
title: 创建管理员
description: 创建新的保管人对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 7142d00f7fdee7643e5c6c2b755c1c88a1e9f9dc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597584"
---
# <a name="create-custodian"></a><span data-ttu-id="14929-103">创建管理员</span><span class="sxs-lookup"><span data-stu-id="14929-103">Create custodian</span></span>

<span data-ttu-id="14929-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14929-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14929-105">创建新的 [保管人](../resources/custodian.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14929-105">Create a new [custodian](../resources/custodian.md) object.</span></span> <span data-ttu-id="14929-106">创建保管人对象后，您需要创建该保管人的 [userSource](../resources/usersource.md) ，以引用其邮箱和 OneDrive for business 网站。</span><span class="sxs-lookup"><span data-stu-id="14929-106">After the custodian object is created, you will need to create the custodian's [userSource](../resources/usersource.md) to reference their mailbox and OneDrive for Business site.</span></span>

## <a name="permissions"></a><span data-ttu-id="14929-107">权限</span><span class="sxs-lookup"><span data-stu-id="14929-107">Permissions</span></span>

<span data-ttu-id="14929-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14929-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14929-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14929-110">Permission type</span></span>|<span data-ttu-id="14929-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="14929-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14929-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14929-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14929-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="14929-113">User.Read</span></span>|
|<span data-ttu-id="14929-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14929-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14929-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14929-115">Not supported.</span></span>|
|<span data-ttu-id="14929-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14929-116">Application</span></span>|<span data-ttu-id="14929-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="14929-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14929-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14929-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a><span data-ttu-id="14929-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="14929-119">Request headers</span></span>

|<span data-ttu-id="14929-120">名称</span><span class="sxs-lookup"><span data-stu-id="14929-120">Name</span></span>|<span data-ttu-id="14929-121">说明</span><span class="sxs-lookup"><span data-stu-id="14929-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="14929-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14929-122">Authorization</span></span>|<span data-ttu-id="14929-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14929-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="14929-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14929-125">Content-Type</span></span>|<span data-ttu-id="14929-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="14929-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14929-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="14929-128">Request body</span></span>

<span data-ttu-id="14929-129">在请求正文中，提供 [保管人](../resources/custodian.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14929-129">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="14929-130">下表显示创建 [保管人](../resources/custodian.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="14929-130">The following table shows the properties that are required when you create the [custodian](../resources/custodian.md).</span></span>

|<span data-ttu-id="14929-131">属性</span><span class="sxs-lookup"><span data-stu-id="14929-131">Property</span></span>|<span data-ttu-id="14929-132">类型</span><span class="sxs-lookup"><span data-stu-id="14929-132">Type</span></span>|<span data-ttu-id="14929-133">Description</span><span class="sxs-lookup"><span data-stu-id="14929-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14929-134">email</span><span class="sxs-lookup"><span data-stu-id="14929-134">email</span></span>|<span data-ttu-id="14929-135">String</span><span class="sxs-lookup"><span data-stu-id="14929-135">String</span></span>|<span data-ttu-id="14929-136">保管人的主 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="14929-136">Custodian's primary SMTP address.</span></span> <span data-ttu-id="14929-137">必需。</span><span class="sxs-lookup"><span data-stu-id="14929-137">Required.</span></span>|
|<span data-ttu-id="14929-138">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="14929-138">applyHoldToSources</span></span>|<span data-ttu-id="14929-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="14929-139">Boolean</span></span>|<span data-ttu-id="14929-140">指示是否将保留应用于保管人的源 (如邮箱、网站或团队) 。</span><span class="sxs-lookup"><span data-stu-id="14929-140">Indicates whether a hold is applied to the custodian's sources (such as mailboxes, sites, or Teams).</span></span>|

## <a name="response"></a><span data-ttu-id="14929-141">响应</span><span class="sxs-lookup"><span data-stu-id="14929-141">Response</span></span>

<span data-ttu-id="14929-142">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [保管人](../resources/custodian.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14929-142">If successful, this method returns a `201 Created` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14929-143">示例</span><span class="sxs-lookup"><span data-stu-id="14929-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14929-144">请求</span><span class="sxs-lookup"><span data-stu-id="14929-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_custodian_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
Content-Type: application/json
Content-length: 279

{
    "email":"AdeleV@contoso.com",
    "applyHoldToSources":"true"
}
```

### <a name="response"></a><span data-ttu-id="14929-145">响应</span><span class="sxs-lookup"><span data-stu-id="14929-145">Response</span></span>

<span data-ttu-id="14929-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="14929-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:47:01.7724531Z",
    "lastModifiedDateTime": "2020-10-30T20:47:02.2512381Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45353243323138344430413038363846",
    "displayName": "Adele Vance"
}
```
