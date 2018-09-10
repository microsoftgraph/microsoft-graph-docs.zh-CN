# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="dffc8-101">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="dffc8-101">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="dffc8-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dffc8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dffc8-103">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="dffc8-103">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="dffc8-104">属性</span><span class="sxs-lookup"><span data-stu-id="dffc8-104">Properties</span></span>
|<span data-ttu-id="dffc8-105">属性</span><span class="sxs-lookup"><span data-stu-id="dffc8-105">Property</span></span>|<span data-ttu-id="dffc8-106">类型</span><span class="sxs-lookup"><span data-stu-id="dffc8-106">Type</span></span>|<span data-ttu-id="dffc8-107">说明</span><span class="sxs-lookup"><span data-stu-id="dffc8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dffc8-108">displayName</span><span class="sxs-lookup"><span data-stu-id="dffc8-108">displayName</span></span>|<span data-ttu-id="dffc8-109">String</span><span class="sxs-lookup"><span data-stu-id="dffc8-109">String</span></span>|<span data-ttu-id="dffc8-110">显示名称</span><span class="sxs-lookup"><span data-stu-id="dffc8-110">Display name</span></span>|
|<span data-ttu-id="dffc8-111">资源</span><span class="sxs-lookup"><span data-stu-id="dffc8-111">resources</span></span>|<span data-ttu-id="dffc8-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="dffc8-112">String collection</span></span>|<span data-ttu-id="dffc8-113">资源集合</span><span class="sxs-lookup"><span data-stu-id="dffc8-113">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="dffc8-114">关系</span><span class="sxs-lookup"><span data-stu-id="dffc8-114">Relationships</span></span>
<span data-ttu-id="dffc8-115">无</span><span class="sxs-lookup"><span data-stu-id="dffc8-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dffc8-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dffc8-116">JSON Representation</span></span>
<span data-ttu-id="dffc8-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dffc8-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```








