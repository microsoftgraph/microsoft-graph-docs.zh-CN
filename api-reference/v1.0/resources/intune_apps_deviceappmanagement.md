# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="aea4d-101">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="aea4d-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="aea4d-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aea4d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aea4d-103">充当所有设备应用管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="aea4d-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="aea4d-104">方法</span><span class="sxs-lookup"><span data-stu-id="aea4d-104">Methods</span></span>
|<span data-ttu-id="aea4d-105">方法</span><span class="sxs-lookup"><span data-stu-id="aea4d-105">Method</span></span>|<span data-ttu-id="aea4d-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="aea4d-106">Return Type</span></span>|<span data-ttu-id="aea4d-107">说明</span><span class="sxs-lookup"><span data-stu-id="aea4d-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aea4d-108">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="aea4d-108">Get deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_get.md)|[<span data-ttu-id="aea4d-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="aea4d-109">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="aea4d-110">读取 [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aea4d-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="aea4d-111">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="aea4d-111">Update deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_update.md)|[<span data-ttu-id="aea4d-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="aea4d-112">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="aea4d-113">更新 [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aea4d-113">Update the properties of a [calendar](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aea4d-114">属性</span><span class="sxs-lookup"><span data-stu-id="aea4d-114">Properties</span></span>
|<span data-ttu-id="aea4d-115">属性</span><span class="sxs-lookup"><span data-stu-id="aea4d-115">Property</span></span>|<span data-ttu-id="aea4d-116">类型</span><span class="sxs-lookup"><span data-stu-id="aea4d-116">Type</span></span>|<span data-ttu-id="aea4d-117">说明</span><span class="sxs-lookup"><span data-stu-id="aea4d-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea4d-118">id</span><span class="sxs-lookup"><span data-stu-id="aea4d-118">id</span></span>|<span data-ttu-id="aea4d-119">String</span><span class="sxs-lookup"><span data-stu-id="aea4d-119">String</span></span>|<span data-ttu-id="aea4d-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aea4d-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aea4d-121">关系</span><span class="sxs-lookup"><span data-stu-id="aea4d-121">Relationships</span></span>
|<span data-ttu-id="aea4d-122">关系</span><span class="sxs-lookup"><span data-stu-id="aea4d-122">Relationship</span></span>|<span data-ttu-id="aea4d-123">类型</span><span class="sxs-lookup"><span data-stu-id="aea4d-123">Type</span></span>|<span data-ttu-id="aea4d-124">说明</span><span class="sxs-lookup"><span data-stu-id="aea4d-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea4d-125">mobileApps</span><span class="sxs-lookup"><span data-stu-id="aea4d-125">mobileApps</span></span>|<span data-ttu-id="aea4d-126">[mobileApp](../resources/intune_apps_mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aea4d-126">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="aea4d-127">移动应用。</span><span class="sxs-lookup"><span data-stu-id="aea4d-127">The mobile apps.</span></span>|
|<span data-ttu-id="aea4d-128">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="aea4d-128">mobileAppCategories</span></span>|<span data-ttu-id="aea4d-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aea4d-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="aea4d-130">移动应用类别。</span><span class="sxs-lookup"><span data-stu-id="aea4d-130">The mobile app categories.</span></span>|
|<span data-ttu-id="aea4d-131">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="aea4d-131">mobileAppConfigurations</span></span>|<span data-ttu-id="aea4d-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aea4d-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="aea4d-133">托管设备移动应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="aea4d-133">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aea4d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aea4d-134">JSON Representation</span></span>
<span data-ttu-id="aea4d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aea4d-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



