---
title: 删除 educationSynchronizationProfile
description: 删除学校数据同步配置文件中租户基于的标识符。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2aaa0d47bcc98c814ad525deb781ac7a7df28d87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512470"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="74ea0-103">删除 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="74ea0-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ea0-104">删除基于标识符为租户中学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="74ea0-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="74ea0-105">权限</span><span class="sxs-lookup"><span data-stu-id="74ea0-105">Permissions</span></span>
<span data-ttu-id="74ea0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74ea0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="74ea0-108">Permission type</span></span> | <span data-ttu-id="74ea0-109">权限</span><span class="sxs-lookup"><span data-stu-id="74ea0-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="74ea0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74ea0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74ea0-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74ea0-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="74ea0-112">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74ea0-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="74ea0-113">请求标头</span><span class="sxs-lookup"><span data-stu-id="74ea0-113">Request headers</span></span>
| <span data-ttu-id="74ea0-114">名称</span><span class="sxs-lookup"><span data-stu-id="74ea0-114">Name</span></span>       | <span data-ttu-id="74ea0-115">类型</span><span class="sxs-lookup"><span data-stu-id="74ea0-115">Type</span></span> | <span data-ttu-id="74ea0-116">说明</span><span class="sxs-lookup"><span data-stu-id="74ea0-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="74ea0-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="74ea0-117">Authorization</span></span>  | <span data-ttu-id="74ea0-118">string</span><span class="sxs-lookup"><span data-stu-id="74ea0-118">string</span></span>  | <span data-ttu-id="74ea0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74ea0-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="74ea0-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74ea0-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="74ea0-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="74ea0-122">Not supported.</span></span>|
|<span data-ttu-id="74ea0-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="74ea0-123">Application</span></span>|<span data-ttu-id="74ea0-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="74ea0-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74ea0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="74ea0-125">Request body</span></span>
<span data-ttu-id="74ea0-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74ea0-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="74ea0-127">响应</span><span class="sxs-lookup"><span data-stu-id="74ea0-127">Response</span></span>
<span data-ttu-id="74ea0-128">如果成功，此方法返回 `202 Accepted` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="74ea0-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ea0-129">示例</span><span class="sxs-lookup"><span data-stu-id="74ea0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74ea0-130">请求</span><span class="sxs-lookup"><span data-stu-id="74ea0-130">Request</span></span>
<span data-ttu-id="74ea0-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74ea0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="74ea0-132">响应</span><span class="sxs-lookup"><span data-stu-id="74ea0-132">Response</span></span>
<span data-ttu-id="74ea0-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="74ea0-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
