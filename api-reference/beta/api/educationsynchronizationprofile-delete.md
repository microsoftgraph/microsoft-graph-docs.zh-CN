---
title: 删除 educationSynchronizationProfile
description: 删除学校数据同步配置文件中租户基于的标识符。
author: mmast-msft
ms.openlocfilehash: b0287133d579915279e0f9a02bf49dd981ccf419
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343300"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="ebbdc-103">删除 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="ebbdc-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="ebbdc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebbdc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebbdc-106">删除基于标识符为租户中学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebbdc-107">权限</span><span class="sxs-lookup"><span data-stu-id="ebbdc-107">Permissions</span></span>
<span data-ttu-id="ebbdc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ebbdc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebbdc-110">Permission type</span></span> | <span data-ttu-id="ebbdc-111">权限</span><span class="sxs-lookup"><span data-stu-id="ebbdc-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ebbdc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebbdc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebbdc-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebbdc-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebbdc-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebbdc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ebbdc-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebbdc-115">Request headers</span></span>
| <span data-ttu-id="ebbdc-116">Name</span><span class="sxs-lookup"><span data-stu-id="ebbdc-116">Name</span></span>       | <span data-ttu-id="ebbdc-117">类型</span><span class="sxs-lookup"><span data-stu-id="ebbdc-117">Type</span></span> | <span data-ttu-id="ebbdc-118">说明</span><span class="sxs-lookup"><span data-stu-id="ebbdc-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ebbdc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebbdc-119">Authorization</span></span>  | <span data-ttu-id="ebbdc-120">string</span><span class="sxs-lookup"><span data-stu-id="ebbdc-120">string</span></span>  | <span data-ttu-id="ebbdc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="ebbdc-123">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ebbdc-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ebbdc-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-124">Not supported.</span></span>|
|<span data-ttu-id="ebbdc-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebbdc-125">Application</span></span>|<span data-ttu-id="ebbdc-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebbdc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebbdc-127">Request body</span></span>
<span data-ttu-id="ebbdc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ebbdc-129">响应</span><span class="sxs-lookup"><span data-stu-id="ebbdc-129">Response</span></span>
<span data-ttu-id="ebbdc-130">如果成功，此方法返回 `202 Accepted` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebbdc-131">示例</span><span class="sxs-lookup"><span data-stu-id="ebbdc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebbdc-132">请求</span><span class="sxs-lookup"><span data-stu-id="ebbdc-132">Request</span></span>
<span data-ttu-id="ebbdc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="ebbdc-134">响应</span><span class="sxs-lookup"><span data-stu-id="ebbdc-134">Response</span></span>
<span data-ttu-id="ebbdc-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebbdc-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
