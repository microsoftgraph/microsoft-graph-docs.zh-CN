# <a name="mimecontent-resource-type"></a><span data-ttu-id="b3b34-101">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3b34-101">mimeContent resource type</span></span>

> <span data-ttu-id="b3b34-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3b34-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3b34-103">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="b3b34-103">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="b3b34-104">属性</span><span class="sxs-lookup"><span data-stu-id="b3b34-104">Properties</span></span>
|<span data-ttu-id="b3b34-105">属性</span><span class="sxs-lookup"><span data-stu-id="b3b34-105">Property</span></span>|<span data-ttu-id="b3b34-106">类型</span><span class="sxs-lookup"><span data-stu-id="b3b34-106">Type</span></span>|<span data-ttu-id="b3b34-107">说明</span><span class="sxs-lookup"><span data-stu-id="b3b34-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3b34-108">类型</span><span class="sxs-lookup"><span data-stu-id="b3b34-108">type</span></span>|<span data-ttu-id="b3b34-109">String</span><span class="sxs-lookup"><span data-stu-id="b3b34-109">String</span></span>|<span data-ttu-id="b3b34-110">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="b3b34-110">Indicates the content mime type.</span></span>|
|<span data-ttu-id="b3b34-111">值</span><span class="sxs-lookup"><span data-stu-id="b3b34-111">value</span></span>|<span data-ttu-id="b3b34-112">Binary</span><span class="sxs-lookup"><span data-stu-id="b3b34-112">Binary</span></span>|<span data-ttu-id="b3b34-113">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="b3b34-113">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3b34-114">关系</span><span class="sxs-lookup"><span data-stu-id="b3b34-114">Relationships</span></span>
<span data-ttu-id="b3b34-115">无</span><span class="sxs-lookup"><span data-stu-id="b3b34-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3b34-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3b34-116">JSON Representation</span></span>
<span data-ttu-id="b3b34-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3b34-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



