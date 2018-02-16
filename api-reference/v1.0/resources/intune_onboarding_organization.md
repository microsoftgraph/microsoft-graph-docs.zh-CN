# <a name="organization-resource-type"></a><span data-ttu-id="80e98-101">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="80e98-101">organization resource type</span></span>

> <span data-ttu-id="80e98-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80e98-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80e98-103">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="80e98-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="80e98-104">方法</span><span class="sxs-lookup"><span data-stu-id="80e98-104">Methods</span></span>
|<span data-ttu-id="80e98-105">方法</span><span class="sxs-lookup"><span data-stu-id="80e98-105">Method</span></span>|<span data-ttu-id="80e98-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="80e98-106">Return Type</span></span>|<span data-ttu-id="80e98-107">说明</span><span class="sxs-lookup"><span data-stu-id="80e98-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80e98-108">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="80e98-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="80e98-109">[organization](../resources/intune_onboarding_organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80e98-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="80e98-110">列出 [organization](../resources/intune_onboarding_organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80e98-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="80e98-111">获取 organization</span><span class="sxs-lookup"><span data-stu-id="80e98-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="80e98-112">organization</span><span class="sxs-lookup"><span data-stu-id="80e98-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="80e98-113">读取 [organization](../resources/intune_onboarding_organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80e98-113">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="80e98-114">更新 organization</span><span class="sxs-lookup"><span data-stu-id="80e98-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="80e98-115">organization</span><span class="sxs-lookup"><span data-stu-id="80e98-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="80e98-116">更新 [organization](../resources/intune_onboarding_organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80e98-116">Update the properties of a [calendar](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="80e98-117">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="80e98-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="80e98-118">Int32</span><span class="sxs-lookup"><span data-stu-id="80e98-118">Int32</span></span>|<span data-ttu-id="80e98-119">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="80e98-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="80e98-120">属性</span><span class="sxs-lookup"><span data-stu-id="80e98-120">Properties</span></span>
|<span data-ttu-id="80e98-121">属性</span><span class="sxs-lookup"><span data-stu-id="80e98-121">Property</span></span>|<span data-ttu-id="80e98-122">类型</span><span class="sxs-lookup"><span data-stu-id="80e98-122">Type</span></span>|<span data-ttu-id="80e98-123">说明</span><span class="sxs-lookup"><span data-stu-id="80e98-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80e98-124">id</span><span class="sxs-lookup"><span data-stu-id="80e98-124">id</span></span>|<span data-ttu-id="80e98-125">String</span><span class="sxs-lookup"><span data-stu-id="80e98-125">String</span></span>|<span data-ttu-id="80e98-126">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="80e98-126">The resource GUID for the security object is not valid.</span></span>|
|<span data-ttu-id="80e98-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="80e98-127">mobileDeviceManagementAuthority</span></span>|<span data-ttu-id="80e98-128">String</span><span class="sxs-lookup"><span data-stu-id="80e98-128">String</span></span>|<span data-ttu-id="80e98-129">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="80e98-129">Mobile device management authority.</span></span> <span data-ttu-id="80e98-130">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="80e98-130">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80e98-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="80e98-131">Relationships</span></span>
<span data-ttu-id="80e98-132">无</span><span class="sxs-lookup"><span data-stu-id="80e98-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80e98-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80e98-133">JSON Representation</span></span>
<span data-ttu-id="80e98-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80e98-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```



