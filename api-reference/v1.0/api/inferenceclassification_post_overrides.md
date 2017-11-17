# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="752c5-101">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="752c5-101">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="752c5-p101">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="752c5-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="752c5-104">**注意**</span><span class="sxs-lookup"><span data-stu-id="752c5-104">**Note**</span></span>

- <span data-ttu-id="752c5-105">如果已经存在具有相同 STMP 地址的替代，则用提供的值更新该替代的 **classifyAs** 和 **name** 字段。</span><span class="sxs-lookup"><span data-stu-id="752c5-105">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="752c5-106">基于唯一发件人的 SMTP 地址，邮箱支持的最大替代数目为 1000 个。</span><span class="sxs-lookup"><span data-stu-id="752c5-106">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="752c5-107">POST 操作仅支持一次创建一个替代。</span><span class="sxs-lookup"><span data-stu-id="752c5-107">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="752c5-108">权限</span><span class="sxs-lookup"><span data-stu-id="752c5-108">Permissions</span></span>
<span data-ttu-id="752c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="752c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="752c5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="752c5-111">Permission type</span></span>      | <span data-ttu-id="752c5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="752c5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="752c5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="752c5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="752c5-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="752c5-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="752c5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="752c5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="752c5-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="752c5-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="752c5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="752c5-117">Application</span></span> | <span data-ttu-id="752c5-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="752c5-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="752c5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="752c5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="752c5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="752c5-120">Request headers</span></span>
| <span data-ttu-id="752c5-121">名称</span><span class="sxs-lookup"><span data-stu-id="752c5-121">Name</span></span>       | <span data-ttu-id="752c5-122">类型</span><span class="sxs-lookup"><span data-stu-id="752c5-122">Type</span></span> | <span data-ttu-id="752c5-123">说明</span><span class="sxs-lookup"><span data-stu-id="752c5-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="752c5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="752c5-124">Authorization</span></span>  | <span data-ttu-id="752c5-125">string</span><span class="sxs-lookup"><span data-stu-id="752c5-125">string</span></span>  | <span data-ttu-id="752c5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="752c5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="752c5-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="752c5-128">Content-Type</span></span> | <span data-ttu-id="752c5-129">string</span><span class="sxs-lookup"><span data-stu-id="752c5-129">string</span></span>  | <span data-ttu-id="752c5-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="752c5-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="752c5-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="752c5-132">Request body</span></span>
<span data-ttu-id="752c5-133">在请求正文中，提供 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="752c5-133">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="752c5-134">响应</span><span class="sxs-lookup"><span data-stu-id="752c5-134">Response</span></span>

<span data-ttu-id="752c5-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="752c5-135">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="752c5-136">示例</span><span class="sxs-lookup"><span data-stu-id="752c5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="752c5-137">请求</span><span class="sxs-lookup"><span data-stu-id="752c5-137">Request</span></span>
<span data-ttu-id="752c5-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="752c5-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="752c5-139">响应</span><span class="sxs-lookup"><span data-stu-id="752c5-139">Response</span></span>
<span data-ttu-id="752c5-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="752c5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->