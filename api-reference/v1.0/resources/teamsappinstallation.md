# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="d242c-101">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d242c-101">teamsAppInstallation resource type</span></span>



<span data-ttu-id="d242c-102">安装在[工作组](team.md) [teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="d242c-102">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="d242c-103">应用程序一部分的任何 bot 将成为应用程序添加到任何工作组的一部分。</span><span class="sxs-lookup"><span data-stu-id="d242c-103">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="d242c-104">方法</span><span class="sxs-lookup"><span data-stu-id="d242c-104">Methods</span></span>

| <span data-ttu-id="d242c-105">方法</span><span class="sxs-lookup"><span data-stu-id="d242c-105">Method</span></span>       | <span data-ttu-id="d242c-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="d242c-106">Return Type</span></span>  |<span data-ttu-id="d242c-107">说明</span><span class="sxs-lookup"><span data-stu-id="d242c-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d242c-108">列表应用程序</span><span class="sxs-lookup"><span data-stu-id="d242c-108">List apps</span></span>](../api/teamsappinstallation_list.md) | [<span data-ttu-id="d242c-109">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d242c-109">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="d242c-110">列出了安装团队中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d242c-110">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="d242c-111">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="d242c-111">Add app</span></span>](../api/teamsappinstallation_add.md) | [<span data-ttu-id="d242c-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d242c-112">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="d242c-113">将 （安装） 添加到团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="d242c-113">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="d242c-114">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="d242c-114">Remove app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="d242c-115">无</span><span class="sxs-lookup"><span data-stu-id="d242c-115">None</span></span> | <span data-ttu-id="d242c-116">删除 （卸载） 从团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="d242c-116">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="d242c-117">升级的应用程序</span><span class="sxs-lookup"><span data-stu-id="d242c-117">Upgrade app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="d242c-118">无</span><span class="sxs-lookup"><span data-stu-id="d242c-118">None</span></span> | <span data-ttu-id="d242c-119">升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d242c-119">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="d242c-120">属性</span><span class="sxs-lookup"><span data-stu-id="d242c-120">Properties</span></span>

| <span data-ttu-id="d242c-121">属性</span><span class="sxs-lookup"><span data-stu-id="d242c-121">Property</span></span>            | <span data-ttu-id="d242c-122">类型</span><span class="sxs-lookup"><span data-stu-id="d242c-122">Type</span></span>     | <span data-ttu-id="d242c-123">说明</span><span class="sxs-lookup"><span data-stu-id="d242c-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d242c-124">ID</span><span class="sxs-lookup"><span data-stu-id="d242c-124">id</span></span>                  | <span data-ttu-id="d242c-125">string</span><span class="sxs-lookup"><span data-stu-id="d242c-125">string</span></span>   | <span data-ttu-id="d242c-126">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="d242c-126">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d242c-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="d242c-127">Relationships</span></span>

| <span data-ttu-id="d242c-128">关系</span><span class="sxs-lookup"><span data-stu-id="d242c-128">Relationship</span></span>   | <span data-ttu-id="d242c-129">类型</span><span class="sxs-lookup"><span data-stu-id="d242c-129">Type</span></span>    | <span data-ttu-id="d242c-130">说明</span><span class="sxs-lookup"><span data-stu-id="d242c-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d242c-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d242c-131">teamsApp</span></span>|[<span data-ttu-id="d242c-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d242c-132">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="d242c-133">安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="d242c-133">The app that is installed.</span></span> |
|<span data-ttu-id="d242c-134">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d242c-134">teamsAppDefinition</span></span>|[<span data-ttu-id="d242c-135">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d242c-135">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="d242c-136">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d242c-136">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d242c-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d242c-137">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="d242c-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d242c-138">See also</span></span>

- [<span data-ttu-id="d242c-139">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d242c-139">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d242c-140">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d242c-140">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d242c-141">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d242c-141">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

