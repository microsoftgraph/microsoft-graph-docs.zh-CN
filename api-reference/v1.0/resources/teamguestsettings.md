# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="35b8e-101">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="35b8e-101">teamGuestSettings resource type</span></span>



<span data-ttu-id="35b8e-102">要配置的是否来宾可以创建、 更新或删除通道[团队](team.md)中的设置。</span><span class="sxs-lookup"><span data-stu-id="35b8e-102">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="35b8e-103">属性</span><span class="sxs-lookup"><span data-stu-id="35b8e-103">Properties</span></span>
| <span data-ttu-id="35b8e-104">属性</span><span class="sxs-lookup"><span data-stu-id="35b8e-104">Property</span></span>     | <span data-ttu-id="35b8e-105">类型</span><span class="sxs-lookup"><span data-stu-id="35b8e-105">Type</span></span>   |<span data-ttu-id="35b8e-106">说明</span><span class="sxs-lookup"><span data-stu-id="35b8e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35b8e-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="35b8e-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="35b8e-108">布尔</span><span class="sxs-lookup"><span data-stu-id="35b8e-108">Boolean</span></span>|<span data-ttu-id="35b8e-109">如果设置为 true，则来宾可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="35b8e-109">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="35b8e-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="35b8e-110">allowDeleteChannels</span></span>|<span data-ttu-id="35b8e-111">布尔</span><span class="sxs-lookup"><span data-stu-id="35b8e-111">Boolean</span></span>|<span data-ttu-id="35b8e-112">如果设置为 true，则来宾可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="35b8e-112">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35b8e-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35b8e-113">JSON representation</span></span>

<span data-ttu-id="35b8e-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35b8e-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
