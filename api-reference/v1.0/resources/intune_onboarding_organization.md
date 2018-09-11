# <a name="organization-resource-type"></a><span data-ttu-id="41113-101">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="41113-101">organization resource type</span></span>

> <span data-ttu-id="41113-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="41113-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41113-103">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="41113-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="41113-104">方法</span><span class="sxs-lookup"><span data-stu-id="41113-104">Methods</span></span>
|<span data-ttu-id="41113-105">方法</span><span class="sxs-lookup"><span data-stu-id="41113-105">Method</span></span>|<span data-ttu-id="41113-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="41113-106">Return Type</span></span>|<span data-ttu-id="41113-107">说明</span><span class="sxs-lookup"><span data-stu-id="41113-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="41113-108">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="41113-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="41113-109">[organization](../resources/intune_onboarding_organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41113-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="41113-110">列出 [organization](../resources/intune_onboarding_organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41113-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="41113-111">获取 organization</span><span class="sxs-lookup"><span data-stu-id="41113-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="41113-112">组织</span><span class="sxs-lookup"><span data-stu-id="41113-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="41113-113">读取 [organization](../resources/intune_onboarding_organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41113-113">Read properties and relationships of the [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="41113-114">更新 organization</span><span class="sxs-lookup"><span data-stu-id="41113-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="41113-115">组织</span><span class="sxs-lookup"><span data-stu-id="41113-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="41113-116">更新 [organization](../resources/intune_onboarding_organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41113-116">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="41113-117">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="41113-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="41113-118">Int32</span><span class="sxs-lookup"><span data-stu-id="41113-118">Int32</span></span>|<span data-ttu-id="41113-119">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="41113-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="41113-120">属性</span><span class="sxs-lookup"><span data-stu-id="41113-120">Properties</span></span>
|<span data-ttu-id="41113-121">属性</span><span class="sxs-lookup"><span data-stu-id="41113-121">Property</span></span>|<span data-ttu-id="41113-122">类型</span><span class="sxs-lookup"><span data-stu-id="41113-122">Type</span></span>|<span data-ttu-id="41113-123">说明</span><span class="sxs-lookup"><span data-stu-id="41113-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41113-124">ID</span><span class="sxs-lookup"><span data-stu-id="41113-124">id</span></span>|<span data-ttu-id="41113-125">字符串</span><span class="sxs-lookup"><span data-stu-id="41113-125">String</span></span>|<span data-ttu-id="41113-126">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="41113-126">The GUID for the object.</span></span>|
|<span data-ttu-id="41113-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="41113-127">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="41113-128">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="41113-128">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="41113-p101">移动设备管理机构。 可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="41113-p101">Mobile device management authority. The possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41113-131">关系</span><span class="sxs-lookup"><span data-stu-id="41113-131">Relationships</span></span>
<span data-ttu-id="41113-132">无</span><span class="sxs-lookup"><span data-stu-id="41113-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="41113-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41113-133">JSON Representation</span></span>
<span data-ttu-id="41113-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41113-134">Here is a JSON representation of the resource.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->






