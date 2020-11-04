---
title: 发布 teamsapp
description: '将应用程序发布到 Microsoft 团队应用程序目录。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8108960cc6ad33b5e5b5282b049194932a804d53
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848729"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="6e449-103">发布 teamsapp</span><span class="sxs-lookup"><span data-stu-id="6e449-103">Publish teamsapp</span></span>

<span data-ttu-id="6e449-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e449-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e449-105">将 [应用程序](../resources/teamsapp.md) 发布到 Microsoft 团队应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="6e449-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="6e449-106">具体而言，此 API 会将应用程序发布到 (租户应用程序目录) 的组织目录中。创建的资源的 **distributionMethod** 属性值为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="6e449-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e449-107">权限</span><span class="sxs-lookup"><span data-stu-id="6e449-107">Permissions</span></span>

<span data-ttu-id="6e449-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="6e449-110">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6e449-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="6e449-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e449-111">Permission Type</span></span>                        | <span data-ttu-id="6e449-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e449-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="6e449-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e449-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e449-114">AppCatalog、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="6e449-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="6e449-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e449-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e449-116">不支持</span><span class="sxs-lookup"><span data-stu-id="6e449-116">Not supported</span></span>|
| <span data-ttu-id="6e449-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e449-117">Application</span></span>                            | <span data-ttu-id="6e449-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e449-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e449-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e449-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="6e449-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e449-120">Request headers</span></span>

| <span data-ttu-id="6e449-121">标头</span><span class="sxs-lookup"><span data-stu-id="6e449-121">Header</span></span>        | <span data-ttu-id="6e449-122">值</span><span class="sxs-lookup"><span data-stu-id="6e449-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="6e449-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e449-123">Authorization</span></span> | <span data-ttu-id="6e449-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e449-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e449-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e449-126">Content-Type</span></span>  | <span data-ttu-id="6e449-127">application/zip。</span><span class="sxs-lookup"><span data-stu-id="6e449-127">application/zip.</span></span> <span data-ttu-id="6e449-128">必填。</span><span class="sxs-lookup"><span data-stu-id="6e449-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e449-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e449-129">Request body</span></span>

<span data-ttu-id="6e449-130">在请求正文中，包括团队 zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="6e449-130">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="6e449-131">有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="6e449-131">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="6e449-132">应用程序目录中的每个应用必须具有唯一的清单 id。</span><span class="sxs-lookup"><span data-stu-id="6e449-132">Each app in the app catalog must have a unique manifest id.</span></span>

## <a name="response"></a><span data-ttu-id="6e449-133">响应</span><span class="sxs-lookup"><span data-stu-id="6e449-133">Response</span></span>

<span data-ttu-id="6e449-134">如果成功，此方法将返回 `200 OK` 响应代码和 [teamsApp](../resources/teamsapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e449-134">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="6e449-135">示例</span><span class="sxs-lookup"><span data-stu-id="6e449-135">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="6e449-136">示例1：将应用程序发布到应用程序目录</span><span class="sxs-lookup"><span data-stu-id="6e449-136">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="6e449-137">请求</span><span class="sxs-lookup"><span data-stu-id="6e449-137">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="6e449-138">有关如何创建 Microsoft 团队应用程序 zip 文件的信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="6e449-138">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="6e449-139">响应</span><span class="sxs-lookup"><span data-stu-id="6e449-139">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
