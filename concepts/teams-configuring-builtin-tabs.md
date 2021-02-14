---
title: 在 Microsoft Teams 中配置内置选项卡类型
description: 使用 Microsoft Graph API 创建或配置 Microsoft Teams 选项卡
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 13f0719a63cc604a8ffb9b77540e346837f1a031
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239441"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a><span data-ttu-id="2337c-103">在 Microsoft Teams 中配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="2337c-103">Configuring the built-in tab types in Microsoft Teams</span></span>

<span data-ttu-id="2337c-104">若要使用 Microsoft Graph API [创建](/graph/api/channel-post-tabs?view=graph-rest-1.0)或[配置](/graph/api/channel-patch-tabs?view=graph-rest-1.0) Microsoft Teams 选项卡，你需要知道应用的 `teamsAppId` 以及为该类应用提供的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl`。</span><span class="sxs-lookup"><span data-stu-id="2337c-104">To [create](/graph/api/channel-post-tabs?view=graph-rest-1.0) or [configure](/graph/api/channel-patch-tabs?view=graph-rest-1.0) a Microsoft Teams tab using Microsoft Graph APIs, you need to know the `teamsAppId` of the app, and the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` to provide for that kind of app.</span></span>
<span data-ttu-id="2337c-105">本文介绍如何获取内置选项卡类型的值。</span><span class="sxs-lookup"><span data-stu-id="2337c-105">This article explains how to get those values for the built-in tab types.</span></span>

## <a name="custom-tabs"></a><span data-ttu-id="2337c-106">自定义选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-106">Custom tabs</span></span>

<span data-ttu-id="2337c-107">若要使用 Microsoft Graph 配置与所编写的[选项卡提供程序](/microsoftteams/platform/concepts/tabs/tabs-overview)关联的选项卡，请标识 `entityId`、`contentUrl`、`removeUrl` 以及应用的[配置 UI 提供给 Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest) 的 `websiteUrl`，并将相同的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl` 值传递给 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="2337c-107">To use Microsoft Graph to configure a tab associated with a [tab provider](/microsoftteams/platform/concepts/tabs/tabs-overview) that you wrote, identify the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` that the app's [configuration UI provides to Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest), and pass the same `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` values to Microsoft Graph.</span></span>

<span data-ttu-id="2337c-108">`teamsAppId` 与 [Microsoft Teams 的应用清单架构](/microsoftteams/platform/resources/schema/manifest-schema)中的 `id` 相同。</span><span class="sxs-lookup"><span data-stu-id="2337c-108">The `teamsAppId` is the same as the `id` in the [app manifest schema for Microsoft Teams](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>

## <a name="website-tabs"></a><span data-ttu-id="2337c-109">网站选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-109">Website tabs</span></span>

<span data-ttu-id="2337c-110">对于网站选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.web`。</span><span class="sxs-lookup"><span data-stu-id="2337c-110">For website tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.web`.</span></span> <span data-ttu-id="2337c-111">以下是配置。</span><span class="sxs-lookup"><span data-stu-id="2337c-111">The following is the configuration.</span></span>

| <span data-ttu-id="2337c-112">属性</span><span class="sxs-lookup"><span data-stu-id="2337c-112">Property</span></span>   | <span data-ttu-id="2337c-113">类型</span><span class="sxs-lookup"><span data-stu-id="2337c-113">Type</span></span>        | <span data-ttu-id="2337c-114">说明</span><span class="sxs-lookup"><span data-stu-id="2337c-114">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="2337c-115">entityId</span><span class="sxs-lookup"><span data-stu-id="2337c-115">entityId</span></span>   | <span data-ttu-id="2337c-116">string</span><span class="sxs-lookup"><span data-stu-id="2337c-116">string</span></span>      | <span data-ttu-id="2337c-117">Null</span><span class="sxs-lookup"><span data-stu-id="2337c-117">Null</span></span>                                                     |
| <span data-ttu-id="2337c-118">contentUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-118">contentUrl</span></span> | <span data-ttu-id="2337c-119">string</span><span class="sxs-lookup"><span data-stu-id="2337c-119">string</span></span>      | <span data-ttu-id="2337c-120">网站的 URL</span><span class="sxs-lookup"><span data-stu-id="2337c-120">URL of the website</span></span>                                       |
| <span data-ttu-id="2337c-121">removeUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-121">removeUrl</span></span>  | <span data-ttu-id="2337c-122">string</span><span class="sxs-lookup"><span data-stu-id="2337c-122">string</span></span>      | <span data-ttu-id="2337c-123">Null</span><span class="sxs-lookup"><span data-stu-id="2337c-123">Null</span></span>                                                     |
| <span data-ttu-id="2337c-124">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-124">websiteUrl</span></span> | <span data-ttu-id="2337c-125">string</span><span class="sxs-lookup"><span data-stu-id="2337c-125">string</span></span>      | <span data-ttu-id="2337c-126">网站的 URL</span><span class="sxs-lookup"><span data-stu-id="2337c-126">URL of the website</span></span>                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a><span data-ttu-id="2337c-127">Word、Excel、PowerPoint 和 PDF 选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-127">Word, Excel, PowerPoint, and PDF tabs</span></span>

<span data-ttu-id="2337c-128">下表列出了每个应用的 `teamsAppId`。</span><span class="sxs-lookup"><span data-stu-id="2337c-128">The following table lists the `teamsAppId` for each app.</span></span>

| <span data-ttu-id="2337c-129">应用</span><span class="sxs-lookup"><span data-stu-id="2337c-129">App</span></span>   | <span data-ttu-id="2337c-130">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="2337c-130">teamsAppId</span></span> | <span data-ttu-id="2337c-131">类型（扩展名）</span><span class="sxs-lookup"><span data-stu-id="2337c-131">type (extension)</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="2337c-132">Word</span><span class="sxs-lookup"><span data-stu-id="2337c-132">Word</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| <span data-ttu-id="2337c-133">Excel</span><span class="sxs-lookup"><span data-stu-id="2337c-133">Excel</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| <span data-ttu-id="2337c-134">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="2337c-134">PowerPoint</span></span>  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| <span data-ttu-id="2337c-135">PDF</span><span class="sxs-lookup"><span data-stu-id="2337c-135">PDF</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

<span data-ttu-id="2337c-136">以下是配置。</span><span class="sxs-lookup"><span data-stu-id="2337c-136">The following is the configuration.</span></span>

| <span data-ttu-id="2337c-137">属性</span><span class="sxs-lookup"><span data-stu-id="2337c-137">Property</span></span>   | <span data-ttu-id="2337c-138">类型</span><span class="sxs-lookup"><span data-stu-id="2337c-138">Type</span></span>        | <span data-ttu-id="2337c-139">说明</span><span class="sxs-lookup"><span data-stu-id="2337c-139">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="2337c-140">entityId</span><span class="sxs-lookup"><span data-stu-id="2337c-140">entityId</span></span>   | <span data-ttu-id="2337c-141">字符串</span><span class="sxs-lookup"><span data-stu-id="2337c-141">string</span></span>      | <span data-ttu-id="2337c-142">文件的 sourceDoc ID。</span><span class="sxs-lookup"><span data-stu-id="2337c-142">The sourceDoc ID of the file.</span></span> <span data-ttu-id="2337c-143">通过打开 SharePoint 中文件并查看地址栏即可找到 – URL 将有一个`sourcedoc=%7B{sourceDocId}%7D`子句。</span><span class="sxs-lookup"><span data-stu-id="2337c-143">You can find this by opening the file in SharePoint and looking at the address bar – the URL will have a `sourcedoc=%7B{sourceDocId}%7D` clause.</span></span> <span data-ttu-id="2337c-144">此外还可从文档 SharePoint 驱动器项的 webUrl 派生。</span><span class="sxs-lookup"><span data-stu-id="2337c-144">You can also derive this from the webUrl of the SharePoint drive item for the document.</span></span> <span data-ttu-id="2337c-145">有关详细信息，请参阅 [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="2337c-145">For details, see [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="2337c-146">contentUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-146">contentUrl</span></span> | <span data-ttu-id="2337c-147">字符串</span><span class="sxs-lookup"><span data-stu-id="2337c-147">string</span></span>      | <span data-ttu-id="2337c-148">`{folder-webUrl}/{item-name}` 格式文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="2337c-148">The URL of file in the format `{folder-webUrl}/{item-name}`.</span></span> <span data-ttu-id="2337c-149">{folder-webUrl} 是包含文件的 SharePoint 文件夹 webUrl，通过打开 SharePoint 中文件并查看地址栏，或使用 [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta) 的 webUrl 属性即可找到该文件。</span><span class="sxs-lookup"><span data-stu-id="2337c-149">{folder-webUrl} is the webUrl of the SharePoint folder containing the file, which can be found by opening the file in SharePoint and looking at the address bar, or by using the webUrl property from [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> <span data-ttu-id="2337c-150">{item-name} 是文件名（例如 file.docx），也就是 [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta) 中的 `name` 属性。</span><span class="sxs-lookup"><span data-stu-id="2337c-150">{item-name} is the file name (for example, file.docx), which is the `name` property in [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="2337c-151">removeUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-151">removeUrl</span></span>  | <span data-ttu-id="2337c-152">string</span><span class="sxs-lookup"><span data-stu-id="2337c-152">string</span></span>      | <span data-ttu-id="2337c-153">Null</span><span class="sxs-lookup"><span data-stu-id="2337c-153">Null</span></span>                                                     |
| <span data-ttu-id="2337c-154">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-154">websiteUrl</span></span> | <span data-ttu-id="2337c-155">string</span><span class="sxs-lookup"><span data-stu-id="2337c-155">string</span></span>      | <span data-ttu-id="2337c-156">Null</span><span class="sxs-lookup"><span data-stu-id="2337c-156">Null</span></span>                                       |

### <a name="example-create-a-configured-word-tab"></a><span data-ttu-id="2337c-157">示例： 创建一个配置好的 Word 选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-157">Example: Create a configured Word tab</span></span>

<span data-ttu-id="2337c-158">以下示例将新建一个配置好的 Word 选项卡。</span><span class="sxs-lookup"><span data-stu-id="2337c-158">The following example creates a configured Word tab.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
  "displayName": "word",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.file.staticviewer.word",
  "configuration": {
     "entityId": "115A90F4-AC9C-4F79-9837-36D1EFB3BE08",
     "contentUrl": "https://m365x165177.sharepoint.com/sites/4NewCloneWithClonableParts/Shared%20Documents/General/Employee Handbook.docx",
     "removeUrl": null,
     "websiteUrl": null
  }
}
```

## <a name="document-library-tabs"></a><span data-ttu-id="2337c-159">文档库选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-159">Document library tabs</span></span>

<span data-ttu-id="2337c-160">对于文档库选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.files.sharepoint`。</span><span class="sxs-lookup"><span data-stu-id="2337c-160">For document library tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.files.sharepoint`.</span></span> <span data-ttu-id="2337c-161">以下是配置。</span><span class="sxs-lookup"><span data-stu-id="2337c-161">The following is the configuration.</span></span>

| <span data-ttu-id="2337c-162">属性</span><span class="sxs-lookup"><span data-stu-id="2337c-162">Property</span></span>   | <span data-ttu-id="2337c-163">类型</span><span class="sxs-lookup"><span data-stu-id="2337c-163">Type</span></span>        | <span data-ttu-id="2337c-164">说明</span><span class="sxs-lookup"><span data-stu-id="2337c-164">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="2337c-165">entityId</span><span class="sxs-lookup"><span data-stu-id="2337c-165">entityId</span></span>   | <span data-ttu-id="2337c-166">string</span><span class="sxs-lookup"><span data-stu-id="2337c-166">string</span></span>      | <span data-ttu-id="2337c-167">空字符串 ("") </span><span class="sxs-lookup"><span data-stu-id="2337c-167">Empty string ("")</span></span>                                        |
| <span data-ttu-id="2337c-168">contentUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-168">contentUrl</span></span> | <span data-ttu-id="2337c-169">string</span><span class="sxs-lookup"><span data-stu-id="2337c-169">string</span></span>      | <span data-ttu-id="2337c-170">文档库的根文件夹的 URL。</span><span class="sxs-lookup"><span data-stu-id="2337c-170">The URL of the root folder of the document library.</span></span> <span data-ttu-id="2337c-171">您可以通过在浏览器中打开 SharePoint 文件夹、复制 URL 以及删除"/Forms/AllItems.aspx"以及之后的所有内容来查找此 URL。</span><span class="sxs-lookup"><span data-stu-id="2337c-171">You can find this URL by opening the SharePoint folder in your browser, copying the URL, and deleting "/Forms/AllItems.aspx" and everything after that.</span></span> |
| <span data-ttu-id="2337c-172">removeUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-172">removeUrl</span></span>  | <span data-ttu-id="2337c-173">string</span><span class="sxs-lookup"><span data-stu-id="2337c-173">string</span></span>      | <span data-ttu-id="2337c-174">Null</span><span class="sxs-lookup"><span data-stu-id="2337c-174">Null</span></span>                                                     |
| <span data-ttu-id="2337c-175">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="2337c-175">websiteUrl</span></span> | <span data-ttu-id="2337c-176">string</span><span class="sxs-lookup"><span data-stu-id="2337c-176">string</span></span>      | <span data-ttu-id="2337c-177">Null</span><span class="sxs-lookup"><span data-stu-id="2337c-177">Null</span></span>                                                     |

### <a name="example-create-a-configured-document-library-tab"></a><span data-ttu-id="2337c-178">示例：创建配置的文档库选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-178">Example: Create a configured document library tab</span></span>

<span data-ttu-id="2337c-179">以下示例创建一个已配置的文档库选项卡。</span><span class="sxs-lookup"><span data-stu-id="2337c-179">The following example creates a configured document library tab.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
    "displayName": "Document%20Library1",
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.files.sharepoint",
    "configuration": {
        "entityId": "",
        "contentUrl": "https://microsoft.sharepoint.com/teams/WWWtest/Shared%20Documents",
        "removeUrl": null,
        "websiteUrl": null
    }
}
```

## <a name="wiki-tabs"></a><span data-ttu-id="2337c-180">Wiki 选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-180">Wiki tabs</span></span>

<span data-ttu-id="2337c-181">对于 wiki 选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.wiki`。</span><span class="sxs-lookup"><span data-stu-id="2337c-181">For wiki tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.wiki`.</span></span>
<span data-ttu-id="2337c-182">Wiki 选项卡不支持通过 Microsoft Graph 进行配置。</span><span class="sxs-lookup"><span data-stu-id="2337c-182">Wiki tabs do not support configuration through Microsoft Graph.</span></span>
<span data-ttu-id="2337c-183">但是请注意，没有太多要配置的内容 -在未配置的 Wiki 选项卡中，第一个用户只需选择"设置" **选项卡来配置** 它。</span><span class="sxs-lookup"><span data-stu-id="2337c-183">Note, however, that there isn't much to configure - in an unconfigured wiki tab, the first user just needs to select **Set up tab** to configure it.</span></span>

## <a name="planner-tabs"></a><span data-ttu-id="2337c-184">规划器选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-184">Planner tabs</span></span>

<span data-ttu-id="2337c-185">对于 Planner 选项卡， `teamsAppId` 为 `com.microsoft.teamspace.tab.planner` 。</span><span class="sxs-lookup"><span data-stu-id="2337c-185">For Planner tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.planner`.</span></span> <span data-ttu-id="2337c-186">配置不受支持。</span><span class="sxs-lookup"><span data-stu-id="2337c-186">Configuration is not supported.</span></span>

## <a name="microsoft-stream-tabs"></a><span data-ttu-id="2337c-187">Microsoft Stream 选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-187">Microsoft Stream tabs</span></span>

<span data-ttu-id="2337c-188">对于 Microsoft Stream 选项卡，`teamsAppId` 为 `com.microsoftstream.embed.skypeteamstab`。</span><span class="sxs-lookup"><span data-stu-id="2337c-188">For Microsoft Stream tabs, the `teamsAppId` is `com.microsoftstream.embed.skypeteamstab`.</span></span> <span data-ttu-id="2337c-189">配置不受支持。</span><span class="sxs-lookup"><span data-stu-id="2337c-189">Configuration is not supported.</span></span>

## <a name="microsoft-forms-tabs"></a><span data-ttu-id="2337c-190">Microsoft Forms 选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-190">Microsoft Forms tabs</span></span>

<span data-ttu-id="2337c-191">对于 Microsoft Forms 选项卡，`teamsAppId` 为 `81fef3a6-72aa-4648-a763-de824aeafb7d`。</span><span class="sxs-lookup"><span data-stu-id="2337c-191">For Microsoft Forms tabs, the `teamsAppId` is `81fef3a6-72aa-4648-a763-de824aeafb7d`.</span></span>
<span data-ttu-id="2337c-192">配置不受支持。</span><span class="sxs-lookup"><span data-stu-id="2337c-192">Configuration is not supported.</span></span>

## <a name="onenote-tabs"></a><span data-ttu-id="2337c-193">OneNote 选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-193">OneNote tabs</span></span>

<span data-ttu-id="2337c-194">对于 OneNote 选项卡，`teamsAppId` 为 `0d820ecd-def2-4297-adad-78056cde7c78`。</span><span class="sxs-lookup"><span data-stu-id="2337c-194">For OneNote tabs, the `teamsAppId` is `0d820ecd-def2-4297-adad-78056cde7c78`.</span></span> <span data-ttu-id="2337c-195">配置不受支持。</span><span class="sxs-lookup"><span data-stu-id="2337c-195">Configuration is not supported.</span></span>

## <a name="power-bi-tabs"></a><span data-ttu-id="2337c-196">Power BI 选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-196">Power BI tabs</span></span>

<span data-ttu-id="2337c-197">对于 Power BI 选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.powerbi`。</span><span class="sxs-lookup"><span data-stu-id="2337c-197">For Power BI tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.powerbi`.</span></span>
<span data-ttu-id="2337c-198">配置不受支持。</span><span class="sxs-lookup"><span data-stu-id="2337c-198">Configuration is not supported.</span></span>

## <a name="sharepoint-page-and-list-tabs"></a><span data-ttu-id="2337c-199">SharePoint 页和列表选项卡</span><span class="sxs-lookup"><span data-stu-id="2337c-199">SharePoint page and list tabs</span></span>

<span data-ttu-id="2337c-200">对于 SharePoint 页和列表选项卡，`teamsAppId` 为 `2a527703-1f6f-4559-a332-d8a7d288cd88`。</span><span class="sxs-lookup"><span data-stu-id="2337c-200">For SharePoint page and list tabs, the `teamsAppId` is `2a527703-1f6f-4559-a332-d8a7d288cd88`.</span></span>
<span data-ttu-id="2337c-201">配置不受支持。</span><span class="sxs-lookup"><span data-stu-id="2337c-201">Configuration is not supported.</span></span>
<span data-ttu-id="2337c-202">若你想要配置选项卡，请考虑使用网站选项卡。</span><span class="sxs-lookup"><span data-stu-id="2337c-202">If you want to configure the tab, consider using a Website tab.</span></span>
