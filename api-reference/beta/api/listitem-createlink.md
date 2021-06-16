---
title: listItem： createLink
description: 创建链接以共享 listItem
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b0d490139763e619a151e3152868f98c1f1b96e4
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941577"
---
# <a name="listitem-createlink"></a><span data-ttu-id="6c062-103">listItem： createLink</span><span class="sxs-lookup"><span data-stu-id="6c062-103">listItem: createLink</span></span>

<span data-ttu-id="6c062-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c062-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c062-105">为 [listItem 创建共享链接](../resources/listitem.md)。</span><span class="sxs-lookup"><span data-stu-id="6c062-105">Create a sharing link for a [listItem](../resources/listitem.md).</span></span>

<span data-ttu-id="6c062-106">如果调用应用程序不存在指定的链接类型 **，createLink** 操作将创建新的共享链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-106">The **createLink** action creates a new sharing link if the specified link type doesn't already exist for the calling application.</span></span>
<span data-ttu-id="6c062-107">如果应用已存在指定类型的共享链接，此操作将返回现有共享链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-107">If a sharing link of the specified type already exists for the app, this action will return the existing sharing link.</span></span>

<span data-ttu-id="6c062-108">**listItem** 资源从项目所在的 [列表中](../resources/list.md) 继承共享权限。</span><span class="sxs-lookup"><span data-stu-id="6c062-108">**listItem** resources inherit sharing permissions from the [list](../resources/list.md) the item resides in.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c062-109">权限</span><span class="sxs-lookup"><span data-stu-id="6c062-109">Permissions</span></span>
<span data-ttu-id="6c062-110">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="6c062-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6c062-111">若要了解更多信息，包括如何选择权限，请参阅 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c062-111">To learn more, including how to choose permissions, see [permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c062-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c062-112">Permission type</span></span>|<span data-ttu-id="6c062-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c062-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c062-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c062-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6c062-115">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c062-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c062-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c062-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c062-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c062-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c062-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c062-118">Application</span></span> | <span data-ttu-id="6c062-119">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c062-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c062-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c062-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
```

## <a name="request-headers"></a><span data-ttu-id="6c062-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c062-121">Request headers</span></span>
|<span data-ttu-id="6c062-122">名称</span><span class="sxs-lookup"><span data-stu-id="6c062-122">Name</span></span>|<span data-ttu-id="6c062-123">说明</span><span class="sxs-lookup"><span data-stu-id="6c062-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c062-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c062-124">Authorization</span></span>|<span data-ttu-id="6c062-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c062-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6c062-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c062-127">Content-Type</span></span>|<span data-ttu-id="6c062-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6c062-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c062-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c062-130">Request body</span></span>
<span data-ttu-id="6c062-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c062-131">In the request body, provide a JSON representation of the parameters.</span></span>

<span data-ttu-id="6c062-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6c062-132">The following table shows the parameters that can be used with this action.</span></span>

|   <span data-ttu-id="6c062-133">属性</span><span class="sxs-lookup"><span data-stu-id="6c062-133">Property</span></span>             |  <span data-ttu-id="6c062-134">类型</span><span class="sxs-lookup"><span data-stu-id="6c062-134">Type</span></span>  |           <span data-ttu-id="6c062-135">说明</span><span class="sxs-lookup"><span data-stu-id="6c062-135">Description</span></span>                        |
| :----------------------| :----- | :--------------------------------------------|
|<span data-ttu-id="6c062-136">type</span><span class="sxs-lookup"><span data-stu-id="6c062-136">type</span></span>|<span data-ttu-id="6c062-137">String</span><span class="sxs-lookup"><span data-stu-id="6c062-137">String</span></span>|<span data-ttu-id="6c062-138">要创建的共享链接的类型。</span><span class="sxs-lookup"><span data-stu-id="6c062-138">The type of sharing link to create.</span></span> <span data-ttu-id="6c062-139">可选。</span><span class="sxs-lookup"><span data-stu-id="6c062-139">Optional.</span></span> |
|<span data-ttu-id="6c062-140">scope</span><span class="sxs-lookup"><span data-stu-id="6c062-140">scope</span></span>|<span data-ttu-id="6c062-141">String</span><span class="sxs-lookup"><span data-stu-id="6c062-141">String</span></span>|<span data-ttu-id="6c062-142">要创建的链接的范围。</span><span class="sxs-lookup"><span data-stu-id="6c062-142">The scope of link to create.</span></span> <span data-ttu-id="6c062-143">、 `anonymous` `organization` 或 `users` 。</span><span class="sxs-lookup"><span data-stu-id="6c062-143">Either `anonymous`, `organization` or `users`.</span></span> <span data-ttu-id="6c062-144">可选。</span><span class="sxs-lookup"><span data-stu-id="6c062-144">Optional.</span></span> |
|<span data-ttu-id="6c062-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6c062-145">expirationDateTime</span></span>|<span data-ttu-id="6c062-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c062-146">DateTimeOffset</span></span>|<span data-ttu-id="6c062-147">DateTime 格式为 yyyy-MM-ddTHH：mm：ssZ 的字符串指示权限的过期时间。</span><span class="sxs-lookup"><span data-stu-id="6c062-147">A string with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span> <span data-ttu-id="6c062-148">可选。</span><span class="sxs-lookup"><span data-stu-id="6c062-148">Optional.</span></span> |
|<span data-ttu-id="6c062-149">密码</span><span class="sxs-lookup"><span data-stu-id="6c062-149">password</span></span>|<span data-ttu-id="6c062-150">String</span><span class="sxs-lookup"><span data-stu-id="6c062-150">String</span></span>|<span data-ttu-id="6c062-151">创建者设置的共享链接的密码。</span><span class="sxs-lookup"><span data-stu-id="6c062-151">The password of the sharing link that is set by the creator.</span></span> <span data-ttu-id="6c062-152">可选。</span><span class="sxs-lookup"><span data-stu-id="6c062-152">Optional.</span></span> |
|<span data-ttu-id="6c062-153">recipients</span><span class="sxs-lookup"><span data-stu-id="6c062-153">recipients</span></span>|<span data-ttu-id="6c062-154">[driveRecipient](../resources/driverecipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c062-154">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="6c062-155">将接收共享链接访问权限的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="6c062-155">A collection of recipients who will receive access to the sharing link.</span></span> <span data-ttu-id="6c062-156">可选。</span><span class="sxs-lookup"><span data-stu-id="6c062-156">Optional.</span></span> |

### <a name="link-types"></a><span data-ttu-id="6c062-157">链接类型</span><span class="sxs-lookup"><span data-stu-id="6c062-157">Link types</span></span>

<span data-ttu-id="6c062-158">**type** 参数允许使用以下值：</span><span class="sxs-lookup"><span data-stu-id="6c062-158">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="6c062-159">类型值</span><span class="sxs-lookup"><span data-stu-id="6c062-159">Type value</span></span> | <span data-ttu-id="6c062-160">说明</span><span class="sxs-lookup"><span data-stu-id="6c062-160">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="6c062-161">view</span><span class="sxs-lookup"><span data-stu-id="6c062-161">view</span></span>           | <span data-ttu-id="6c062-162">创建到项目的只读链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-162">Creates a read-only link to the item.</span></span>                                                                        |
| <span data-ttu-id="6c062-163">review</span><span class="sxs-lookup"><span data-stu-id="6c062-163">review</span></span>         | <span data-ttu-id="6c062-164">创建指向该项目的审阅链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-164">Creates a review link to the item.</span></span> <span data-ttu-id="6c062-165">此选项仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6c062-165">This option is only available for files in OneDrive for Business and SharePoint.</span></span>                   |
| <span data-ttu-id="6c062-166">edit</span><span class="sxs-lookup"><span data-stu-id="6c062-166">edit</span></span>           | <span data-ttu-id="6c062-167">创建指向该项目的读写链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-167">Creates an read-write link to the item.</span></span>                                                                       |
| <span data-ttu-id="6c062-168">嵌入</span><span class="sxs-lookup"><span data-stu-id="6c062-168">embed</span></span>          | <span data-ttu-id="6c062-169">创建到项目的可嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-169">Creates an embeddable link to the item.</span></span>                                                                      |
| <span data-ttu-id="6c062-170">blocksDownload</span><span class="sxs-lookup"><span data-stu-id="6c062-170">blocksDownload</span></span> | <span data-ttu-id="6c062-171">创建阻止下载到项目的只读链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-171">Creates a read-only link that blocks download to the item.</span></span> <span data-ttu-id="6c062-172">此选项仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6c062-172">This option is only available for files in OneDrive for Business and SharePoint.</span></span>  |
| <span data-ttu-id="6c062-173">createOnly</span><span class="sxs-lookup"><span data-stu-id="6c062-173">createOnly</span></span>     | <span data-ttu-id="6c062-174">创建项的仅上载链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-174">Creates an upload-only link to the item.</span></span> <span data-ttu-id="6c062-175">此选项仅适用于 OneDrive for Business 和 SharePoint 中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="6c062-175">This option is only available for folders in OneDrive for Business and SharePoint.</span></span>             |
| <span data-ttu-id="6c062-176">addressBar</span><span class="sxs-lookup"><span data-stu-id="6c062-176">addressBar</span></span>     | <span data-ttu-id="6c062-177">为新建的文件创建浏览器地址栏中显示的默认链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-177">Creates the default link that is shown in the browser address bars for newly created files.</span></span> <span data-ttu-id="6c062-178">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6c062-178">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="6c062-179">组织管理员配置此链接类型是否受支持，以及此链接类型支持哪些功能。</span><span class="sxs-lookup"><span data-stu-id="6c062-179">The organization admin configures whether this link type is supported, and what features are supported by this link type.</span></span> |
| <span data-ttu-id="6c062-180">adminDefault</span><span class="sxs-lookup"><span data-stu-id="6c062-180">adminDefault</span></span>   | <span data-ttu-id="6c062-181">创建指向项目的默认链接，该链接由组织的管理员确定。</span><span class="sxs-lookup"><span data-stu-id="6c062-181">Creates the default link to the item as determined by the administrator of the organization.</span></span> <span data-ttu-id="6c062-182">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6c062-182">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="6c062-183">该策略由管理员为组织强制执行</span><span class="sxs-lookup"><span data-stu-id="6c062-183">The policy is enforced for the organization by the admin</span></span> |

### <a name="scope-types"></a><span data-ttu-id="6c062-184">范围类型</span><span class="sxs-lookup"><span data-stu-id="6c062-184">Scope types</span></span>

<span data-ttu-id="6c062-185">**scope** 参数允许使用以下值。</span><span class="sxs-lookup"><span data-stu-id="6c062-185">The following values are allowed for the **scope** parameter.</span></span>

| <span data-ttu-id="6c062-186">值</span><span class="sxs-lookup"><span data-stu-id="6c062-186">Value</span></span>          | <span data-ttu-id="6c062-187">说明</span><span class="sxs-lookup"><span data-stu-id="6c062-187">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="6c062-188">anonymous</span><span class="sxs-lookup"><span data-stu-id="6c062-188">anonymous</span></span>    | <span data-ttu-id="6c062-189">拥有该链接的任何人都可以访问，无需登录。</span><span class="sxs-lookup"><span data-stu-id="6c062-189">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="6c062-190">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="6c062-190">This may include people outside of your organization.</span></span> <span data-ttu-id="6c062-191">管理员可能会禁用匿名链接支持。</span><span class="sxs-lookup"><span data-stu-id="6c062-191">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="6c062-192">组织</span><span class="sxs-lookup"><span data-stu-id="6c062-192">organization</span></span> | <span data-ttu-id="6c062-193">登录到组织（租户）的任何人都可以使用该链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="6c062-193">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="6c062-194">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6c062-194">Only available in OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="6c062-195">users</span><span class="sxs-lookup"><span data-stu-id="6c062-195">users</span></span>        | <span data-ttu-id="6c062-196">收件人集合中的特定人员可以使用链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="6c062-196">Specific people in the recipients collection can use the link to get access.</span></span> <span data-ttu-id="6c062-197">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6c062-197">Only available in OneDrive for Business and SharePoint.</span></span>

## <a name="response"></a><span data-ttu-id="6c062-198">响应</span><span class="sxs-lookup"><span data-stu-id="6c062-198">Response</span></span>

<span data-ttu-id="6c062-199">如果成功，此方法在表示请求的[](../resources/permission.md)共享权限的响应正文中返回单个权限资源。</span><span class="sxs-lookup"><span data-stu-id="6c062-199">If successful, this method returns a single [permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="6c062-200">如果为 listItem 创建了新的共享链接，或者 `201 Created` `200 OK` 返回了现有链接，则响应将为 。</span><span class="sxs-lookup"><span data-stu-id="6c062-200">The response will be `201 Created` if a new sharing link is created for the listItem or `200 OK` if an existing link is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="6c062-201">示例</span><span class="sxs-lookup"><span data-stu-id="6c062-201">Examples</span></span>

### <a name="example-1-create-an-anonymous-sharing-link"></a><span data-ttu-id="6c062-202">示例 1：创建匿名共享链接</span><span class="sxs-lookup"><span data-stu-id="6c062-202">Example 1: Create an anonymous sharing link</span></span>
<span data-ttu-id="6c062-203">以下示例请求为 {itemId} 在指定的 {listId} 列表中指定的 listItem 创建共享链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-203">The following example requests a sharing link to be created for the listItem specified by {itemId} in the list specified {listId}.</span></span>
<span data-ttu-id="6c062-204">共享链接配置为只读并且可由具有该链接的任何用户使用。</span><span class="sxs-lookup"><span data-stu-id="6c062-204">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

#### <a name="request"></a><span data-ttu-id="6c062-205">请求</span><span class="sxs-lookup"><span data-stu-id="6c062-205">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json
Content-length: 212

{
  "type": "view",
  "scope": "anonymous",
  "password": "String",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="6c062-206">响应</span><span class="sxs-lookup"><span data-stu-id="6c062-206">Response</span></span>
><span data-ttu-id="6c062-207">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6c062-207">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  },
  "hasPassword": true
}
```

### <a name="example-2-creating-company-sharable-links"></a><span data-ttu-id="6c062-208">示例 2：创建公司可共享链接</span><span class="sxs-lookup"><span data-stu-id="6c062-208">Example 2: Creating company sharable links</span></span>

<span data-ttu-id="6c062-209">OneDrive for Business 和 SharePoint 都支持公司可共享的链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-209">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="6c062-210">此类链接与匿名链接类似，只不过仅适用于拥有组织的成员。</span><span class="sxs-lookup"><span data-stu-id="6c062-210">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="6c062-211">若要创建公司可共享的链接，请使用值为 `organization` 的 **scope** 参数。</span><span class="sxs-lookup"><span data-stu-id="6c062-211">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

#### <a name="request"></a><span data-ttu-id="6c062-212">请求</span><span class="sxs-lookup"><span data-stu-id="6c062-212">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

#### <a name="response"></a><span data-ttu-id="6c062-213">响应</span><span class="sxs-lookup"><span data-stu-id="6c062-213">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

### <a name="example-3-creating-embeddable-links"></a><span data-ttu-id="6c062-214">示例 3：创建可嵌入链接</span><span class="sxs-lookup"><span data-stu-id="6c062-214">Example 3: Creating embeddable links</span></span>

<span data-ttu-id="6c062-p120">使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。</span><span class="sxs-lookup"><span data-stu-id="6c062-p120">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

><span data-ttu-id="6c062-217">**注意：** 仅 OneDrive 个人版支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="6c062-217">**Note:** Embed links are only supported for OneDrive personal.</span></span>

#### <a name="request"></a><span data-ttu-id="6c062-218">请求</span><span class="sxs-lookup"><span data-stu-id="6c062-218">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

#### <a name="response"></a><span data-ttu-id="6c062-219">响应</span><span class="sxs-lookup"><span data-stu-id="6c062-219">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="6c062-220">注解</span><span class="sxs-lookup"><span data-stu-id="6c062-220">Remarks</span></span>

* <span data-ttu-id="6c062-221">若要基于组织的默认策略和呼叫者对 listItem 的权限创建链接，请省略 scope 和 type 参数</span><span class="sxs-lookup"><span data-stu-id="6c062-221">To create a link based on the organization's default policy and the caller's permissions on the listItem, omit the scope and type parameters</span></span>
* <span data-ttu-id="6c062-222">使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。</span><span class="sxs-lookup"><span data-stu-id="6c062-222">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="6c062-223">链接在 listItem 的共享权限中可见，并且可以通过 listItem 的所有者删除。</span><span class="sxs-lookup"><span data-stu-id="6c062-223">Links are visible in the sharing permissions for the listItem and can be removed by an owner of the listItem.</span></span>
* <span data-ttu-id="6c062-224">链接始终指向 listItem 的当前版本，除非 listItem 已签出 (SharePoint仅) 。</span><span class="sxs-lookup"><span data-stu-id="6c062-224">Links always point to the current version of a listItem unless the listItem is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an listItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->