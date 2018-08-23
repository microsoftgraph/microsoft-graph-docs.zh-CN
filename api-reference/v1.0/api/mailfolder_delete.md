# <a name="delete-mailfolder"></a><span data-ttu-id="5bc98-101">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="5bc98-101">Delete mailFolder</span></span>

<span data-ttu-id="5bc98-102">删除指定的 [mailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5bc98-102">Delete the specified mailFolder object.</span></span>

<span data-ttu-id="5bc98-103">如果存在，您可以由其文件夹 ID 或按[已知文件夹名称](../resources/mailfolder.md)指定邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="5bc98-103">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="5bc98-104">**注**：您可能无法删除可恢复删除邮件文件夹中的项目（由已知文件夹名称 `recoverableitemsdeletions` 所指代）。</span><span class="sxs-lookup"><span data-stu-id="5bc98-104">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="5bc98-105">有关详细信息，请参阅[已删除邮件的保留期](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清理已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="5bc98-105">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bc98-106">权限</span><span class="sxs-lookup"><span data-stu-id="5bc98-106">Permissions</span></span>
<span data-ttu-id="5bc98-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5bc98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5bc98-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bc98-109">Permission type</span></span>      | <span data-ttu-id="5bc98-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bc98-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bc98-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bc98-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5bc98-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bc98-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5bc98-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bc98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bc98-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bc98-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5bc98-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bc98-115">Application</span></span> | <span data-ttu-id="5bc98-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bc98-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bc98-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bc98-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5bc98-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bc98-118">Request headers</span></span>
| <span data-ttu-id="5bc98-119">名称</span><span class="sxs-lookup"><span data-stu-id="5bc98-119">Name</span></span>       | <span data-ttu-id="5bc98-120">类型</span><span class="sxs-lookup"><span data-stu-id="5bc98-120">Type</span></span> | <span data-ttu-id="5bc98-121">说明</span><span class="sxs-lookup"><span data-stu-id="5bc98-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5bc98-122">授权</span><span class="sxs-lookup"><span data-stu-id="5bc98-122">Authorization</span></span>  | <span data-ttu-id="5bc98-123">字符串</span><span class="sxs-lookup"><span data-stu-id="5bc98-123">string</span></span>  | <span data-ttu-id="5bc98-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bc98-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bc98-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bc98-126">Request body</span></span>
<span data-ttu-id="5bc98-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bc98-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bc98-128">响应</span><span class="sxs-lookup"><span data-stu-id="5bc98-128">Response</span></span>

<span data-ttu-id="5bc98-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5bc98-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bc98-131">示例</span><span class="sxs-lookup"><span data-stu-id="5bc98-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bc98-132">请求</span><span class="sxs-lookup"><span data-stu-id="5bc98-132">Request</span></span>
<span data-ttu-id="5bc98-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5bc98-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="5bc98-134">响应</span><span class="sxs-lookup"><span data-stu-id="5bc98-134">Response</span></span>
<span data-ttu-id="5bc98-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5bc98-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->