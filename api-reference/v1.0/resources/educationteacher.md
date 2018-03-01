# <a name="educationteacher-resource-type"></a><span data-ttu-id="3d784-101">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d784-101">educationTeacher resource type</span></span>

<span data-ttu-id="3d784-102">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="3d784-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="3d784-103">属性</span><span class="sxs-lookup"><span data-stu-id="3d784-103">Properties</span></span>
| <span data-ttu-id="3d784-104">属性</span><span class="sxs-lookup"><span data-stu-id="3d784-104">Property</span></span>     | <span data-ttu-id="3d784-105">类型</span><span class="sxs-lookup"><span data-stu-id="3d784-105">Type</span></span>   |<span data-ttu-id="3d784-106">说明</span><span class="sxs-lookup"><span data-stu-id="3d784-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d784-107">externalId</span><span class="sxs-lookup"><span data-stu-id="3d784-107">externalId</span></span>|<span data-ttu-id="3d784-108">String</span><span class="sxs-lookup"><span data-stu-id="3d784-108">String</span></span>| <span data-ttu-id="3d784-109">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="3d784-109">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="3d784-110">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="3d784-110">teacherNumber</span></span>|<span data-ttu-id="3d784-111">String</span><span class="sxs-lookup"><span data-stu-id="3d784-111">String</span></span>|<span data-ttu-id="3d784-112">教师编号。</span><span class="sxs-lookup"><span data-stu-id="3d784-112">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d784-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d784-113">JSON representation</span></span>

<span data-ttu-id="3d784-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d784-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->