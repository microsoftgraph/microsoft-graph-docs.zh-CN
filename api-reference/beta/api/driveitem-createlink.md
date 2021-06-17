---
author: JeremyKelley
description: 可以使用 createLink 操作通过共享链接共享 DriveItem。
title: driveItem： createLink
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e65cdc780b5c38441471dd14292f0420bf0ca629
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990729"
---
# <a name="driveitem-createlink"></a><span data-ttu-id="b80b7-103">driveItem： createLink</span><span class="sxs-lookup"><span data-stu-id="b80b7-103">driveItem: createLink</span></span>

<span data-ttu-id="b80b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b80b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b80b7-105">可以使用 **createLink** 操作通过共享链接共享 [driveItem。](../resources/driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="b80b7-105">You can use **createLink** action to share a [driveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="b80b7-p101">如果调用应用程序指定的链接类型尚不存在，**CreateLink** 操作将创建新的共享链接。如果应用程序指定的共享链接类型已存在，则返回现有的共享链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="b80b7-108">DriveItem 资源从其上级继承共享权限。</span><span class="sxs-lookup"><span data-stu-id="b80b7-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="b80b7-109">权限</span><span class="sxs-lookup"><span data-stu-id="b80b7-109">Permissions</span></span>

<span data-ttu-id="b80b7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b80b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b80b7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b80b7-112">Permission type</span></span>      | <span data-ttu-id="b80b7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b80b7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b80b7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b80b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b80b7-115">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80b7-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b80b7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b80b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b80b7-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80b7-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b80b7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b80b7-118">Application</span></span> | <span data-ttu-id="b80b7-119">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80b7-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b80b7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b80b7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```
## <a name="request-headers"></a><span data-ttu-id="b80b7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b80b7-121">Request headers</span></span>
|<span data-ttu-id="b80b7-122">名称</span><span class="sxs-lookup"><span data-stu-id="b80b7-122">Name</span></span>|<span data-ttu-id="b80b7-123">说明</span><span class="sxs-lookup"><span data-stu-id="b80b7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b80b7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b80b7-124">Authorization</span></span>|<span data-ttu-id="b80b7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b80b7-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b80b7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b80b7-127">Content-Type</span></span>|<span data-ttu-id="b80b7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b80b7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b80b7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b80b7-130">Request body</span></span>

<span data-ttu-id="b80b7-131">请求正文定义应用程序正在请求的共享链接的属性。</span><span class="sxs-lookup"><span data-stu-id="b80b7-131">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="b80b7-132">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b80b7-132">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="b80b7-133">属性</span><span class="sxs-lookup"><span data-stu-id="b80b7-133">Property</span></span>                 |  <span data-ttu-id="b80b7-134">类型</span><span class="sxs-lookup"><span data-stu-id="b80b7-134">Type</span></span>  |                                 <span data-ttu-id="b80b7-135">说明</span><span class="sxs-lookup"><span data-stu-id="b80b7-135">Description</span></span>                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b80b7-136">type</span><span class="sxs-lookup"><span data-stu-id="b80b7-136">type</span></span>|<span data-ttu-id="b80b7-137">String</span><span class="sxs-lookup"><span data-stu-id="b80b7-137">String</span></span>|<span data-ttu-id="b80b7-138">可选。要创建的共享链接的类型。</span><span class="sxs-lookup"><span data-stu-id="b80b7-138">Optional.The type of sharing link to create.</span></span>   |
|<span data-ttu-id="b80b7-139">scope</span><span class="sxs-lookup"><span data-stu-id="b80b7-139">scope</span></span>|<span data-ttu-id="b80b7-140">String</span><span class="sxs-lookup"><span data-stu-id="b80b7-140">String</span></span>|<span data-ttu-id="b80b7-141">可选。</span><span class="sxs-lookup"><span data-stu-id="b80b7-141">Optional.</span></span> <span data-ttu-id="b80b7-142">要创建的链接的范围。</span><span class="sxs-lookup"><span data-stu-id="b80b7-142">The scope of link to create.</span></span> <span data-ttu-id="b80b7-143">匿名、组织或用户。</span><span class="sxs-lookup"><span data-stu-id="b80b7-143">Either anonymous, organization or users.</span></span>|
|<span data-ttu-id="b80b7-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b80b7-144">expirationDateTime</span></span>|<span data-ttu-id="b80b7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b80b7-145">DateTimeOffset</span></span>|<span data-ttu-id="b80b7-146">可选。</span><span class="sxs-lookup"><span data-stu-id="b80b7-146">Optional.</span></span> <span data-ttu-id="b80b7-147">DateTime 格式为 yyyy-MM-ddTHH：mm：ssZ 的 String 表示权限的过期时间。</span><span class="sxs-lookup"><span data-stu-id="b80b7-147">A String with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span>|
|<span data-ttu-id="b80b7-148">密码</span><span class="sxs-lookup"><span data-stu-id="b80b7-148">password</span></span>|<span data-ttu-id="b80b7-149">String</span><span class="sxs-lookup"><span data-stu-id="b80b7-149">String</span></span>|<span data-ttu-id="b80b7-150">可选。创建者设置的共享链接的密码。</span><span class="sxs-lookup"><span data-stu-id="b80b7-150">Optional.The password of the sharing link that is set by the creator.</span></span>|
|<span data-ttu-id="b80b7-151">recipients</span><span class="sxs-lookup"><span data-stu-id="b80b7-151">recipients</span></span>|<span data-ttu-id="b80b7-152">[driveRecipient](../resources/driverecipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b80b7-152">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="b80b7-153">可选。</span><span class="sxs-lookup"><span data-stu-id="b80b7-153">Optional.</span></span> <span data-ttu-id="b80b7-154">将接收共享链接访问权限的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="b80b7-154">A collection of recipients who will receive access to the sharing link.</span></span>|

### <a name="link-types"></a><span data-ttu-id="b80b7-155">链接类型</span><span class="sxs-lookup"><span data-stu-id="b80b7-155">Link types</span></span>

<span data-ttu-id="b80b7-156">**type** 参数允许使用以下值：</span><span class="sxs-lookup"><span data-stu-id="b80b7-156">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="b80b7-157">类型值</span><span class="sxs-lookup"><span data-stu-id="b80b7-157">Type value</span></span> | <span data-ttu-id="b80b7-158">说明</span><span class="sxs-lookup"><span data-stu-id="b80b7-158">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="b80b7-159">view</span><span class="sxs-lookup"><span data-stu-id="b80b7-159">view</span></span>           | <span data-ttu-id="b80b7-160">创建到 **driveItem** 的只读链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-160">Creates a read-only link to the **driveItem**.</span></span>                                                                        |
| <span data-ttu-id="b80b7-161">review</span><span class="sxs-lookup"><span data-stu-id="b80b7-161">review</span></span>         | <span data-ttu-id="b80b7-162">创建 **driveItem 的审阅链接**。</span><span class="sxs-lookup"><span data-stu-id="b80b7-162">Creates a review link to the **driveItem**.</span></span> <span data-ttu-id="b80b7-163">此选项仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b80b7-163">This option is only available for files in OneDrive for Business and SharePoint.</span></span>                   |
| <span data-ttu-id="b80b7-164">edit</span><span class="sxs-lookup"><span data-stu-id="b80b7-164">edit</span></span>           | <span data-ttu-id="b80b7-165">创建到 **driveItem** 的读写链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-165">Creates an read-write link to the **driveItem**.</span></span>                                                                       |
| <span data-ttu-id="b80b7-166">嵌入</span><span class="sxs-lookup"><span data-stu-id="b80b7-166">embed</span></span>          | <span data-ttu-id="b80b7-167">创建 **driveItem** 的可嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-167">Creates an embeddable link to the **driveItem**.</span></span>                                                                      |
| <span data-ttu-id="b80b7-168">blocksDownload</span><span class="sxs-lookup"><span data-stu-id="b80b7-168">blocksDownload</span></span> | <span data-ttu-id="b80b7-169">创建阻止下载到 **driveItem** 的只读链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-169">Creates a read-only link that blocks download to the **driveItem**.</span></span> <span data-ttu-id="b80b7-170">此选项仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b80b7-170">This option is only available for files in OneDrive for Business and SharePoint.</span></span>  |
| <span data-ttu-id="b80b7-171">createOnly</span><span class="sxs-lookup"><span data-stu-id="b80b7-171">createOnly</span></span>     | <span data-ttu-id="b80b7-172">创建 **driveItem** 的仅上载链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-172">Creates an upload-only link to the **driveItem**.</span></span> <span data-ttu-id="b80b7-173">此选项仅适用于 OneDrive for Business 和 SharePoint 中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b80b7-173">This option is only available for folders in OneDrive for Business and SharePoint.</span></span>             |
| <span data-ttu-id="b80b7-174">addressBar</span><span class="sxs-lookup"><span data-stu-id="b80b7-174">addressBar</span></span>     | <span data-ttu-id="b80b7-175">为新建的文件创建浏览器地址栏中显示的默认链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-175">Creates the default link that is shown in the browser address bars for newly created files.</span></span> <span data-ttu-id="b80b7-176">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b80b7-176">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="b80b7-177">组织管理员配置此链接类型是否受支持，以及此链接类型支持哪些功能。</span><span class="sxs-lookup"><span data-stu-id="b80b7-177">The organization admin configures whether this link type is supported, and what features are supported by this link type.</span></span> |
| <span data-ttu-id="b80b7-178">adminDefault</span><span class="sxs-lookup"><span data-stu-id="b80b7-178">adminDefault</span></span>   | <span data-ttu-id="b80b7-179">创建到 **driveItem** 的默认链接，该链接由组织的管理员确定。</span><span class="sxs-lookup"><span data-stu-id="b80b7-179">Creates the default link to the **driveItem** as determined by the administrator of the organization.</span></span> <span data-ttu-id="b80b7-180">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b80b7-180">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="b80b7-181">该策略由管理员为组织强制执行</span><span class="sxs-lookup"><span data-stu-id="b80b7-181">The policy is enforced for the organization by the admin</span></span> |

### <a name="scope-types"></a><span data-ttu-id="b80b7-182">范围类型</span><span class="sxs-lookup"><span data-stu-id="b80b7-182">Scope types</span></span>

<span data-ttu-id="b80b7-183">**scope** 参数允许使用以下值。</span><span class="sxs-lookup"><span data-stu-id="b80b7-183">The following values are allowed for the **scope** parameter.</span></span>

| <span data-ttu-id="b80b7-184">值</span><span class="sxs-lookup"><span data-stu-id="b80b7-184">Value</span></span>          | <span data-ttu-id="b80b7-185">说明</span><span class="sxs-lookup"><span data-stu-id="b80b7-185">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="b80b7-186">anonymous</span><span class="sxs-lookup"><span data-stu-id="b80b7-186">anonymous</span></span>    | <span data-ttu-id="b80b7-187">拥有该链接的任何人都可以访问，无需登录。</span><span class="sxs-lookup"><span data-stu-id="b80b7-187">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="b80b7-188">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="b80b7-188">This may include people outside of your organization.</span></span> <span data-ttu-id="b80b7-189">管理员可能会禁用匿名链接支持。</span><span class="sxs-lookup"><span data-stu-id="b80b7-189">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="b80b7-190">组织</span><span class="sxs-lookup"><span data-stu-id="b80b7-190">organization</span></span> | <span data-ttu-id="b80b7-191">登录到组织（租户）的任何人都可以使用该链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="b80b7-191">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="b80b7-192">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b80b7-192">Only available in OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="b80b7-193">users</span><span class="sxs-lookup"><span data-stu-id="b80b7-193">users</span></span>        | <span data-ttu-id="b80b7-194">收件人集合中的特定人员可以使用链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="b80b7-194">Specific people in the recipients collection can use the link to get access.</span></span> <span data-ttu-id="b80b7-195">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b80b7-195">Only available in OneDrive for Business and SharePoint.</span></span>

## <a name="response"></a><span data-ttu-id="b80b7-196">响应</span><span class="sxs-lookup"><span data-stu-id="b80b7-196">Response</span></span>

<span data-ttu-id="b80b7-197">如果成功，此方法将在响应正文中返回单个 [Permission](../resources/permission.md) 资源，此响应正文表示请求的共享权限。</span><span class="sxs-lookup"><span data-stu-id="b80b7-197">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="b80b7-198">如果为 `201 Created` **driveItem** 创建了新的共享链接，或者返回了现有链接， `200 OK` 则响应将为 。</span><span class="sxs-lookup"><span data-stu-id="b80b7-198">The response will be `201 Created` if a new sharing link is created for the **driveItem** or `200 OK` if an existing link is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="b80b7-199">示例</span><span class="sxs-lookup"><span data-stu-id="b80b7-199">Examples</span></span>

### <a name="example-1-create-an-anonymous-sharing-link"></a><span data-ttu-id="b80b7-200">示例 1：创建匿名共享链接</span><span class="sxs-lookup"><span data-stu-id="b80b7-200">Example 1: Create an anonymous sharing link</span></span>
<span data-ttu-id="b80b7-201">以下示例请求为用户的 OneDrive 中的 {itemId} 指定的 **driveItem** 创建共享OneDrive。</span><span class="sxs-lookup"><span data-stu-id="b80b7-201">The following example requests a sharing link to be created for the **driveItem** specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="b80b7-202">共享链接配置为只读并且可由具有该链接的任何用户使用。</span><span class="sxs-lookup"><span data-stu-id="b80b7-202">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

#### <a name="request"></a><span data-ttu-id="b80b7-203">请求</span><span class="sxs-lookup"><span data-stu-id="b80b7-203">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "driveItem_createlink",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
}-->

```http
POST /me/drive/items/{itemId}/createLink
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

# <a name="c"></a>[<span data-ttu-id="b80b7-204">C#</span><span class="sxs-lookup"><span data-stu-id="b80b7-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/driveitem-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b80b7-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b80b7-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/driveitem-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b80b7-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b80b7-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/driveitem-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b80b7-207">Java</span><span class="sxs-lookup"><span data-stu-id="b80b7-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/driveitem-createlink-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b80b7-208">响应</span><span class="sxs-lookup"><span data-stu-id="b80b7-208">Response</span></span>
><span data-ttu-id="b80b7-209">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b80b7-209">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

```http
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

### <a name="example-2-creating-company-sharable-links"></a><span data-ttu-id="b80b7-210">示例 2：创建公司可共享链接</span><span class="sxs-lookup"><span data-stu-id="b80b7-210">Example 2: Creating company sharable links</span></span>

<span data-ttu-id="b80b7-211">OneDrive for Business 和 SharePoint 都支持公司可共享的链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-211">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="b80b7-212">此类链接与匿名链接类似，只不过仅适用于拥有组织的成员。</span><span class="sxs-lookup"><span data-stu-id="b80b7-212">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="b80b7-213">若要创建公司可共享的链接，请使用值为 `organization` 的 **scope** 参数。</span><span class="sxs-lookup"><span data-stu-id="b80b7-213">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

#### <a name="request"></a><span data-ttu-id="b80b7-214">请求</span><span class="sxs-lookup"><span data-stu-id="b80b7-214">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-link-scoped",
  "scopes": "files.readwrite service.sharepoint",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
 } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="b80b7-215">C#</span><span class="sxs-lookup"><span data-stu-id="b80b7-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b80b7-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b80b7-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b80b7-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b80b7-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b80b7-218">Java</span><span class="sxs-lookup"><span data-stu-id="b80b7-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b80b7-219">响应</span><span class="sxs-lookup"><span data-stu-id="b80b7-219">Response</span></span>

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

### <a name="example-3-creating-embeddable-links"></a><span data-ttu-id="b80b7-220">示例 3：创建可嵌入链接</span><span class="sxs-lookup"><span data-stu-id="b80b7-220">Example 3: Creating embeddable links</span></span>

<span data-ttu-id="b80b7-p119">使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。</span><span class="sxs-lookup"><span data-stu-id="b80b7-p119">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

><span data-ttu-id="b80b7-223">**注意：** 仅 OneDrive 个人版支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="b80b7-223">**Note:** Embed links are only supported for OneDrive personal.</span></span>

#### <a name="request"></a><span data-ttu-id="b80b7-224">请求</span><span class="sxs-lookup"><span data-stu-id="b80b7-224">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-embedded-link",
  "scopes": "files.readwrite service.onedrive",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
} -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[<span data-ttu-id="b80b7-225">C#</span><span class="sxs-lookup"><span data-stu-id="b80b7-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b80b7-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b80b7-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b80b7-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b80b7-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b80b7-228">Java</span><span class="sxs-lookup"><span data-stu-id="b80b7-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b80b7-229">响应</span><span class="sxs-lookup"><span data-stu-id="b80b7-229">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b80b7-230">注解</span><span class="sxs-lookup"><span data-stu-id="b80b7-230">Remarks</span></span>

* <span data-ttu-id="b80b7-231">若要根据组织的默认策略和呼叫者对 **driveItem** 的权限创建链接，请省略 scope 和 type 参数</span><span class="sxs-lookup"><span data-stu-id="b80b7-231">To create a link based on the organization's default policy and the caller's permissions on the **driveItem**, omit the scope and type parameters</span></span>
* <span data-ttu-id="b80b7-232">使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。</span><span class="sxs-lookup"><span data-stu-id="b80b7-232">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="b80b7-233">链接在 **driveItem** 的共享权限中可见，并且可以通过 **driveItem** 的所有者删除。</span><span class="sxs-lookup"><span data-stu-id="b80b7-233">Links are visible in the sharing permissions for the **driveItem** and can be removed by an owner of the **driveItem**.</span></span>
* <span data-ttu-id="b80b7-234">链接始终指向 **driveItem** 的当前版本，除非仅将 **driveItem** (SharePoint签出) 。</span><span class="sxs-lookup"><span data-stu-id="b80b7-234">Links always point to the current version of a **driveItem** unless the **driveItem** is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for a driveItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->
