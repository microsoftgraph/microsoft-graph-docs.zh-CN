---
title: 在 Microsoft Teams 中配置内置选项卡类型
description: 使用 Microsoft Graph API 创建或配置 Microsoft Teams 选项卡
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ffe2799f557b12dd72fa72e6bf8b20f72f507647
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345987"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a><span data-ttu-id="e11b0-103">在 Microsoft Teams 中配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="e11b0-103">Configuring the built-in tab types in Microsoft Teams</span></span>

<span data-ttu-id="e11b0-104">若要使用 Microsoft Graph API [创建](/graph/api/teamstab-add?view=graph-rest-beta)或[配置](/graph/api/teamstab-update?view=graph-rest-beta) Microsoft Teams 选项卡，你需要知道应用的 `teamsAppId` 以及为该类应用提供的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl`。</span><span class="sxs-lookup"><span data-stu-id="e11b0-104">To [create](/graph/api/teamstab-add?view=graph-rest-beta) or [configure](/graph/api/teamstab-update?view=graph-rest-beta) a Microsoft Teams tab using Microsoft Graph APIs, you need to know the `teamsAppId` of the app, and the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` to provide for that kind of app.</span></span>
<span data-ttu-id="e11b0-105">本文介绍如何获取内置选项卡类型的值。</span><span class="sxs-lookup"><span data-stu-id="e11b0-105">This article explains how to get those values for the built-in tab types.</span></span>

## <a name="website-tabs"></a><span data-ttu-id="e11b0-106">网站选项卡</span><span class="sxs-lookup"><span data-stu-id="e11b0-106">Website tabs</span></span>

<span data-ttu-id="e11b0-107">对于网站选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.web`。</span><span class="sxs-lookup"><span data-stu-id="e11b0-107">For website tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.web`.</span></span> <span data-ttu-id="e11b0-108">以下是配置。</span><span class="sxs-lookup"><span data-stu-id="e11b0-108">The following is the configuration.</span></span>

| <span data-ttu-id="e11b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="e11b0-109">Property</span></span>   | <span data-ttu-id="e11b0-110">类型</span><span class="sxs-lookup"><span data-stu-id="e11b0-110">Type</span></span>        | <span data-ttu-id="e11b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="e11b0-111">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="e11b0-112">entityId</span><span class="sxs-lookup"><span data-stu-id="e11b0-112">entityId</span></span>   | <span data-ttu-id="e11b0-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e11b0-113">string</span></span>      | <span data-ttu-id="e11b0-114">Null</span><span class="sxs-lookup"><span data-stu-id="e11b0-114">Null</span></span>                                                     |
| <span data-ttu-id="e11b0-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="e11b0-115">contentUrl</span></span> | <span data-ttu-id="e11b0-116">string</span><span class="sxs-lookup"><span data-stu-id="e11b0-116">string</span></span>      | <span data-ttu-id="e11b0-117">网站的 URL</span><span class="sxs-lookup"><span data-stu-id="e11b0-117">URL of the website</span></span>                                       |
| <span data-ttu-id="e11b0-118">removeUrl</span><span class="sxs-lookup"><span data-stu-id="e11b0-118">removeUrl</span></span>  | <span data-ttu-id="e11b0-119">字符串</span><span class="sxs-lookup"><span data-stu-id="e11b0-119">string</span></span>      | <span data-ttu-id="e11b0-120">Null</span><span class="sxs-lookup"><span data-stu-id="e11b0-120">Null</span></span>                                                     |
| <span data-ttu-id="e11b0-121">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="e11b0-121">websiteUrl</span></span> | <span data-ttu-id="e11b0-122">string</span><span class="sxs-lookup"><span data-stu-id="e11b0-122">string</span></span>      | <span data-ttu-id="e11b0-123">网站的 URL</span><span class="sxs-lookup"><span data-stu-id="e11b0-123">URL of the website</span></span>                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a><span data-ttu-id="e11b0-124">Word、Excel、PowerPoint 和 PDF 选项卡</span><span class="sxs-lookup"><span data-stu-id="e11b0-124">Word, Excel, PowerPoint, and PDF tabs</span></span>

<span data-ttu-id="e11b0-125">下表列出了每个应用的 `teamsAppId`。</span><span class="sxs-lookup"><span data-stu-id="e11b0-125">The following table lists the `teamsAppId` for each app.</span></span>

| <span data-ttu-id="e11b0-126">应用</span><span class="sxs-lookup"><span data-stu-id="e11b0-126">App</span></span>   | <span data-ttu-id="e11b0-127">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="e11b0-127">teamsAppId</span></span> | <span data-ttu-id="e11b0-128">类型（扩展名）</span><span class="sxs-lookup"><span data-stu-id="e11b0-128">type (extension)</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="e11b0-129">Word</span><span class="sxs-lookup"><span data-stu-id="e11b0-129">Word</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| <span data-ttu-id="e11b0-130">Excel</span><span class="sxs-lookup"><span data-stu-id="e11b0-130">Excel</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| <span data-ttu-id="e11b0-131">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="e11b0-131">PowerPoint</span></span>  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| <span data-ttu-id="e11b0-132">PDF</span><span class="sxs-lookup"><span data-stu-id="e11b0-132">PDF</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

<span data-ttu-id="e11b0-133">以下是配置。</span><span class="sxs-lookup"><span data-stu-id="e11b0-133">The following is the configuration.</span></span>

| <span data-ttu-id="e11b0-134">属性</span><span class="sxs-lookup"><span data-stu-id="e11b0-134">Property</span></span>   | <span data-ttu-id="e11b0-135">类型</span><span class="sxs-lookup"><span data-stu-id="e11b0-135">Type</span></span>        | <span data-ttu-id="e11b0-136">说明</span><span class="sxs-lookup"><span data-stu-id="e11b0-136">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="e11b0-137">entityId</span><span class="sxs-lookup"><span data-stu-id="e11b0-137">entityId</span></span>   | <span data-ttu-id="e11b0-138">字符串</span><span class="sxs-lookup"><span data-stu-id="e11b0-138">string</span></span>      | <span data-ttu-id="e11b0-139">文件的 sourceDoc ID。</span><span class="sxs-lookup"><span data-stu-id="e11b0-139">The sourceDoc ID of the file.</span></span> <span data-ttu-id="e11b0-140">通过打开 SharePoint 中文件并查看地址栏即可找到 – URL 将有一个`sourcedoc=%7B{sourceDocId}%7D`子句。</span><span class="sxs-lookup"><span data-stu-id="e11b0-140">You can find this by opening the file in SharePoint and looking at the address bar – the URL will have a `sourcedoc=%7B{sourceDocId}%7D` clause.</span></span> <span data-ttu-id="e11b0-141">此外还可从文档 SharePoint 驱动器项的 webUrl 派生。</span><span class="sxs-lookup"><span data-stu-id="e11b0-141">You can also derive this from the webUrl of the SharePoint drive item for the document.</span></span> <span data-ttu-id="e11b0-142">有关详细信息，请参阅 [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="e11b0-142">For details, see [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="e11b0-143">contentUrl</span><span class="sxs-lookup"><span data-stu-id="e11b0-143">contentUrl</span></span> | <span data-ttu-id="e11b0-144">字符串</span><span class="sxs-lookup"><span data-stu-id="e11b0-144">string</span></span>      | <span data-ttu-id="e11b0-145">`{folder-webUrl}/{item-name}` 格式文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="e11b0-145">The URL of file in the format `{folder-webUrl}/{item-name}`.</span></span> <span data-ttu-id="e11b0-146">{folder-webUrl} 是包含文件的 SharePoint 文件夹 webUrl，通过打开 SharePoint 中文件并查看地址栏，或使用 [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta) 的 webUrl 属性即可找到该文件。</span><span class="sxs-lookup"><span data-stu-id="e11b0-146">{folder-webUrl} is the webUrl of the SharePoint folder containing the file, which can be found by opening the file in SharePoint and looking at the address bar, or by using the webUrl property from [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> <span data-ttu-id="e11b0-147">{item-name} 是文件名（例如 file.docx），也就是 [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta) 中的 `name` 属性。</span><span class="sxs-lookup"><span data-stu-id="e11b0-147">{item-name} is the file name (for example, file.docx), which is the `name` property in [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="e11b0-148">removeUrl</span><span class="sxs-lookup"><span data-stu-id="e11b0-148">removeUrl</span></span>  | <span data-ttu-id="e11b0-149">字符串</span><span class="sxs-lookup"><span data-stu-id="e11b0-149">string</span></span>      | <span data-ttu-id="e11b0-150">Null</span><span class="sxs-lookup"><span data-stu-id="e11b0-150">Null</span></span>                                                     |
| <span data-ttu-id="e11b0-151">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="e11b0-151">websiteUrl</span></span> | <span data-ttu-id="e11b0-152">字符串</span><span class="sxs-lookup"><span data-stu-id="e11b0-152">string</span></span>      | <span data-ttu-id="e11b0-153">Null</span><span class="sxs-lookup"><span data-stu-id="e11b0-153">Null</span></span>                                       |

### <a name="example-create-a-configured-word-tab"></a><span data-ttu-id="e11b0-154">示例： 创建一个配置好的 Word 选项卡</span><span class="sxs-lookup"><span data-stu-id="e11b0-154">Example: Create a configured Word tab</span></span>

<span data-ttu-id="e11b0-155">以下示例将新建一个配置好的 Word 选项卡。</span><span class="sxs-lookup"><span data-stu-id="e11b0-155">The following example creates a configured Word tab.</span></span>

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
