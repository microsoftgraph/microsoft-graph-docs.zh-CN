---
title: 删除 educationSynchronizationProfile
description: 删除学校数据同步配置文件中租户基于的标识符。
ms.openlocfilehash: 829b723b48eb9a15750bc9d0e00ba50d432e8ab6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046106"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="0c7a6-103">删除 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="0c7a6-103">Delete a educationSynchronizationProfile</span></span>

> <span data-ttu-id="0c7a6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c7a6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c7a6-106">删除基于标识符为租户中学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-106">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c7a6-107">权限</span><span class="sxs-lookup"><span data-stu-id="0c7a6-107">Permissions</span></span>
<span data-ttu-id="0c7a6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c7a6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c7a6-110">Permission type</span></span> | <span data-ttu-id="0c7a6-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="0c7a6-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="0c7a6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c7a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c7a6-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c7a6-113">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c7a6-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c7a6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0c7a6-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c7a6-115">Request headers</span></span>
| <span data-ttu-id="0c7a6-116">名称</span><span class="sxs-lookup"><span data-stu-id="0c7a6-116">Name</span></span>       | <span data-ttu-id="0c7a6-117">类型</span><span class="sxs-lookup"><span data-stu-id="0c7a6-117">Type</span></span> | <span data-ttu-id="0c7a6-118">说明</span><span class="sxs-lookup"><span data-stu-id="0c7a6-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0c7a6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c7a6-119">Authorization</span></span>  | <span data-ttu-id="0c7a6-120">string</span><span class="sxs-lookup"><span data-stu-id="0c7a6-120">string</span></span>  | <span data-ttu-id="0c7a6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-p103">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="0c7a6-123">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="0c7a6-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0c7a6-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-124">Not supported.</span></span>|
|<span data-ttu-id="0c7a6-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c7a6-125">Application</span></span>|<span data-ttu-id="0c7a6-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-126">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c7a6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c7a6-127">Request body</span></span>
<span data-ttu-id="0c7a6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0c7a6-129">响应</span><span class="sxs-lookup"><span data-stu-id="0c7a6-129">Response</span></span>
<span data-ttu-id="0c7a6-130">如果成功，此方法返回 `202 Accepted` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-130">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c7a6-131">示例</span><span class="sxs-lookup"><span data-stu-id="0c7a6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c7a6-132">请求</span><span class="sxs-lookup"><span data-stu-id="0c7a6-132">Request</span></span>
<span data-ttu-id="0c7a6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="0c7a6-134">响应</span><span class="sxs-lookup"><span data-stu-id="0c7a6-134">Response</span></span>
<span data-ttu-id="0c7a6-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0c7a6-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
