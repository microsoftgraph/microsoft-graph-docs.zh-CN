# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="c115c-101">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="c115c-101">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="c115c-102"> [user](user.md) 实体的 **onPremisesExtensionAttributes** 属性包含 15 个自定义扩展特性的属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-102">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="c115c-103">对于 **onPremisesSyncEnabled** 用户，此组属性是在本地 Active Directory 中主控并以只读方式同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="c115c-103">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="c115c-104">对于仅限云的用户（其 **onPremisesSyncEnabled** 为 false），这些属性可以在创建过程中设置或更新。</span><span class="sxs-lookup"><span data-stu-id="c115c-104">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="c115c-105">属性</span><span class="sxs-lookup"><span data-stu-id="c115c-105">Properties</span></span>
| <span data-ttu-id="c115c-106">属性</span><span class="sxs-lookup"><span data-stu-id="c115c-106">Property</span></span>     | <span data-ttu-id="c115c-107">类型</span><span class="sxs-lookup"><span data-stu-id="c115c-107">Type</span></span>   |<span data-ttu-id="c115c-108">说明</span><span class="sxs-lookup"><span data-stu-id="c115c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c115c-109">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="c115c-109">extensionAttribute1</span></span>|<span data-ttu-id="c115c-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-110">String</span></span>| <span data-ttu-id="c115c-111">第一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-111">First customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-112">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="c115c-112">extensionAttribute2</span></span>|<span data-ttu-id="c115c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-113">String</span></span>| <span data-ttu-id="c115c-114">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-114">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-115">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="c115c-115">extensionAttribute3</span></span>|<span data-ttu-id="c115c-116">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-116">String</span></span>| <span data-ttu-id="c115c-117">第三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-117">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-118">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="c115c-118">extensionAttribute4</span></span>|<span data-ttu-id="c115c-119">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-119">String</span></span>| <span data-ttu-id="c115c-120">第四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-120">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-121">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="c115c-121">extensionAttribute5</span></span>|<span data-ttu-id="c115c-122">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-122">String</span></span>| <span data-ttu-id="c115c-123">第五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-123">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-124">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="c115c-124">extensionAttribute6</span></span>|<span data-ttu-id="c115c-125">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-125">String</span></span>| <span data-ttu-id="c115c-126">第六个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-126">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-127">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="c115c-127">extensionAttribute7</span></span>|<span data-ttu-id="c115c-128">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-128">String</span></span>| <span data-ttu-id="c115c-129">第七个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-129">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-130">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="c115c-130">extensionAttribute8</span></span>|<span data-ttu-id="c115c-131">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-131">String</span></span>| <span data-ttu-id="c115c-132">第八个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-132">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-133">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="c115c-133">extensionAttribute9</span></span>|<span data-ttu-id="c115c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-134">String</span></span>| <span data-ttu-id="c115c-135">第九个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-135">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-136">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="c115c-136">extensionAttribute10</span></span>|<span data-ttu-id="c115c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-137">String</span></span>| <span data-ttu-id="c115c-138">第十个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-138">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-139">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="c115c-139">extensionAttribute11</span></span>|<span data-ttu-id="c115c-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-140">String</span></span>| <span data-ttu-id="c115c-141">第十一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-141">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-142">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="c115c-142">extensionAttribute12</span></span>|<span data-ttu-id="c115c-143">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-143">String</span></span>| <span data-ttu-id="c115c-144">第十二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-144">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-145">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="c115c-145">extensionAttribute13</span></span>|<span data-ttu-id="c115c-146">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-146">String</span></span>| <span data-ttu-id="c115c-147">第十三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-147">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-148">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="c115c-148">extensionAttribute14</span></span>|<span data-ttu-id="c115c-149">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-149">String</span></span>| <span data-ttu-id="c115c-150">第十四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-150">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c115c-151">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="c115c-151">extensionAttribute15</span></span>|<span data-ttu-id="c115c-152">字符串</span><span class="sxs-lookup"><span data-stu-id="c115c-152">String</span></span>| <span data-ttu-id="c115c-153">第十五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c115c-153">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c115c-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c115c-154">JSON representation</span></span>

<span data-ttu-id="c115c-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c115c-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->