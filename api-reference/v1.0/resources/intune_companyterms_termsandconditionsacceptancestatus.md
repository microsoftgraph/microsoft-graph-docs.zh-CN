# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="81f06-101">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="81f06-101">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="81f06-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="81f06-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81f06-103">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="81f06-103">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="81f06-104">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="81f06-104">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="81f06-105">方法</span><span class="sxs-lookup"><span data-stu-id="81f06-105">Methods</span></span>
|<span data-ttu-id="81f06-106">方法</span><span class="sxs-lookup"><span data-stu-id="81f06-106">Method</span></span>|<span data-ttu-id="81f06-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="81f06-107">Return Type</span></span>|<span data-ttu-id="81f06-108">说明</span><span class="sxs-lookup"><span data-stu-id="81f06-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81f06-109">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="81f06-109">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|<span data-ttu-id="81f06-110">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81f06-110">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="81f06-111">列出 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81f06-111">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="81f06-112">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="81f06-112">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[<span data-ttu-id="81f06-113">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="81f06-113">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="81f06-114">读取 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81f06-114">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="81f06-115">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="81f06-115">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[<span data-ttu-id="81f06-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="81f06-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="81f06-117">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81f06-117">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="81f06-118">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="81f06-118">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|<span data-ttu-id="81f06-119">无</span><span class="sxs-lookup"><span data-stu-id="81f06-119">None</span></span>|<span data-ttu-id="81f06-120">删除 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="81f06-120">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="81f06-121">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="81f06-121">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[<span data-ttu-id="81f06-122">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="81f06-122">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="81f06-123">更新 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="81f06-123">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81f06-124">属性</span><span class="sxs-lookup"><span data-stu-id="81f06-124">Properties</span></span>
|<span data-ttu-id="81f06-125">属性</span><span class="sxs-lookup"><span data-stu-id="81f06-125">Property</span></span>|<span data-ttu-id="81f06-126">类型</span><span class="sxs-lookup"><span data-stu-id="81f06-126">Type</span></span>|<span data-ttu-id="81f06-127">说明</span><span class="sxs-lookup"><span data-stu-id="81f06-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f06-128">ID</span><span class="sxs-lookup"><span data-stu-id="81f06-128">id</span></span>|<span data-ttu-id="81f06-129">字符串</span><span class="sxs-lookup"><span data-stu-id="81f06-129">String</span></span>|<span data-ttu-id="81f06-130">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="81f06-130">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="81f06-131">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="81f06-131">userDisplayName</span></span>|<span data-ttu-id="81f06-132">String</span><span class="sxs-lookup"><span data-stu-id="81f06-132">String</span></span>|<span data-ttu-id="81f06-133">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="81f06-133">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="81f06-134">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="81f06-134">acceptedVersion</span></span>|<span data-ttu-id="81f06-135">Int32</span><span class="sxs-lookup"><span data-stu-id="81f06-135">Int32</span></span>|<span data-ttu-id="81f06-136">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="81f06-136">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="81f06-137">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="81f06-137">acceptedDateTime</span></span>|<span data-ttu-id="81f06-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81f06-138">DateTimeOffset</span></span>|<span data-ttu-id="81f06-139">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="81f06-139">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81f06-140">关系</span><span class="sxs-lookup"><span data-stu-id="81f06-140">Relationships</span></span>
|<span data-ttu-id="81f06-141">关系</span><span class="sxs-lookup"><span data-stu-id="81f06-141">Relationship</span></span>|<span data-ttu-id="81f06-142">类型</span><span class="sxs-lookup"><span data-stu-id="81f06-142">Type</span></span>|<span data-ttu-id="81f06-143">说明</span><span class="sxs-lookup"><span data-stu-id="81f06-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f06-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="81f06-144">termsAndConditions</span></span>|[<span data-ttu-id="81f06-145">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="81f06-145">termsAndConditions</span></span>](../resources/intune_companyterms_termsandconditions.md)|<span data-ttu-id="81f06-146">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="81f06-146">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81f06-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81f06-147">JSON Representation</span></span>
<span data-ttu-id="81f06-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81f06-148">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```








