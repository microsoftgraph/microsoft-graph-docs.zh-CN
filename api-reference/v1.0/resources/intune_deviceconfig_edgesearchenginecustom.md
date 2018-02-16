# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="5cbb1-101">edgeSearchEngineCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cbb1-101">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="5cbb1-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5cbb1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cbb1-103">允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="5cbb1-103">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="5cbb1-104">继承自 [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="5cbb1-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5cbb1-105">属性</span><span class="sxs-lookup"><span data-stu-id="5cbb1-105">Properties</span></span>
|<span data-ttu-id="5cbb1-106">属性</span><span class="sxs-lookup"><span data-stu-id="5cbb1-106">Property</span></span>|<span data-ttu-id="5cbb1-107">类型</span><span class="sxs-lookup"><span data-stu-id="5cbb1-107">Type</span></span>|<span data-ttu-id="5cbb1-108">说明</span><span class="sxs-lookup"><span data-stu-id="5cbb1-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cbb1-109">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="5cbb1-109">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="5cbb1-110">String</span><span class="sxs-lookup"><span data-stu-id="5cbb1-110">String</span></span>|<span data-ttu-id="5cbb1-111">指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。</span><span class="sxs-lookup"><span data-stu-id="5cbb1-111">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cbb1-112">关系</span><span class="sxs-lookup"><span data-stu-id="5cbb1-112">Relationships</span></span>
<span data-ttu-id="5cbb1-113">无</span><span class="sxs-lookup"><span data-stu-id="5cbb1-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5cbb1-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cbb1-114">JSON Representation</span></span>
<span data-ttu-id="5cbb1-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cbb1-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



