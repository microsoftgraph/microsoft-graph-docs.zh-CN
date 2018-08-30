# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="2e49c-101">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e49c-101">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="2e49c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2e49c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e49c-103">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="2e49c-103">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="2e49c-104">继承自 [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="2e49c-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e49c-105">属性</span><span class="sxs-lookup"><span data-stu-id="2e49c-105">Properties</span></span>
|<span data-ttu-id="2e49c-106">属性</span><span class="sxs-lookup"><span data-stu-id="2e49c-106">Property</span></span>|<span data-ttu-id="2e49c-107">类型</span><span class="sxs-lookup"><span data-stu-id="2e49c-107">Type</span></span>|<span data-ttu-id="2e49c-108">说明</span><span class="sxs-lookup"><span data-stu-id="2e49c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e49c-109">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2e49c-109">edgeSearchEngineType</span></span>|[<span data-ttu-id="2e49c-110">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2e49c-110">edgeSearchEngineType</span></span>](../resources/intune_deviceconfig_edgesearchenginetype.md)|<span data-ttu-id="2e49c-111">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="2e49c-111">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="2e49c-112">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="2e49c-112">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e49c-113">关系</span><span class="sxs-lookup"><span data-stu-id="2e49c-113">Relationships</span></span>
<span data-ttu-id="2e49c-114">无</span><span class="sxs-lookup"><span data-stu-id="2e49c-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e49c-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e49c-115">JSON Representation</span></span>
<span data-ttu-id="2e49c-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e49c-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.edgeSearchEngineBase",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



