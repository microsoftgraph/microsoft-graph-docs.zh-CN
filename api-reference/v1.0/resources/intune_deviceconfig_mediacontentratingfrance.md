# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="b7e3b-101">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7e3b-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="b7e3b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b7e3b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7e3b-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b7e3b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b7e3b-104">属性</span><span class="sxs-lookup"><span data-stu-id="b7e3b-104">Properties</span></span>
|<span data-ttu-id="b7e3b-105">属性</span><span class="sxs-lookup"><span data-stu-id="b7e3b-105">Property</span></span>|<span data-ttu-id="b7e3b-106">类型</span><span class="sxs-lookup"><span data-stu-id="b7e3b-106">Type</span></span>|<span data-ttu-id="b7e3b-107">说明</span><span class="sxs-lookup"><span data-stu-id="b7e3b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7e3b-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7e3b-108">movieRating</span></span>|[<span data-ttu-id="b7e3b-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7e3b-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="b7e3b-110">法国分级所选的影片。</span><span class="sxs-lookup"><span data-stu-id="b7e3b-110">Movies rating selected for France.</span></span> <span data-ttu-id="b7e3b-111">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b7e3b-111">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b7e3b-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7e3b-112">tvRating</span></span>|[<span data-ttu-id="b7e3b-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7e3b-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="b7e3b-114">选择法国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="b7e3b-114">TV rating selected for France.</span></span> <span data-ttu-id="b7e3b-115">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b7e3b-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7e3b-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="b7e3b-116">Relationships</span></span>
<span data-ttu-id="b7e3b-117">无</span><span class="sxs-lookup"><span data-stu-id="b7e3b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7e3b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7e3b-118">JSON Representation</span></span>
<span data-ttu-id="b7e3b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7e3b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



