# <a name="devicemanagement-resource-type"></a><span data-ttu-id="bbbd6-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="bbbd6-101">deviceManagement resource type</span></span>

> <span data-ttu-id="bbbd6-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbbd6-103">充当设备管理下的 Android for Work 设置功能容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-103">Singleton entity that acts as a container for Android for Work settings functionality under device management.</span></span>
## <a name="methods"></a><span data-ttu-id="bbbd6-104">方法</span><span class="sxs-lookup"><span data-stu-id="bbbd6-104">Methods</span></span>
|<span data-ttu-id="bbbd6-105">方法</span><span class="sxs-lookup"><span data-stu-id="bbbd6-105">Method</span></span>|<span data-ttu-id="bbbd6-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="bbbd6-106">Return Type</span></span>|<span data-ttu-id="bbbd6-107">说明</span><span class="sxs-lookup"><span data-stu-id="bbbd6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bbbd6-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="bbbd6-108">Get deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_get.md)|[<span data-ttu-id="bbbd6-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="bbbd6-109">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="bbbd6-110">读取 [deviceManagement](../resources/intune_androidforwork_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="bbbd6-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="bbbd6-111">Update deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_update.md)|[<span data-ttu-id="bbbd6-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="bbbd6-112">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="bbbd6-113">更新 [deviceManagement](../resources/intune_androidforwork_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-113">Update the properties of a [calendar](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bbbd6-114">属性</span><span class="sxs-lookup"><span data-stu-id="bbbd6-114">Properties</span></span>
|<span data-ttu-id="bbbd6-115">属性</span><span class="sxs-lookup"><span data-stu-id="bbbd6-115">Property</span></span>|<span data-ttu-id="bbbd6-116">类型</span><span class="sxs-lookup"><span data-stu-id="bbbd6-116">Type</span></span>|<span data-ttu-id="bbbd6-117">说明</span><span class="sxs-lookup"><span data-stu-id="bbbd6-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbbd6-118">id</span><span class="sxs-lookup"><span data-stu-id="bbbd6-118">id</span></span>|<span data-ttu-id="bbbd6-119">String</span><span class="sxs-lookup"><span data-stu-id="bbbd6-119">String</span></span>|<span data-ttu-id="bbbd6-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bbbd6-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbbd6-121">关系</span><span class="sxs-lookup"><span data-stu-id="bbbd6-121">Relationships</span></span>
|<span data-ttu-id="bbbd6-122">关系</span><span class="sxs-lookup"><span data-stu-id="bbbd6-122">Relationship</span></span>|<span data-ttu-id="bbbd6-123">类型</span><span class="sxs-lookup"><span data-stu-id="bbbd6-123">Type</span></span>|<span data-ttu-id="bbbd6-124">说明</span><span class="sxs-lookup"><span data-stu-id="bbbd6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbbd6-125">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="bbbd6-125">androidForWorkSettings</span></span>|[<span data-ttu-id="bbbd6-126">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="bbbd6-126">androidForWorkSettings</span></span>](../resources/intune_androidforwork_androidforworksettings.md)|<span data-ttu-id="bbbd6-127">Android for Work 设置单例实体。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-127">The singleton Android for Work settings entity.</span></span>|
|<span data-ttu-id="bbbd6-128">androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="bbbd6-128">androidForWorkAppConfigurationSchemas</span></span>|<span data-ttu-id="bbbd6-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bbbd6-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="bbbd6-130">Android for Work 应用配置架构实体。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-130">Android for Work app configuration schema entities.</span></span>|
|<span data-ttu-id="bbbd6-131">androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="bbbd6-131">androidForWorkEnrollmentProfiles</span></span>|<span data-ttu-id="bbbd6-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bbbd6-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) collection</span></span>|<span data-ttu-id="bbbd6-133">Android for Work 注册配置文件实体。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-133">Android for Work enrollment profile entities.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbbd6-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bbbd6-134">JSON Representation</span></span>
<span data-ttu-id="bbbd6-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbbd6-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



