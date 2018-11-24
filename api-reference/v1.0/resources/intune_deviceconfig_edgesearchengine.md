# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="f96f3-101">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="f96f3-101">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="f96f3-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f96f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f96f3-103">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="f96f3-103">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="f96f3-104">继承自 [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="f96f3-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f96f3-105">属性</span><span class="sxs-lookup"><span data-stu-id="f96f3-105">Properties</span></span>
|<span data-ttu-id="f96f3-106">属性</span><span class="sxs-lookup"><span data-stu-id="f96f3-106">Property</span></span>|<span data-ttu-id="f96f3-107">类型</span><span class="sxs-lookup"><span data-stu-id="f96f3-107">Type</span></span>|<span data-ttu-id="f96f3-108">说明</span><span class="sxs-lookup"><span data-stu-id="f96f3-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f96f3-109">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f96f3-109">edgeSearchEngineType</span></span>|[<span data-ttu-id="f96f3-110">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f96f3-110">edgeSearchEngineType</span></span>](../resources/intune_deviceconfig_edgesearchenginetype.md)|<span data-ttu-id="f96f3-111">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="f96f3-111">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="f96f3-112">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="f96f3-112">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f96f3-113">Relationships</span><span class="sxs-lookup"><span data-stu-id="f96f3-113">Relationships</span></span>
<span data-ttu-id="f96f3-114">无</span><span class="sxs-lookup"><span data-stu-id="f96f3-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f96f3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f96f3-115">JSON Representation</span></span>
<span data-ttu-id="f96f3-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f96f3-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



