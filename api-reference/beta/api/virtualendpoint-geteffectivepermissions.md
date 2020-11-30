---
title: virtualEndpoint： getEffectivePermissions
description: '**GetEffectivePermissions 是一种 retrives 当前已通过身份验证的用户的有效权限的功能，可帮助 UX 隐藏或禁用当前用户无权访问的内容。**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78b58c5ea00e1b170d831a91f5dc3ff1569bd0d7
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378323"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="0d54b-103">virtualEndpoint： getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="0d54b-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="0d54b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d54b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d54b-105">查看当前经过身份验证的用户的有效权限。</span><span class="sxs-lookup"><span data-stu-id="0d54b-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="0d54b-106">GetEffectivePermissions 是一种 retrives 当前已通过身份验证的用户的有效权限的功能，可帮助 UX 隐藏或禁用当前用户无权访问的内容。</span><span class="sxs-lookup"><span data-stu-id="0d54b-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d54b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0d54b-107">Permissions</span></span>

<span data-ttu-id="0d54b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d54b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d54b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d54b-110">Permission type</span></span>|<span data-ttu-id="0d54b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0d54b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d54b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d54b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d54b-113">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="0d54b-113">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="0d54b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d54b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d54b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d54b-115">Not supported.</span></span>|
|<span data-ttu-id="0d54b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d54b-116">Application</span></span>| <span data-ttu-id="0d54b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d54b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d54b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d54b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="0d54b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d54b-119">Request headers</span></span>

| <span data-ttu-id="0d54b-120">名称</span><span class="sxs-lookup"><span data-stu-id="0d54b-120">Name</span></span>          | <span data-ttu-id="0d54b-121">说明</span><span class="sxs-lookup"><span data-stu-id="0d54b-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0d54b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d54b-122">Authorization</span></span> | <span data-ttu-id="0d54b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d54b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d54b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d54b-125">Request body</span></span>

<span data-ttu-id="0d54b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d54b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d54b-127">响应</span><span class="sxs-lookup"><span data-stu-id="0d54b-127">Response</span></span>

<span data-ttu-id="0d54b-128">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="0d54b-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="0d54b-129">如果用户具有完全权限，则响应为 `["*"]` 。</span><span class="sxs-lookup"><span data-stu-id="0d54b-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="0d54b-130">示例</span><span class="sxs-lookup"><span data-stu-id="0d54b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d54b-131">请求</span><span class="sxs-lookup"><span data-stu-id="0d54b-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```

### <a name="response"></a><span data-ttu-id="0d54b-132">响应</span><span class="sxs-lookup"><span data-stu-id="0d54b-132">Response</span></span>

<span data-ttu-id="0d54b-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0d54b-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    "Microsoft.CloudPC/CloudPCs/Read"
  ]
}
```
