# <a name="omasetting-resource-type"></a><span data-ttu-id="68587-101">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="68587-101">omaSetting resource type</span></span>

> <span data-ttu-id="68587-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="68587-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68587-103">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="68587-103">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="68587-104">属性</span><span class="sxs-lookup"><span data-stu-id="68587-104">Properties</span></span>
|<span data-ttu-id="68587-105">属性</span><span class="sxs-lookup"><span data-stu-id="68587-105">Property</span></span>|<span data-ttu-id="68587-106">类型</span><span class="sxs-lookup"><span data-stu-id="68587-106">Type</span></span>|<span data-ttu-id="68587-107">说明</span><span class="sxs-lookup"><span data-stu-id="68587-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68587-108">displayName</span><span class="sxs-lookup"><span data-stu-id="68587-108">displayName</span></span>|<span data-ttu-id="68587-109">String</span><span class="sxs-lookup"><span data-stu-id="68587-109">String</span></span>|<span data-ttu-id="68587-110">显示名称。</span><span class="sxs-lookup"><span data-stu-id="68587-110">Display Name</span></span>|
|<span data-ttu-id="68587-111">description</span><span class="sxs-lookup"><span data-stu-id="68587-111">description</span></span>|<span data-ttu-id="68587-112">String</span><span class="sxs-lookup"><span data-stu-id="68587-112">String</span></span>|<span data-ttu-id="68587-113">说明。</span><span class="sxs-lookup"><span data-stu-id="68587-113">Description.</span></span>|
|<span data-ttu-id="68587-114">omaUri</span><span class="sxs-lookup"><span data-stu-id="68587-114">omaUri</span></span>|<span data-ttu-id="68587-115">String</span><span class="sxs-lookup"><span data-stu-id="68587-115">String</span></span>|<span data-ttu-id="68587-116">OMA。</span><span class="sxs-lookup"><span data-stu-id="68587-116">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68587-117">关系</span><span class="sxs-lookup"><span data-stu-id="68587-117">Relationships</span></span>
<span data-ttu-id="68587-118">无</span><span class="sxs-lookup"><span data-stu-id="68587-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68587-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68587-119">JSON Representation</span></span>
<span data-ttu-id="68587-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68587-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



