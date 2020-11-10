---
author: kevklam
ms.author: kevinlam
title: 授予权限
description: 授予用户列表访问权限以使用指定的链接
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 307fcf8850666960265986a48ee96140d1c5d28f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979949"
---
# <a name="permission-grant"></a><span data-ttu-id="3bf95-103">权限：授予</span><span class="sxs-lookup"><span data-stu-id="3bf95-103">permission: grant</span></span>

<span data-ttu-id="3bf95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bf95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bf95-105">授予用户对由 [权限][]表示的链接的访问权限。</span><span class="sxs-lookup"><span data-stu-id="3bf95-105">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="3bf95-106">权限</span><span class="sxs-lookup"><span data-stu-id="3bf95-106">Permissions</span></span>

<span data-ttu-id="3bf95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bf95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bf95-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bf95-109">Permission type</span></span>                   | <span data-ttu-id="3bf95-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3bf95-110">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bf95-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bf95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3bf95-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf95-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bf95-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bf95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bf95-114">不支持</span><span class="sxs-lookup"><span data-stu-id="3bf95-114">Not supported</span></span>    |
|<span data-ttu-id="3bf95-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bf95-115">Application</span></span> | <span data-ttu-id="3bf95-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf95-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bf95-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bf95-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="3bf95-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bf95-118">Request headers</span></span>

| <span data-ttu-id="3bf95-119">名称</span><span class="sxs-lookup"><span data-stu-id="3bf95-119">Name</span></span>          | <span data-ttu-id="3bf95-120">说明</span><span class="sxs-lookup"><span data-stu-id="3bf95-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="3bf95-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bf95-121">Authorization</span></span> | <span data-ttu-id="3bf95-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="3bf95-122">Bearer \{token\}.</span></span> <span data-ttu-id="3bf95-123">必填。</span><span class="sxs-lookup"><span data-stu-id="3bf95-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bf95-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bf95-124">Request body</span></span>

<span data-ttu-id="3bf95-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3bf95-125">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="3bf95-126">参数</span><span class="sxs-lookup"><span data-stu-id="3bf95-126">Parameter</span></span>          | <span data-ttu-id="3bf95-127">类型</span><span class="sxs-lookup"><span data-stu-id="3bf95-127">Type</span></span>                           | <span data-ttu-id="3bf95-128">说明</span><span class="sxs-lookup"><span data-stu-id="3bf95-128">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="3bf95-129">recipients</span><span class="sxs-lookup"><span data-stu-id="3bf95-129">recipients</span></span>         | <span data-ttu-id="3bf95-130"> ([driveRecipient][]) 的集合</span><span class="sxs-lookup"><span data-stu-id="3bf95-130">Collection([driveRecipient][])</span></span> | <span data-ttu-id="3bf95-131">将接收访问权限的收件人集合。</span><span class="sxs-lookup"><span data-stu-id="3bf95-131">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="3bf95-132">角色</span><span class="sxs-lookup"><span data-stu-id="3bf95-132">roles</span></span>              | <span data-ttu-id="3bf95-133">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="3bf95-133">Collection(String)</span></span>             | <span data-ttu-id="3bf95-134">如果链接是 "现有访问" 链接，则指定要向用户授予的角色。</span><span class="sxs-lookup"><span data-stu-id="3bf95-134">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="3bf95-135">否则，必须与链接的角色相匹配。</span><span class="sxs-lookup"><span data-stu-id="3bf95-135">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="3bf95-136">有关可用角色的列表，请参阅 [roles 属性值](../resources/permission.md#roles-property-values)。</span><span class="sxs-lookup"><span data-stu-id="3bf95-136">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="response"></a><span data-ttu-id="3bf95-137">响应</span><span class="sxs-lookup"><span data-stu-id="3bf95-137">Response</span></span>

<span data-ttu-id="3bf95-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [权限][] 集合。</span><span class="sxs-lookup"><span data-stu-id="3bf95-138">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="3bf95-139">在成功时，将始终在结果集中返回一个表示已更新链接的 [权限][] 。</span><span class="sxs-lookup"><span data-stu-id="3bf95-139">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="3bf95-140">更新的链接可以通过包含 "scope" 属性的 "link" facet 来标识。</span><span class="sxs-lookup"><span data-stu-id="3bf95-140">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="3bf95-141">在某些情况下，可能更新的链接具有与原始链接不同的 URL，在这种情况下应使用新的 URL。</span><span class="sxs-lookup"><span data-stu-id="3bf95-141">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="3bf95-142">阅读 " [错误响应][error-response] " 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3bf95-142">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="3bf95-143">示例</span><span class="sxs-lookup"><span data-stu-id="3bf95-143">Example</span></span>

<span data-ttu-id="3bf95-144">此示例授予用户 john@contoso.com 和 ryan@external.com 对共享链接的访问权限，而不修改该链接的其他现有权限。</span><span class="sxs-lookup"><span data-stu-id="3bf95-144">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="3bf95-145">请求</span><span class="sxs-lookup"><span data-stu-id="3bf95-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3bf95-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bf95-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "permission-grant", "scopes": "files.readwrite", "target": "action" } -->

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
# <a name="c"></a>[<span data-ttu-id="3bf95-147">C#</span><span class="sxs-lookup"><span data-stu-id="3bf95-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-grant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bf95-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bf95-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-grant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bf95-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bf95-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-grant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bf95-150">Java</span><span class="sxs-lookup"><span data-stu-id="3bf95-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-grant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3bf95-151">响应</span><span class="sxs-lookup"><span data-stu-id="3bf95-151">Response</span></span>

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

><span data-ttu-id="3bf95-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3bf95-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="3bf95-154">如果链接是现有的 [访问](../resources/permission.md#existing-access-link) 链接，则将返回其他权限，代表以下内容：</span><span class="sxs-lookup"><span data-stu-id="3bf95-154">If the link is an [existing access](../resources/permission.md#existing-access-link) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="3bf95-155">代表成功授予访问权限的收件人的用户类型权限。</span><span class="sxs-lookup"><span data-stu-id="3bf95-155">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="3bf95-156">可以通过 **grantedTo** 属性的状态来识别这些属性。</span><span class="sxs-lookup"><span data-stu-id="3bf95-156">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="3bf95-157">代表需要发送到无法识别的外部用户以获取访问权限的邀请的链接类型权限。</span><span class="sxs-lookup"><span data-stu-id="3bf95-157">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="3bf95-158">可以通过 [邀请](../resources/sharinginvitation.md) 方面来识别这些信息。</span><span class="sxs-lookup"><span data-stu-id="3bf95-158">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="3bf95-159">这些条目将包含具有邀请 URL 的 [链接][sharing-link] ，grantedToIdentities 集合将指示应向其发送该链接的用户。</span><span class="sxs-lookup"><span data-stu-id="3bf95-159">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

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

><span data-ttu-id="3bf95-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3bf95-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3bf95-161">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3bf95-161">All the properties will be returned from an actual call.</span></span>



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


