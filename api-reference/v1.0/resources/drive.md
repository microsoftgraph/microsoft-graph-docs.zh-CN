# <a name="drive-resource-type"></a><span data-ttu-id="be2a9-101">驱动器资源类型</span><span class="sxs-lookup"><span data-stu-id="be2a9-101">Drive resource type</span></span>

<span data-ttu-id="be2a9-102">驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="be2a9-102">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="be2a9-p101">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be2a9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be2a9-105">JSON representation</span></span>

<span data-ttu-id="be2a9-106">下面是**驱动器**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be2a9-106">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="be2a9-107">**驱动器**资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="be2a9-107">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special", "owner", "description" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }],

  /* inherited from baseItem */
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="be2a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="be2a9-108">Properties</span></span>

| <span data-ttu-id="be2a9-109">属性</span><span class="sxs-lookup"><span data-stu-id="be2a9-109">Property</span></span>             | <span data-ttu-id="be2a9-110">类型</span><span class="sxs-lookup"><span data-stu-id="be2a9-110">Type</span></span>                          | <span data-ttu-id="be2a9-111">说明</span><span class="sxs-lookup"><span data-stu-id="be2a9-111">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="be2a9-112">id</span><span class="sxs-lookup"><span data-stu-id="be2a9-112">id</span></span>                   | <span data-ttu-id="be2a9-113">String</span><span class="sxs-lookup"><span data-stu-id="be2a9-113">String</span></span>                        | <span data-ttu-id="be2a9-p102">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p102">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="be2a9-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="be2a9-116">createdBy</span></span>            | <span data-ttu-id="be2a9-117">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="be2a9-117">[identitySet][]</span></span>               | <span data-ttu-id="be2a9-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="be2a9-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be2a9-120">createdDateTime</span></span>      | <span data-ttu-id="be2a9-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be2a9-121">dateTimeOffset</span></span>                | <span data-ttu-id="be2a9-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="be2a9-124">driveType</span><span class="sxs-lookup"><span data-stu-id="be2a9-124">driveType</span></span>            | <span data-ttu-id="be2a9-125">String</span><span class="sxs-lookup"><span data-stu-id="be2a9-125">String</span></span>                        | <span data-ttu-id="be2a9-p105">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="be2a9-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="be2a9-131">lastModifiedBy</span></span>       | <span data-ttu-id="be2a9-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="be2a9-132">[identitySet][]</span></span>               | <span data-ttu-id="be2a9-p106">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="be2a9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be2a9-135">lastModifiedDateTime</span></span> | <span data-ttu-id="be2a9-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be2a9-136">dateTimeOffset</span></span>                | <span data-ttu-id="be2a9-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p107">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="be2a9-139">name</span><span class="sxs-lookup"><span data-stu-id="be2a9-139">name</span></span>                 | <span data-ttu-id="be2a9-140">string</span><span class="sxs-lookup"><span data-stu-id="be2a9-140">string</span></span>                        | <span data-ttu-id="be2a9-p108">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p108">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="be2a9-143">所有者</span><span class="sxs-lookup"><span data-stu-id="be2a9-143">owner</span></span>                | [<span data-ttu-id="be2a9-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="be2a9-144">identitySet</span></span>](identityset.md) | <span data-ttu-id="be2a9-p109">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p109">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="be2a9-148">配额</span><span class="sxs-lookup"><span data-stu-id="be2a9-148">quota</span></span>                | [<span data-ttu-id="be2a9-149">配额</span><span class="sxs-lookup"><span data-stu-id="be2a9-149">quota</span></span>](quota.md)             | <span data-ttu-id="be2a9-p110">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p110">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="be2a9-153">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="be2a9-153">sharepointIds</span></span>        | <span data-ttu-id="be2a9-154">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="be2a9-154">[sharepointIds][]</span></span>             | <span data-ttu-id="be2a9-p111">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="be2a9-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="be2a9-157">webUrl</span></span>               | <span data-ttu-id="be2a9-158">string (url)</span><span class="sxs-lookup"><span data-stu-id="be2a9-158">string (url)</span></span>                  | <span data-ttu-id="be2a9-p112">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p112">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

<span data-ttu-id="be2a9-161">[identitySet]: identityset.md</span><span class="sxs-lookup"><span data-stu-id="be2a9-161">[identitySet]: identityset.md</span></span>
<span data-ttu-id="be2a9-162">[sharepointIds]: sharepointids.md</span><span class="sxs-lookup"><span data-stu-id="be2a9-162">[sharepointIds]: sharepointids.md</span></span>

## <a name="relationships"></a><span data-ttu-id="be2a9-163">关系</span><span class="sxs-lookup"><span data-stu-id="be2a9-163">Relationships</span></span>

| <span data-ttu-id="be2a9-164">关系</span><span class="sxs-lookup"><span data-stu-id="be2a9-164">Relationship</span></span> | <span data-ttu-id="be2a9-165">类型</span><span class="sxs-lookup"><span data-stu-id="be2a9-165">Type</span></span>                                 | <span data-ttu-id="be2a9-166">说明</span><span class="sxs-lookup"><span data-stu-id="be2a9-166">Description</span></span>                                                              |
| :----------- | :----------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="be2a9-167">项目</span><span class="sxs-lookup"><span data-stu-id="be2a9-167">items</span></span>        | <span data-ttu-id="be2a9-168">[driveitem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be2a9-168">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="be2a9-p113">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p113">All items contained in the drive. Read-only. Nullable.</span></span>                   |
| <span data-ttu-id="be2a9-172">根</span><span class="sxs-lookup"><span data-stu-id="be2a9-172">root</span></span>         | [<span data-ttu-id="be2a9-173">driveitem</span><span class="sxs-lookup"><span data-stu-id="be2a9-173">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="be2a9-p114">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p114">The root folder of the drive. Read-only.</span></span>                                 |
| <span data-ttu-id="be2a9-176">special</span><span class="sxs-lookup"><span data-stu-id="be2a9-176">special</span></span>      | <span data-ttu-id="be2a9-177">[driveitem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be2a9-177">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="be2a9-p115">OneDrive 中可用的公用文件夹的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="be2a9-p115">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span> |

## <a name="methods"></a><span data-ttu-id="be2a9-181">方法</span><span class="sxs-lookup"><span data-stu-id="be2a9-181">Methods</span></span>

<span data-ttu-id="be2a9-182">下列方法均可用于驱动器资源。</span><span class="sxs-lookup"><span data-stu-id="be2a9-182">The following methods are available for drive resources.</span></span>

| <span data-ttu-id="be2a9-183">方法</span><span class="sxs-lookup"><span data-stu-id="be2a9-183">Method</span></span>                                                | <span data-ttu-id="be2a9-184">REST 路径</span><span class="sxs-lookup"><span data-stu-id="be2a9-184">REST Path</span></span>                        |
| :---------------------------------------------------- | :------------------------------- |
| [<span data-ttu-id="be2a9-185">获取用户的默认驱动器</span><span class="sxs-lookup"><span data-stu-id="be2a9-185">Get user's default drive</span></span>](../api/drive_get.md)       | `GET /me/drive`                  |
| [<span data-ttu-id="be2a9-186">获取其他用户的驱动器</span><span class="sxs-lookup"><span data-stu-id="be2a9-186">Get another user's drive</span></span>](../api/drive_get.md)       | `GET /users/{user-id}/drive`     |
| [<span data-ttu-id="be2a9-187">获取驱动器的根文件夹</span><span class="sxs-lookup"><span data-stu-id="be2a9-187">Get root folder for a drive</span></span>](../api/item_get.md)     | `GET /drives/{drive-id}/root`    |
| [<span data-ttu-id="be2a9-188">列出驱动器中的项目</span><span class="sxs-lookup"><span data-stu-id="be2a9-188">List items in a drive</span></span>](../api/item_list_children.md) | `GET /me/drive/root/children`    |
| [<span data-ttu-id="be2a9-189">列出驱动器中的更改</span><span class="sxs-lookup"><span data-stu-id="be2a9-189">List changes in a drive</span></span>](../api/item_delta.md)       | `GET /me/drive/root/delta`       |
| [<span data-ttu-id="be2a9-190">搜索驱动器中的项目</span><span class="sxs-lookup"><span data-stu-id="be2a9-190">Search items in a drive</span></span>](../api/item_search.md)      | `GET /me/drive/search(q='text')` |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
