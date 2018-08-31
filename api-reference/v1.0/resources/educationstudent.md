# <a name="educationstudent-resource-type"></a><span data-ttu-id="c47a9-101">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c47a9-101">educationStudent resource type</span></span>

<span data-ttu-id="c47a9-102">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="c47a9-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="c47a9-103">属性</span><span class="sxs-lookup"><span data-stu-id="c47a9-103">Properties</span></span>
| <span data-ttu-id="c47a9-104">属性</span><span class="sxs-lookup"><span data-stu-id="c47a9-104">Property</span></span>     | <span data-ttu-id="c47a9-105">类型</span><span class="sxs-lookup"><span data-stu-id="c47a9-105">Type</span></span>   |<span data-ttu-id="c47a9-106">说明</span><span class="sxs-lookup"><span data-stu-id="c47a9-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c47a9-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="c47a9-107">birthDate</span></span>|<span data-ttu-id="c47a9-108">日期</span><span class="sxs-lookup"><span data-stu-id="c47a9-108">Date</span></span>| <span data-ttu-id="c47a9-109">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="c47a9-109">Birth date of the student.</span></span>|
|<span data-ttu-id="c47a9-110">externalId</span><span class="sxs-lookup"><span data-stu-id="c47a9-110">externalId</span></span>|<span data-ttu-id="c47a9-111">字符串</span><span class="sxs-lookup"><span data-stu-id="c47a9-111">String</span></span>| <span data-ttu-id="c47a9-112">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="c47a9-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="c47a9-113">性别</span><span class="sxs-lookup"><span data-stu-id="c47a9-113">gender</span></span>|<span data-ttu-id="c47a9-114">educationGender</span><span class="sxs-lookup"><span data-stu-id="c47a9-114">educationGender values</span></span>| <span data-ttu-id="c47a9-115">可取值为：`female`、`male`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c47a9-115">The possible values are `female`, `male`, `other`, `unknownFutureValue`, , , , , , , , or .</span></span>|
|<span data-ttu-id="c47a9-116">年级</span><span class="sxs-lookup"><span data-stu-id="c47a9-116">grade</span></span>|<span data-ttu-id="c47a9-117">字符串</span><span class="sxs-lookup"><span data-stu-id="c47a9-117">String</span></span>|<span data-ttu-id="c47a9-118">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="c47a9-118">Current grade level of the student.</span></span>|
|<span data-ttu-id="c47a9-119">graduationYear</span><span class="sxs-lookup"><span data-stu-id="c47a9-119">graduationYear</span></span>|<span data-ttu-id="c47a9-120">字符串</span><span class="sxs-lookup"><span data-stu-id="c47a9-120">String</span></span>| <span data-ttu-id="c47a9-121">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="c47a9-121">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="c47a9-122">studentNumber</span><span class="sxs-lookup"><span data-stu-id="c47a9-122">studentNumber</span></span>|<span data-ttu-id="c47a9-123">字符串</span><span class="sxs-lookup"><span data-stu-id="c47a9-123">String</span></span>| <span data-ttu-id="c47a9-124">学生编号。</span><span class="sxs-lookup"><span data-stu-id="c47a9-124">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c47a9-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c47a9-125">JSON representation</span></span>

<span data-ttu-id="c47a9-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c47a9-126">The following is a JSON representation of the resource.</span></span>

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
