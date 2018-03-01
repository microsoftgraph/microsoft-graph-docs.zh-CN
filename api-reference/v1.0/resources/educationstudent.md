# <a name="educationstudent-resource-type"></a><span data-ttu-id="12cd5-101">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="12cd5-101">educationStudent resource type</span></span>

<span data-ttu-id="12cd5-102">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="12cd5-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="12cd5-103">属性</span><span class="sxs-lookup"><span data-stu-id="12cd5-103">Properties</span></span>
| <span data-ttu-id="12cd5-104">属性</span><span class="sxs-lookup"><span data-stu-id="12cd5-104">Property</span></span>     | <span data-ttu-id="12cd5-105">类型</span><span class="sxs-lookup"><span data-stu-id="12cd5-105">Type</span></span>   |<span data-ttu-id="12cd5-106">说明</span><span class="sxs-lookup"><span data-stu-id="12cd5-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12cd5-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="12cd5-107">birthDate</span></span>|<span data-ttu-id="12cd5-108">Date</span><span class="sxs-lookup"><span data-stu-id="12cd5-108">Date</span></span>| <span data-ttu-id="12cd5-109">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="12cd5-109">Birth date of the student.</span></span>|
|<span data-ttu-id="12cd5-110">externalId</span><span class="sxs-lookup"><span data-stu-id="12cd5-110">externalId</span></span>|<span data-ttu-id="12cd5-111">String</span><span class="sxs-lookup"><span data-stu-id="12cd5-111">String</span></span>| <span data-ttu-id="12cd5-112">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="12cd5-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="12cd5-113">gender</span><span class="sxs-lookup"><span data-stu-id="12cd5-113">Gender</span></span>|`educationGender enumeration`| <span data-ttu-id="12cd5-114">可取值为：`female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="12cd5-114">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="12cd5-115">grade</span><span class="sxs-lookup"><span data-stu-id="12cd5-115">QuizInfoPage: grade</span></span>|<span data-ttu-id="12cd5-116">String</span><span class="sxs-lookup"><span data-stu-id="12cd5-116">String</span></span>|<span data-ttu-id="12cd5-117">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="12cd5-117">Current grade level of the student.</span></span>|
|<span data-ttu-id="12cd5-118">graduationYear</span><span class="sxs-lookup"><span data-stu-id="12cd5-118">graduationYear</span></span>|<span data-ttu-id="12cd5-119">String</span><span class="sxs-lookup"><span data-stu-id="12cd5-119">String</span></span>| <span data-ttu-id="12cd5-120">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="12cd5-120">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="12cd5-121">studentNumber</span><span class="sxs-lookup"><span data-stu-id="12cd5-121">studentNumber</span></span>|<span data-ttu-id="12cd5-122">String</span><span class="sxs-lookup"><span data-stu-id="12cd5-122">String</span></span>| <span data-ttu-id="12cd5-123">学生编号。</span><span class="sxs-lookup"><span data-stu-id="12cd5-123">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12cd5-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12cd5-124">JSON representation</span></span>

<span data-ttu-id="12cd5-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12cd5-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->