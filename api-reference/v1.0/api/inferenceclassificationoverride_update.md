# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="d0964-101">更新 inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="d0964-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="d0964-102">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="d0964-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="d0964-103">不能在 [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) 示例中使用 PATCH 更改任何其他字段。</span><span class="sxs-lookup"><span data-stu-id="d0964-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="d0964-104">如果发件人的替代存在，并且发件人更改了他/她的显示名称，可以使用 [POST](inferenceclassification_post_overrides.md) 强制更新现有替代中的名称字段。</span><span class="sxs-lookup"><span data-stu-id="d0964-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="d0964-105">如果发件人的替代存在，并且发件人更改了他/她的 SMTP 地址，“更新”此发件人的替代的唯一方法是：[删除](inferenceclassificationoverride_delete.md) 现有替代，然后使用新的 SMTP 地址 [创建](inferenceclassification_post_overrides.md) 新替代。</span><span class="sxs-lookup"><span data-stu-id="d0964-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0964-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0964-106">Permissions</span></span>
<span data-ttu-id="d0964-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d0964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0964-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0964-109">Permission type</span></span>      | <span data-ttu-id="d0964-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0964-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0964-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0964-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0964-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0964-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d0964-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0964-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0964-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0964-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d0964-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0964-115">Application</span></span> | <span data-ttu-id="d0964-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0964-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0964-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0964-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d0964-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0964-118">Request headers</span></span>
| <span data-ttu-id="d0964-119">名称</span><span class="sxs-lookup"><span data-stu-id="d0964-119">Name</span></span>       | <span data-ttu-id="d0964-120">类型</span><span class="sxs-lookup"><span data-stu-id="d0964-120">Type</span></span> | <span data-ttu-id="d0964-121">说明</span><span class="sxs-lookup"><span data-stu-id="d0964-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d0964-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0964-122">Authorization</span></span>  | <span data-ttu-id="d0964-123">string</span><span class="sxs-lookup"><span data-stu-id="d0964-123">string</span></span>  | <span data-ttu-id="d0964-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0964-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0964-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0964-126">Content-Type</span></span> | <span data-ttu-id="d0964-127">string</span><span class="sxs-lookup"><span data-stu-id="d0964-127">string</span></span>  | <span data-ttu-id="d0964-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="d0964-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0964-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0964-130">Request body</span></span>
<span data-ttu-id="d0964-p104">在请求正文中，提供 **classifyAs** 的新值。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d0964-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="d0964-133">属性</span><span class="sxs-lookup"><span data-stu-id="d0964-133">Property</span></span>     | <span data-ttu-id="d0964-134">类型</span><span class="sxs-lookup"><span data-stu-id="d0964-134">Type</span></span>   |<span data-ttu-id="d0964-135">说明</span><span class="sxs-lookup"><span data-stu-id="d0964-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0964-136">classifyAs</span><span class="sxs-lookup"><span data-stu-id="d0964-136">classifyAs</span></span>|<span data-ttu-id="d0964-137">string</span><span class="sxs-lookup"><span data-stu-id="d0964-137">string</span></span>| <span data-ttu-id="d0964-p105">指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="d0964-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="d0964-140">响应</span><span class="sxs-lookup"><span data-stu-id="d0964-140">Response</span></span>

<span data-ttu-id="d0964-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0964-141">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0964-142">示例</span><span class="sxs-lookup"><span data-stu-id="d0964-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0964-143">请求</span><span class="sxs-lookup"><span data-stu-id="d0964-143">Request</span></span>
<span data-ttu-id="d0964-144">以下示例将 SMTP 地址 randiw@adatum.onmicrosoft.com 的替代从 `other` 更改为 `focused`。</span><span class="sxs-lookup"><span data-stu-id="d0964-144">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="d0964-145">响应</span><span class="sxs-lookup"><span data-stu-id="d0964-145">Response</span></span>
<span data-ttu-id="d0964-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0964-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->