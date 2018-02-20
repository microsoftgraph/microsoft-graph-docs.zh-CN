# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="4b86f-101">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b86f-101">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="4b86f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4b86f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b86f-103">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="4b86f-103">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="4b86f-104">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="4b86f-104">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="4b86f-105">方法</span><span class="sxs-lookup"><span data-stu-id="4b86f-105">Methods</span></span>
|<span data-ttu-id="4b86f-106">方法</span><span class="sxs-lookup"><span data-stu-id="4b86f-106">Method</span></span>|<span data-ttu-id="4b86f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b86f-107">Return Type</span></span>|<span data-ttu-id="4b86f-108">说明</span><span class="sxs-lookup"><span data-stu-id="4b86f-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b86f-109">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="4b86f-109">List termsAndConditionsAssignments</span></span>](../api/intune_companyterms_termsandconditionsassignment_list.md)|<span data-ttu-id="4b86f-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b86f-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="4b86f-111">列出 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b86f-111">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="4b86f-112">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4b86f-112">Get termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_get.md)|[<span data-ttu-id="4b86f-113">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4b86f-113">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="4b86f-114">读取 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b86f-114">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="4b86f-115">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4b86f-115">Create termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_create.md)|[<span data-ttu-id="4b86f-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4b86f-116">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="4b86f-117">创建新的 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b86f-117">Create a new [plannerBucket](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="4b86f-118">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4b86f-118">Delete termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_delete.md)|<span data-ttu-id="4b86f-119">无</span><span class="sxs-lookup"><span data-stu-id="4b86f-119">None</span></span>|<span data-ttu-id="4b86f-120">删除 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b86f-120">Deletes a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="4b86f-121">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4b86f-121">Update termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_update.md)|[<span data-ttu-id="4b86f-122">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4b86f-122">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="4b86f-123">更新 [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4b86f-123">Update the properties of a [calendar](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b86f-124">属性</span><span class="sxs-lookup"><span data-stu-id="4b86f-124">Properties</span></span>
|<span data-ttu-id="4b86f-125">属性</span><span class="sxs-lookup"><span data-stu-id="4b86f-125">Property</span></span>|<span data-ttu-id="4b86f-126">类型</span><span class="sxs-lookup"><span data-stu-id="4b86f-126">Type</span></span>|<span data-ttu-id="4b86f-127">说明</span><span class="sxs-lookup"><span data-stu-id="4b86f-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b86f-128">id</span><span class="sxs-lookup"><span data-stu-id="4b86f-128">id</span></span>|<span data-ttu-id="4b86f-129">String</span><span class="sxs-lookup"><span data-stu-id="4b86f-129">String</span></span>|<span data-ttu-id="4b86f-130">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4b86f-130">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="4b86f-131">target</span><span class="sxs-lookup"><span data-stu-id="4b86f-131">target</span></span>|[<span data-ttu-id="4b86f-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4b86f-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_companyterms_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4b86f-133">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="4b86f-133">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b86f-134">关系</span><span class="sxs-lookup"><span data-stu-id="4b86f-134">Relationships</span></span>
<span data-ttu-id="4b86f-135">无</span><span class="sxs-lookup"><span data-stu-id="4b86f-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b86f-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b86f-136">JSON Representation</span></span>
<span data-ttu-id="4b86f-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b86f-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



