# <a name="user-resource-type"></a><span data-ttu-id="fab32-101">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="fab32-101">user resource type</span></span>

> <span data-ttu-id="fab32-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fab32-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fab32-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fab32-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="fab32-104">方法</span><span class="sxs-lookup"><span data-stu-id="fab32-104">Methods</span></span>
|<span data-ttu-id="fab32-105">方法</span><span class="sxs-lookup"><span data-stu-id="fab32-105">Method</span></span>|<span data-ttu-id="fab32-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="fab32-106">Return Type</span></span>|<span data-ttu-id="fab32-107">说明</span><span class="sxs-lookup"><span data-stu-id="fab32-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fab32-108">List users</span><span class="sxs-lookup"><span data-stu-id="fab32-108">List users</span></span>](../api/intune_onboarding_user_list.md)|<span data-ttu-id="fab32-109">[user](../resources/intune_onboarding_user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fab32-109">[user](../resources/intune_onboarding_user.md) collection</span></span>|<span data-ttu-id="fab32-110">列出 [user](../resources/intune_onboarding_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fab32-110">List properties and relationships of the [user](../resources/intune_onboarding_user.md) objects.</span></span>|
|[<span data-ttu-id="fab32-111">获取 user</span><span class="sxs-lookup"><span data-stu-id="fab32-111">Get user</span></span>](../api/intune_onboarding_user_get.md)|[<span data-ttu-id="fab32-112">user</span><span class="sxs-lookup"><span data-stu-id="fab32-112">user</span></span>](../resources/intune_onboarding_user.md)|<span data-ttu-id="fab32-113">读取 [user](../resources/intune_onboarding_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fab32-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_onboarding_user.md) object.</span></span>|
|[<span data-ttu-id="fab32-114">创建 user</span><span class="sxs-lookup"><span data-stu-id="fab32-114">Create user</span></span>](../api/intune_onboarding_user_create.md)|[<span data-ttu-id="fab32-115">user</span><span class="sxs-lookup"><span data-stu-id="fab32-115">user</span></span>](../resources/intune_onboarding_user.md)|<span data-ttu-id="fab32-116">创建新的 [user](../resources/intune_onboarding_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fab32-116">Create a new user object.</span></span>|
|[<span data-ttu-id="fab32-117">删除 user</span><span class="sxs-lookup"><span data-stu-id="fab32-117">Delete user</span></span>](../api/intune_onboarding_user_delete.md)|<span data-ttu-id="fab32-118">无</span><span class="sxs-lookup"><span data-stu-id="fab32-118">None</span></span>|<span data-ttu-id="fab32-119">删除 [user](../resources/intune_onboarding_user.md)。</span><span class="sxs-lookup"><span data-stu-id="fab32-119">Deletes a [user](../resources/intune_onboarding_user.md).</span></span>|
|[<span data-ttu-id="fab32-120">更新 user</span><span class="sxs-lookup"><span data-stu-id="fab32-120">Update user</span></span>](../api/intune_onboarding_user_update.md)|[<span data-ttu-id="fab32-121">user</span><span class="sxs-lookup"><span data-stu-id="fab32-121">user</span></span>](../resources/intune_onboarding_user.md)|<span data-ttu-id="fab32-122">更新 [user](../resources/intune_onboarding_user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fab32-122">Update the properties of a user object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fab32-123">属性</span><span class="sxs-lookup"><span data-stu-id="fab32-123">Properties</span></span>
|<span data-ttu-id="fab32-124">属性</span><span class="sxs-lookup"><span data-stu-id="fab32-124">Property</span></span>|<span data-ttu-id="fab32-125">类型</span><span class="sxs-lookup"><span data-stu-id="fab32-125">Type</span></span>|<span data-ttu-id="fab32-126">说明</span><span class="sxs-lookup"><span data-stu-id="fab32-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fab32-127">id</span><span class="sxs-lookup"><span data-stu-id="fab32-127">id</span></span>|<span data-ttu-id="fab32-128">String</span><span class="sxs-lookup"><span data-stu-id="fab32-128">String</span></span>|<span data-ttu-id="fab32-129">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fab32-129">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="fab32-130">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="fab32-130">deviceEnrollmentLimit</span></span>|<span data-ttu-id="fab32-131">Int32</span><span class="sxs-lookup"><span data-stu-id="fab32-131">Int32</span></span>|<span data-ttu-id="fab32-132">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="fab32-132">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="fab32-133">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="fab32-133">Allowed values are 5 or 1000.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fab32-134">关系</span><span class="sxs-lookup"><span data-stu-id="fab32-134">Relationships</span></span>
<span data-ttu-id="fab32-135">无</span><span class="sxs-lookup"><span data-stu-id="fab32-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fab32-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fab32-136">JSON Representation</span></span>
<span data-ttu-id="fab32-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fab32-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```



