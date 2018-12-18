---
title: 权限
description: '将应用程序发布到 Microsoft 团队的应用程序目录。 '
author: nkramer
ms.openlocfilehash: 01d552a013b3d1324893bd775611e797253ff261
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335194"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="a7f07-103">将应用程序发布到组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="a7f07-103">Publish apps to your organization's app catalog</span></span>

> <span data-ttu-id="a7f07-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a7f07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7f07-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a7f07-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7f07-106">将[应用程序](../resources/teamsapp.md)发布到 Microsoft 团队的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="a7f07-106">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="a7f07-107">具体而言，此 API 将应用程序发布到组织的目录 （租户应用程序目录）;创建的资源将具有`distributionMethod`  =  `organization`。</span><span class="sxs-lookup"><span data-stu-id="a7f07-107">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7f07-108">权限</span><span class="sxs-lookup"><span data-stu-id="a7f07-108">Permissions</span></span>

<span data-ttu-id="a7f07-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="a7f07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="a7f07-111">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a7f07-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="a7f07-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7f07-112">Permission Type</span></span>                        | <span data-ttu-id="a7f07-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7f07-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="a7f07-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7f07-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7f07-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7f07-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="a7f07-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7f07-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7f07-117">不支持</span><span class="sxs-lookup"><span data-stu-id="a7f07-117">Not supported</span></span>|
| <span data-ttu-id="a7f07-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7f07-118">Application</span></span>                            | <span data-ttu-id="a7f07-119">不支持</span><span class="sxs-lookup"><span data-stu-id="a7f07-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7f07-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7f07-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="a7f07-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7f07-121">Request headers</span></span>

| <span data-ttu-id="a7f07-122">标头</span><span class="sxs-lookup"><span data-stu-id="a7f07-122">Header</span></span>        | <span data-ttu-id="a7f07-123">值</span><span class="sxs-lookup"><span data-stu-id="a7f07-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a7f07-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7f07-124">Authorization</span></span> | <span data-ttu-id="a7f07-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7f07-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7f07-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7f07-127">Content-Type</span></span>  | <span data-ttu-id="a7f07-128">应用程序/zip</span><span class="sxs-lookup"><span data-stu-id="a7f07-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7f07-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7f07-129">Request body</span></span>

<span data-ttu-id="a7f07-130">团队 Zip 清单负载。</span><span class="sxs-lookup"><span data-stu-id="a7f07-130">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="a7f07-131">团队应用程序 zip 文件，[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="a7f07-131">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="a7f07-132">无法创建应用程序的组织的组织中具有相同的清单另一个应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="a7f07-132">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="a7f07-133">响应</span><span class="sxs-lookup"><span data-stu-id="a7f07-133">Response</span></span>

<span data-ttu-id="a7f07-134">如果成功，此方法返回`200 OK`响应代码和[teamsCatalogApp](../resources/teamsapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a7f07-134">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="a7f07-135">示例</span><span class="sxs-lookup"><span data-stu-id="a7f07-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7f07-136">请求</span><span class="sxs-lookup"><span data-stu-id="a7f07-136">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="a7f07-137">有关如何创建的 Microsoft 团队应用程序 zip 文件的信息，请参阅[创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="a7f07-137">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="a7f07-138">响应</span><span class="sxs-lookup"><span data-stu-id="a7f07-138">Response</span></span>

```
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
