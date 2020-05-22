---
title: 权限
description: '更新之前发布到 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f03ee786a5c8f46a65d7af7c70d771346242e41
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345756"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="8a3e0-103">更新发布到组织的应用程序目录的应用程序</span><span class="sxs-lookup"><span data-stu-id="8a3e0-103">Update apps published to your organization's app catalog</span></span>

<span data-ttu-id="8a3e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a3e0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8a3e0-105">更新之前发布到 Microsoft 团队应用程序目录的[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="8a3e0-106">此 API 专门更新发布到您的组织的应用程序目录（租户应用程序目录）的应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-106">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>
<span data-ttu-id="8a3e0-107">若要发布到您的组织的应用程序目录，请 `organization` 在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-107">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a3e0-108">权限</span><span class="sxs-lookup"><span data-stu-id="8a3e0-108">Permissions</span></span>

<span data-ttu-id="8a3e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="8a3e0-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="8a3e0-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a3e0-112">Permission Type</span></span>                        | <span data-ttu-id="8a3e0-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a3e0-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="8a3e0-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a3e0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a3e0-115">AppCatalog、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="8a3e0-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a3e0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a3e0-117">不支持</span><span class="sxs-lookup"><span data-stu-id="8a3e0-117">Not supported</span></span>|
| <span data-ttu-id="8a3e0-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a3e0-118">Application</span></span>                            | <span data-ttu-id="8a3e0-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a3e0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a3e0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a3e0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a3e0-121">Request headers</span></span>

| <span data-ttu-id="8a3e0-122">标头</span><span class="sxs-lookup"><span data-stu-id="8a3e0-122">Header</span></span>        | <span data-ttu-id="8a3e0-123">值</span><span class="sxs-lookup"><span data-stu-id="8a3e0-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="8a3e0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a3e0-124">Authorization</span></span> | <span data-ttu-id="8a3e0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a3e0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a3e0-127">Content-Type</span></span>  | <span data-ttu-id="8a3e0-128">application/zip</span><span class="sxs-lookup"><span data-stu-id="8a3e0-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a3e0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a3e0-129">Request body</span></span>

<span data-ttu-id="8a3e0-130">团队 Zip 清单有效负载：对于团队应用程序 Zip 文件，[请参阅创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="8a3e0-130">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="8a3e0-131">**注意：** 使用从[列表已发布的应用程序](./teamsapp-list.md)调用中返回的 ID 引用要更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-131">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span>
<span data-ttu-id="8a3e0-132">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="8a3e0-132">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="8a3e0-133">响应</span><span class="sxs-lookup"><span data-stu-id="8a3e0-133">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="8a3e0-134">示例</span><span class="sxs-lookup"><span data-stu-id="8a3e0-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a3e0-135">请求</span><span class="sxs-lookup"><span data-stu-id="8a3e0-135">Request</span></span>

```
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="8a3e0-136">对于团队应用程序 zip 文件，[请参阅创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="8a3e0-136">For Teams application zip file [see Create app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="8a3e0-137">响应</span><span class="sxs-lookup"><span data-stu-id="8a3e0-137">Response</span></span>

```
HTTP/1.1 204 No Content
```
