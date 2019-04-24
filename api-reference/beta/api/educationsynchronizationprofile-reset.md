---
title: 在 educationSynchronizationProfile 上重置同步
description: 在租户中重置特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 502eb8d7afdc61926a024b7ddfbac5383a146622
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457501"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="4d399-103">在 educationSynchronizationProfile 上重置同步</span><span class="sxs-lookup"><span data-stu-id="4d399-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d399-104">在租户中重置特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="4d399-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="4d399-105">**注意:** 此操作将导致重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="4d399-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="4d399-106">遇到的任何错误都将被删除。</span><span class="sxs-lookup"><span data-stu-id="4d399-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="4d399-107">将不会从 azure Active Directory (azure AD) 中删除任何数据。</span><span class="sxs-lookup"><span data-stu-id="4d399-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="4d399-108">权限</span><span class="sxs-lookup"><span data-stu-id="4d399-108">Permissions</span></span>
<span data-ttu-id="4d399-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d399-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d399-111">Permission type</span></span> | <span data-ttu-id="4d399-112">权限</span><span class="sxs-lookup"><span data-stu-id="4d399-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4d399-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d399-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4d399-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d399-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="4d399-115">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="4d399-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4d399-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d399-116">Not supported.</span></span>|
|<span data-ttu-id="4d399-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d399-117">Application</span></span>|<span data-ttu-id="4d399-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d399-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d399-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d399-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="4d399-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d399-120">Request headers</span></span>
| <span data-ttu-id="4d399-121">名称</span><span class="sxs-lookup"><span data-stu-id="4d399-121">Name</span></span>       | <span data-ttu-id="4d399-122">类型</span><span class="sxs-lookup"><span data-stu-id="4d399-122">Type</span></span> | <span data-ttu-id="4d399-123">说明</span><span class="sxs-lookup"><span data-stu-id="4d399-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4d399-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d399-124">Authorization</span></span>  | <span data-ttu-id="4d399-125">string</span><span class="sxs-lookup"><span data-stu-id="4d399-125">string</span></span>  | <span data-ttu-id="4d399-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d399-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d399-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d399-128">Request body</span></span>
<span data-ttu-id="4d399-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d399-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4d399-130">响应</span><span class="sxs-lookup"><span data-stu-id="4d399-130">Response</span></span>
<span data-ttu-id="4d399-131">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4d399-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d399-132">示例</span><span class="sxs-lookup"><span data-stu-id="4d399-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d399-133">请求</span><span class="sxs-lookup"><span data-stu-id="4d399-133">Request</span></span>
<span data-ttu-id="4d399-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d399-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="4d399-135">响应</span><span class="sxs-lookup"><span data-stu-id="4d399-135">Response</span></span>

<span data-ttu-id="4d399-136">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="4d399-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
