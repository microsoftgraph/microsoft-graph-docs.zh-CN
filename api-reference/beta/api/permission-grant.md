---
author: kevklam
ms.author: kevinlam
title: 授予权限
description: 授予用户列表访问权限以使用指定的链接
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4163c93179ecc55b71c76d1d18d64bf8dae36b96
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349563"
---
# <a name="grant-permission"></a><span data-ttu-id="e05c9-103">授予权限</span><span class="sxs-lookup"><span data-stu-id="e05c9-103">Grant permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e05c9-104">授予用户对由[权限][]表示的链接的访问权限。</span><span class="sxs-lookup"><span data-stu-id="e05c9-104">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="e05c9-105">权限</span><span class="sxs-lookup"><span data-stu-id="e05c9-105">Permissions</span></span>

<span data-ttu-id="e05c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e05c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e05c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e05c9-108">Permission type</span></span>                   | <span data-ttu-id="e05c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e05c9-109">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e05c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e05c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e05c9-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e05c9-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e05c9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e05c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e05c9-113">不支持</span><span class="sxs-lookup"><span data-stu-id="e05c9-113">Not supported</span></span>    |
|<span data-ttu-id="e05c9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e05c9-114">Application</span></span> | <span data-ttu-id="e05c9-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e05c9-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e05c9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e05c9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="e05c9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e05c9-117">Request headers</span></span>

| <span data-ttu-id="e05c9-118">名称</span><span class="sxs-lookup"><span data-stu-id="e05c9-118">Name</span></span>          | <span data-ttu-id="e05c9-119">说明</span><span class="sxs-lookup"><span data-stu-id="e05c9-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="e05c9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e05c9-120">Authorization</span></span> | <span data-ttu-id="e05c9-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="e05c9-121">Bearer \{token\}.</span></span> <span data-ttu-id="e05c9-122">必需。</span><span class="sxs-lookup"><span data-stu-id="e05c9-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e05c9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e05c9-123">Request body</span></span>

<span data-ttu-id="e05c9-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e05c9-124">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="e05c9-125">参数</span><span class="sxs-lookup"><span data-stu-id="e05c9-125">Parameter</span></span>          | <span data-ttu-id="e05c9-126">类型</span><span class="sxs-lookup"><span data-stu-id="e05c9-126">Type</span></span>                           | <span data-ttu-id="e05c9-127">说明</span><span class="sxs-lookup"><span data-stu-id="e05c9-127">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="e05c9-128">recipients</span><span class="sxs-lookup"><span data-stu-id="e05c9-128">recipients</span></span>         | <span data-ttu-id="e05c9-129">集合 ([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="e05c9-129">Collection([driveRecipient][])</span></span> | <span data-ttu-id="e05c9-130">将接收访问权限的收件人集合。</span><span class="sxs-lookup"><span data-stu-id="e05c9-130">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="e05c9-131">roles</span><span class="sxs-lookup"><span data-stu-id="e05c9-131">roles</span></span>              | <span data-ttu-id="e05c9-132">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="e05c9-132">Collection(String)</span></span>             | <span data-ttu-id="e05c9-133">如果链接是 "现有访问" 链接, 则指定要向用户授予的角色。</span><span class="sxs-lookup"><span data-stu-id="e05c9-133">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="e05c9-134">否则, 必须与链接的角色相匹配。</span><span class="sxs-lookup"><span data-stu-id="e05c9-134">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="e05c9-135">如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration-values)。</span><span class="sxs-lookup"><span data-stu-id="e05c9-135">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="response"></a><span data-ttu-id="e05c9-136">响应</span><span class="sxs-lookup"><span data-stu-id="e05c9-136">Response</span></span>

<span data-ttu-id="e05c9-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[权限][]集合。</span><span class="sxs-lookup"><span data-stu-id="e05c9-137">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="e05c9-138">在成功时, 将始终在结果集中返回一个表示已更新链接的[权限][]。</span><span class="sxs-lookup"><span data-stu-id="e05c9-138">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="e05c9-139">更新的链接可以通过包含 "scope" 属性的 "link" facet 来标识。</span><span class="sxs-lookup"><span data-stu-id="e05c9-139">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="e05c9-140">在某些情况下, 可能更新的链接具有与原始链接不同的 URL, 在这种情况下应使用新的 URL。</span><span class="sxs-lookup"><span data-stu-id="e05c9-140">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="e05c9-141">阅读 "[错误响应][error-response]" 主题, 了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e05c9-141">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="e05c9-142">示例</span><span class="sxs-lookup"><span data-stu-id="e05c9-142">Example</span></span>

<span data-ttu-id="e05c9-143">此示例授予用户 john@contoso.com 和 ryan@external.com 对共享链接的访问权限, 而不修改该链接的其他现有权限。</span><span class="sxs-lookup"><span data-stu-id="e05c9-143">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="e05c9-144">请求</span><span class="sxs-lookup"><span data-stu-id="e05c9-144">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e05c9-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e05c9-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST https://graph.microsoft.com/beta/shares/{encoded-sharing-url}/permission/grant
Content-type: application/json

{
  "recipients": [
    {
      "email": "john@contoso.com"
    },
    {
      "email": "ryan@external.com"
    }
  ],
  "roles": ["read"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e05c9-146">C#</span><span class="sxs-lookup"><span data-stu-id="e05c9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e05c9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e05c9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e05c9-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="e05c9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e05c9-149">Java</span><span class="sxs-lookup"><span data-stu-id="e05c9-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e05c9-150">响应</span><span class="sxs-lookup"><span data-stu-id="e05c9-150">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "5fab944a-47ec-48d0-a9b5-5178a926d00f",
      "link": {
        "preventsDownload": false,
        "scope": "users",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/design/EZexPoDjW4dMtKFUfAl6BK4BvIUuss52hLYzihBfx-PD6Q"
      },
      "roles": [
        "read"
      ]
    }
  ]
}
```

><span data-ttu-id="e05c9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e05c9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="e05c9-153">如果链接是现有的[访问](../resources/permission.md#existing-access-link)链接, 则将返回其他权限, 代表以下内容:</span><span class="sxs-lookup"><span data-stu-id="e05c9-153">If the link is an [existing access](../resources/permission.md#existing-access-link) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="e05c9-154">代表成功授予访问权限的收件人的用户类型权限。</span><span class="sxs-lookup"><span data-stu-id="e05c9-154">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="e05c9-155">可以通过**grantedTo**属性的状态来识别这些属性。</span><span class="sxs-lookup"><span data-stu-id="e05c9-155">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="e05c9-156">代表需要发送到无法识别的外部用户以获取访问权限的邀请的链接类型权限。</span><span class="sxs-lookup"><span data-stu-id="e05c9-156">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="e05c9-157">可以通过[邀请](../resources/sharinginvitation.md)方面来识别这些信息。</span><span class="sxs-lookup"><span data-stu-id="e05c9-157">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="e05c9-158">这些条目将包含具有邀请 URL 的[链接][sharing-link], grantedToIdentities 集合将指示应向其发送该链接的用户。</span><span class="sxs-lookup"><span data-stu-id="e05c9-158">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "00000000-0000-0000-0000-000000000000",
      "link": {
        "preventsDownload": false,
        "scope": "existingAccess",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/teams/design/shareddocs/Document.docx"
      },
      "roles": [
        "read"
      ]
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "John Smith",
          "email": "john@contoso.com",
          "id": "47aecee2-d061-4730-8ecb-4c61360441ae"
        }
      },
      "id": "aTowIy5mfG1lbWJlcnNoaXB8bGltaXRlZDJAa2xhbW9kYi5vbm1pY3Jvc29mdC5jb20",
      "roles": [
        "read"
      ]
    },
    {
      "grantedToIdentities": [
        {
          "user": {
            "email": "ryan@external.com"
          }
        }
      ],
      "invitation": {
        "signInRequired": true
      },
      "roles": [
        "read"
      ],
      "link": {
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/teams/design/EZexPoDjW4dMtKFUfAl6BK4Bw_F7gFH63O310A7lDtK0mQ"
      }
    }
  ]
}

```

><span data-ttu-id="e05c9-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e05c9-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e05c9-160">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e05c9-160">All the properties will be returned from an actual call.</span></span>



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[权限]: ../resources/permission.md
[permission]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
