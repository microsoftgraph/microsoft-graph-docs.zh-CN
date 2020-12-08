---
title: 更新管理员
description: 更新保管人对象的属性。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c9c58671dd2be9d97e9317cc0b268245402b44e5
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597508"
---
# <a name="update-custodian"></a><span data-ttu-id="6e7eb-103">更新管理员</span><span class="sxs-lookup"><span data-stu-id="6e7eb-103">Update custodian</span></span>

<span data-ttu-id="6e7eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e7eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e7eb-105">更新 [保管人](../resources/custodian.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-105">Update the properties of a [custodian](../resources/custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e7eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="6e7eb-106">Permissions</span></span>

<span data-ttu-id="6e7eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e7eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e7eb-109">Permission type</span></span>|<span data-ttu-id="6e7eb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e7eb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e7eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e7eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e7eb-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="6e7eb-112">User.Read</span></span>|
|<span data-ttu-id="6e7eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e7eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e7eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-114">Not supported.</span></span>|
|<span data-ttu-id="6e7eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e7eb-115">Application</span></span>|<span data-ttu-id="6e7eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e7eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e7eb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="6e7eb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e7eb-118">Request headers</span></span>

|<span data-ttu-id="6e7eb-119">名称</span><span class="sxs-lookup"><span data-stu-id="6e7eb-119">Name</span></span>|<span data-ttu-id="6e7eb-120">说明</span><span class="sxs-lookup"><span data-stu-id="6e7eb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e7eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e7eb-121">Authorization</span></span>|<span data-ttu-id="6e7eb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6e7eb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e7eb-124">Content-Type</span></span>|<span data-ttu-id="6e7eb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6e7eb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e7eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e7eb-127">Request body</span></span>

<span data-ttu-id="6e7eb-128">在请求正文中，提供 [保管人](../resources/custodian.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-128">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="6e7eb-129">下表列出了可修改的 [保管人](../resources/custodian.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-129">The following table lists the properties of a [custodian](../resources/custodian.md) object that can be modified.</span></span>

|<span data-ttu-id="6e7eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="6e7eb-130">Property</span></span>|<span data-ttu-id="6e7eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="6e7eb-131">Type</span></span>|<span data-ttu-id="6e7eb-132">Description</span><span class="sxs-lookup"><span data-stu-id="6e7eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e7eb-133">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="6e7eb-133">applyHoldToSources</span></span>|<span data-ttu-id="6e7eb-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="6e7eb-134">Boolean</span></span>|<span data-ttu-id="6e7eb-135">标识在创建过程中是否将保管人的源置于保留状态。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-135">Identifies whether a custodian's sources were placed on hold during creation.</span></span> <span data-ttu-id="6e7eb-136">有关详细信息，请参阅 [将保管人置于保留状态](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold)。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-136">For details, see [Place custodians on hold](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold).</span></span>|

## <a name="response"></a><span data-ttu-id="6e7eb-137">响应</span><span class="sxs-lookup"><span data-stu-id="6e7eb-137">Response</span></span>

<span data-ttu-id="6e7eb-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [保管人](../resources/custodian.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-138">If successful, this method returns a `200 OK` response code and an updated [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e7eb-139">示例</span><span class="sxs-lookup"><span data-stu-id="6e7eb-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e7eb-140">请求</span><span class="sxs-lookup"><span data-stu-id="6e7eb-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_custodian"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
Content-Type: application/json
Content-length: 254

{
  "applyHoldToSources": "false",
}
```

### <a name="response"></a><span data-ttu-id="6e7eb-141">响应</span><span class="sxs-lookup"><span data-stu-id="6e7eb-141">Response</span></span>

<span data-ttu-id="6e7eb-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6e7eb-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T21:01:34.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
