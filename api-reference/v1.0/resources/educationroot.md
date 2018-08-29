# <a name="educationroot-resource-type"></a><span data-ttu-id="1feab-101">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="1feab-101">educationRoot resource type</span></span>

<span data-ttu-id="1feab-102">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="1feab-102">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="1feab-103">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="1feab-103">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="1feab-104">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="1feab-104">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="1feab-105">方法</span><span class="sxs-lookup"><span data-stu-id="1feab-105">Methods</span></span>

| <span data-ttu-id="1feab-106">方法</span><span class="sxs-lookup"><span data-stu-id="1feab-106">Method</span></span>           | <span data-ttu-id="1feab-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="1feab-107">Return Type</span></span>    |<span data-ttu-id="1feab-108">说明</span><span class="sxs-lookup"><span data-stu-id="1feab-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1feab-109">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="1feab-109">Create educationClass</span></span>](../api/educationroot_post_classes.md) |[<span data-ttu-id="1feab-110">educationClass</span><span class="sxs-lookup"><span data-stu-id="1feab-110">educationClass</span></span>](educationclass.md)| <span data-ttu-id="1feab-111">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="1feab-111">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="1feab-112">List classes</span><span class="sxs-lookup"><span data-stu-id="1feab-112">List classes</span></span>](../api/educationroot_list_classes.md) |<span data-ttu-id="1feab-113">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1feab-113">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="1feab-114">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1feab-114">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="1feab-115">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="1feab-115">Create educationSchool</span></span>](../api/educationroot_post_schools.md) |[<span data-ttu-id="1feab-116">educationSchool</span><span class="sxs-lookup"><span data-stu-id="1feab-116">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="1feab-117">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="1feab-117">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="1feab-118">List schools</span><span class="sxs-lookup"><span data-stu-id="1feab-118">List schools</span></span>](../api/educationroot_list_schools.md) |<span data-ttu-id="1feab-119">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1feab-119">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="1feab-120">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1feab-120">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="1feab-121">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="1feab-121">Create educationUser</span></span>](../api/educationroot_post_users.md) |[<span data-ttu-id="1feab-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="1feab-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1feab-123">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="1feab-123">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="1feab-124">List users</span><span class="sxs-lookup"><span data-stu-id="1feab-124">List users</span></span>](../api/educationroot_list_users.md) |<span data-ttu-id="1feab-125">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1feab-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="1feab-126">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1feab-126">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1feab-127">属性</span><span class="sxs-lookup"><span data-stu-id="1feab-127">Properties</span></span>
<span data-ttu-id="1feab-128">无。</span><span class="sxs-lookup"><span data-stu-id="1feab-128">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="1feab-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="1feab-129">Relationships</span></span>
| <span data-ttu-id="1feab-130">关系</span><span class="sxs-lookup"><span data-stu-id="1feab-130">Relationship</span></span> | <span data-ttu-id="1feab-131">类型</span><span class="sxs-lookup"><span data-stu-id="1feab-131">Type</span></span>   |<span data-ttu-id="1feab-132">说明</span><span class="sxs-lookup"><span data-stu-id="1feab-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1feab-133">classes</span><span class="sxs-lookup"><span data-stu-id="1feab-133">classes</span></span>|<span data-ttu-id="1feab-134">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1feab-134">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="1feab-p102">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1feab-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="1feab-137">me</span><span class="sxs-lookup"><span data-stu-id="1feab-137">me</span></span>|[<span data-ttu-id="1feab-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="1feab-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1feab-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1feab-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="1feab-141">schools</span><span class="sxs-lookup"><span data-stu-id="1feab-141">schools</span></span>|<span data-ttu-id="1feab-142">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1feab-142">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="1feab-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1feab-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="1feab-145">users</span><span class="sxs-lookup"><span data-stu-id="1feab-145">users</span></span>|<span data-ttu-id="1feab-146">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1feab-146">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="1feab-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1feab-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1feab-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1feab-149">JSON representation</span></span>
<span data-ttu-id="1feab-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1feab-150">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->