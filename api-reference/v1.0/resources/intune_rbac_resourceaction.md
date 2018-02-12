# <a name="resourceaction-resource-type"></a><span data-ttu-id="b171f-101">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b171f-101">resourceAction resource type</span></span>

> <span data-ttu-id="b171f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b171f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b171f-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b171f-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b171f-104">属性</span><span class="sxs-lookup"><span data-stu-id="b171f-104">Properties</span></span>
|<span data-ttu-id="b171f-105">属性</span><span class="sxs-lookup"><span data-stu-id="b171f-105">Property</span></span>|<span data-ttu-id="b171f-106">类型</span><span class="sxs-lookup"><span data-stu-id="b171f-106">Type</span></span>|<span data-ttu-id="b171f-107">说明</span><span class="sxs-lookup"><span data-stu-id="b171f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b171f-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b171f-108">allowedResourceActions</span></span>|<span data-ttu-id="b171f-109">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b171f-109">String collection</span></span>|<span data-ttu-id="b171f-110">允许的操作</span><span class="sxs-lookup"><span data-stu-id="b171f-110">Allowed Actions</span></span>|
|<span data-ttu-id="b171f-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b171f-111">notAllowedResourceActions</span></span>|<span data-ttu-id="b171f-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b171f-112">String collection</span></span>|<span data-ttu-id="b171f-113">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="b171f-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="b171f-114">关系</span><span class="sxs-lookup"><span data-stu-id="b171f-114">Relationships</span></span>
<span data-ttu-id="b171f-115">无</span><span class="sxs-lookup"><span data-stu-id="b171f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b171f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b171f-116">JSON Representation</span></span>
<span data-ttu-id="b171f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b171f-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



