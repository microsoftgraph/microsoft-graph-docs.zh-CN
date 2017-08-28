# <a name="emailaddress-resource-type"></a><span data-ttu-id="05c0e-101">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="05c0e-101">emailAddress resource type</span></span>

<span data-ttu-id="05c0e-102">联系人或邮件收件人的姓名和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="05c0e-102">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="05c0e-103">属性</span><span class="sxs-lookup"><span data-stu-id="05c0e-103">Properties</span></span>
| <span data-ttu-id="05c0e-104">属性</span><span class="sxs-lookup"><span data-stu-id="05c0e-104">Property</span></span>     | <span data-ttu-id="05c0e-105">类型</span><span class="sxs-lookup"><span data-stu-id="05c0e-105">Type</span></span>   |<span data-ttu-id="05c0e-106">说明</span><span class="sxs-lookup"><span data-stu-id="05c0e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05c0e-107">address</span><span class="sxs-lookup"><span data-stu-id="05c0e-107">address</span></span>|<span data-ttu-id="05c0e-108">String</span><span class="sxs-lookup"><span data-stu-id="05c0e-108">String</span></span>|<span data-ttu-id="05c0e-109">人员或实体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="05c0e-109">The email address of the person or entity.</span></span>|
|<span data-ttu-id="05c0e-110">name</span><span class="sxs-lookup"><span data-stu-id="05c0e-110">name</span></span>|<span data-ttu-id="05c0e-111">String</span><span class="sxs-lookup"><span data-stu-id="05c0e-111">String</span></span>|<span data-ttu-id="05c0e-112">人员或实体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="05c0e-112">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05c0e-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05c0e-113">JSON representation</span></span>

<span data-ttu-id="05c0e-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05c0e-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
