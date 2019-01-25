---
title: 重置 sync educationSynchronizationProfile 上
description: 重置为租户中的特定学校数据同步配置文件同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 502eb8d7afdc61926a024b7ddfbac5383a146622
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520408"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="a7887-103">重置 sync educationSynchronizationProfile 上</span><span class="sxs-lookup"><span data-stu-id="a7887-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7887-104">重置为租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="a7887-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="a7887-105">**注意：** 此操作将导致同步重新启动。</span><span class="sxs-lookup"><span data-stu-id="a7887-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="a7887-106">遇到的任何错误都将被删除。</span><span class="sxs-lookup"><span data-stu-id="a7887-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="a7887-107">将从 Azure Active Directory (Azure AD) 中不删除任何数据。</span><span class="sxs-lookup"><span data-stu-id="a7887-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a7887-108">权限</span><span class="sxs-lookup"><span data-stu-id="a7887-108">Permissions</span></span>
<span data-ttu-id="a7887-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7887-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7887-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7887-111">Permission type</span></span> | <span data-ttu-id="a7887-112">权限</span><span class="sxs-lookup"><span data-stu-id="a7887-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a7887-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7887-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a7887-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7887-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="a7887-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7887-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a7887-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7887-116">Not supported.</span></span>|
|<span data-ttu-id="a7887-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7887-117">Application</span></span>|<span data-ttu-id="a7887-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7887-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7887-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7887-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="a7887-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7887-120">Request headers</span></span>
| <span data-ttu-id="a7887-121">名称</span><span class="sxs-lookup"><span data-stu-id="a7887-121">Name</span></span>       | <span data-ttu-id="a7887-122">类型</span><span class="sxs-lookup"><span data-stu-id="a7887-122">Type</span></span> | <span data-ttu-id="a7887-123">说明</span><span class="sxs-lookup"><span data-stu-id="a7887-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7887-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7887-124">Authorization</span></span>  | <span data-ttu-id="a7887-125">string</span><span class="sxs-lookup"><span data-stu-id="a7887-125">string</span></span>  | <span data-ttu-id="a7887-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7887-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7887-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7887-128">Request body</span></span>
<span data-ttu-id="a7887-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7887-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a7887-130">响应</span><span class="sxs-lookup"><span data-stu-id="a7887-130">Response</span></span>
<span data-ttu-id="a7887-131">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a7887-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7887-132">示例</span><span class="sxs-lookup"><span data-stu-id="a7887-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7887-133">请求</span><span class="sxs-lookup"><span data-stu-id="a7887-133">Request</span></span>
<span data-ttu-id="a7887-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a7887-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="a7887-135">响应</span><span class="sxs-lookup"><span data-stu-id="a7887-135">Response</span></span>

<span data-ttu-id="a7887-136">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="a7887-136">There is no response body.</span></span>

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
