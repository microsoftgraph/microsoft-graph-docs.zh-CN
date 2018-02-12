# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="8bfe8-101">edgeSearchEngineBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bfe8-101">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="8bfe8-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8bfe8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bfe8-103">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="8bfe8-103">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="8bfe8-104">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="8bfe8-104">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="8bfe8-105">属性</span><span class="sxs-lookup"><span data-stu-id="8bfe8-105">Properties</span></span>
|<span data-ttu-id="8bfe8-106">属性</span><span class="sxs-lookup"><span data-stu-id="8bfe8-106">Property</span></span>|<span data-ttu-id="8bfe8-107">类型</span><span class="sxs-lookup"><span data-stu-id="8bfe8-107">Type</span></span>|<span data-ttu-id="8bfe8-108">说明</span><span class="sxs-lookup"><span data-stu-id="8bfe8-108">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="8bfe8-109">关系</span><span class="sxs-lookup"><span data-stu-id="8bfe8-109">Relationships</span></span>
<span data-ttu-id="8bfe8-110">无</span><span class="sxs-lookup"><span data-stu-id="8bfe8-110">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8bfe8-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bfe8-111">JSON Representation</span></span>
<span data-ttu-id="8bfe8-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bfe8-112">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```



