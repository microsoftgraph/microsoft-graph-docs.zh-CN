---
title: 创建 userSource
description: 创建新的 userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9ff054926611c990f8db0a2f868ac3449708436f
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597511"
---
# <a name="create-usersource"></a><span data-ttu-id="927a5-103">创建 userSource</span><span class="sxs-lookup"><span data-stu-id="927a5-103">Create userSource</span></span>

<span data-ttu-id="927a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="927a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="927a5-105">创建新的 [userSource](../resources/usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="927a5-105">Create a new [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="927a5-106">权限</span><span class="sxs-lookup"><span data-stu-id="927a5-106">Permissions</span></span>

<span data-ttu-id="927a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="927a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="927a5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="927a5-109">Permission type</span></span>|<span data-ttu-id="927a5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="927a5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="927a5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="927a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="927a5-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="927a5-112">User.Read</span></span>|
|<span data-ttu-id="927a5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="927a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="927a5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="927a5-114">Not supported.</span></span>|
|<span data-ttu-id="927a5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="927a5-115">Application</span></span>|<span data-ttu-id="927a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="927a5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="927a5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="927a5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="927a5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="927a5-118">Request headers</span></span>

|<span data-ttu-id="927a5-119">名称</span><span class="sxs-lookup"><span data-stu-id="927a5-119">Name</span></span>|<span data-ttu-id="927a5-120">说明</span><span class="sxs-lookup"><span data-stu-id="927a5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="927a5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="927a5-121">Authorization</span></span>|<span data-ttu-id="927a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="927a5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="927a5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="927a5-124">Content-Type</span></span>|<span data-ttu-id="927a5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="927a5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="927a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="927a5-127">Request body</span></span>

<span data-ttu-id="927a5-128">在请求正文中，提供 [userSource](../resources/usersource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="927a5-128">In the request body, supply a JSON representation of the [userSource](../resources/usersource.md) object.</span></span>

<span data-ttu-id="927a5-129">下表显示创建 [userSource](../resources/usersource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="927a5-129">The following table shows the properties that are required when you create the [userSource](../resources/usersource.md).</span></span>

|<span data-ttu-id="927a5-130">属性</span><span class="sxs-lookup"><span data-stu-id="927a5-130">Property</span></span>|<span data-ttu-id="927a5-131">类型</span><span class="sxs-lookup"><span data-stu-id="927a5-131">Type</span></span>|<span data-ttu-id="927a5-132">Description</span><span class="sxs-lookup"><span data-stu-id="927a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="927a5-133">email</span><span class="sxs-lookup"><span data-stu-id="927a5-133">email</span></span>|<span data-ttu-id="927a5-134">String</span><span class="sxs-lookup"><span data-stu-id="927a5-134">String</span></span>|<span data-ttu-id="927a5-135">用户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="927a5-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="927a5-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="927a5-136">includedSources</span></span>|<span data-ttu-id="927a5-137">sourceType</span><span class="sxs-lookup"><span data-stu-id="927a5-137">sourceType</span></span>|<span data-ttu-id="927a5-138">指定要包含在此组中的源。</span><span class="sxs-lookup"><span data-stu-id="927a5-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="927a5-139">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="927a5-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="927a5-140">响应</span><span class="sxs-lookup"><span data-stu-id="927a5-140">Response</span></span>

<span data-ttu-id="927a5-141">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userSource](../resources/usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="927a5-141">If successful, this method returns a `201 Created` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="927a5-142">示例</span><span class="sxs-lookup"><span data-stu-id="927a5-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="927a5-143">请求</span><span class="sxs-lookup"><span data-stu-id="927a5-143">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="927a5-144">响应</span><span class="sxs-lookup"><span data-stu-id="927a5-144">Response</span></span>

<span data-ttu-id="927a5-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="927a5-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
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
