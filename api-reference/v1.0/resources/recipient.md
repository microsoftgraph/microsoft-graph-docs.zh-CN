# <a name="recipient-resource-type"></a><span data-ttu-id="acb5b-101">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="acb5b-101">recipient resource type</span></span>

<span data-ttu-id="acb5b-102">表示事件、邮件或组帖子发送或接收端的用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="acb5b-102">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="acb5b-103">属性</span><span class="sxs-lookup"><span data-stu-id="acb5b-103">Properties</span></span>
| <span data-ttu-id="acb5b-104">属性</span><span class="sxs-lookup"><span data-stu-id="acb5b-104">Property</span></span>     | <span data-ttu-id="acb5b-105">类型</span><span class="sxs-lookup"><span data-stu-id="acb5b-105">Type</span></span>   |<span data-ttu-id="acb5b-106">说明</span><span class="sxs-lookup"><span data-stu-id="acb5b-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acb5b-107">emailAddress</span><span class="sxs-lookup"><span data-stu-id="acb5b-107">emailAddress</span></span>|[<span data-ttu-id="acb5b-108">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="acb5b-108">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="acb5b-109">收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="acb5b-109">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acb5b-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acb5b-110">JSON representation</span></span>

<span data-ttu-id="acb5b-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acb5b-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->