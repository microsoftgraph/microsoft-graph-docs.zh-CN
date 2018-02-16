# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="a19cd-101">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="a19cd-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="a19cd-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a19cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a19cd-103">充当所有设备应用管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="a19cd-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="a19cd-104">方法</span><span class="sxs-lookup"><span data-stu-id="a19cd-104">Methods</span></span>
|<span data-ttu-id="a19cd-105">方法</span><span class="sxs-lookup"><span data-stu-id="a19cd-105">Method</span></span>|<span data-ttu-id="a19cd-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="a19cd-106">Return Type</span></span>|<span data-ttu-id="a19cd-107">说明</span><span class="sxs-lookup"><span data-stu-id="a19cd-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a19cd-108">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a19cd-108">Get deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_get.md)|[<span data-ttu-id="a19cd-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a19cd-109">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="a19cd-110">读取 [deviceAppManagement](../resources/intune_books_deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a19cd-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="a19cd-111">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a19cd-111">Update deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_update.md)|[<span data-ttu-id="a19cd-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a19cd-112">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="a19cd-113">更新 [deviceAppManagement](../resources/intune_books_deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a19cd-113">Update the properties of a [calendar](../resources/intune_books_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a19cd-114">属性</span><span class="sxs-lookup"><span data-stu-id="a19cd-114">Properties</span></span>
|<span data-ttu-id="a19cd-115">属性</span><span class="sxs-lookup"><span data-stu-id="a19cd-115">Property</span></span>|<span data-ttu-id="a19cd-116">类型</span><span class="sxs-lookup"><span data-stu-id="a19cd-116">Type</span></span>|<span data-ttu-id="a19cd-117">说明</span><span class="sxs-lookup"><span data-stu-id="a19cd-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a19cd-118">id</span><span class="sxs-lookup"><span data-stu-id="a19cd-118">id</span></span>|<span data-ttu-id="a19cd-119">String</span><span class="sxs-lookup"><span data-stu-id="a19cd-119">String</span></span>|<span data-ttu-id="a19cd-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a19cd-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a19cd-121">关系</span><span class="sxs-lookup"><span data-stu-id="a19cd-121">Relationships</span></span>
|<span data-ttu-id="a19cd-122">关系</span><span class="sxs-lookup"><span data-stu-id="a19cd-122">Relationship</span></span>|<span data-ttu-id="a19cd-123">类型</span><span class="sxs-lookup"><span data-stu-id="a19cd-123">Type</span></span>|<span data-ttu-id="a19cd-124">说明</span><span class="sxs-lookup"><span data-stu-id="a19cd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a19cd-125">managedEBooks</span><span class="sxs-lookup"><span data-stu-id="a19cd-125">managedEBooks</span></span>|<span data-ttu-id="a19cd-126">[managedEBook](../resources/intune_books_managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a19cd-126">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="a19cd-127">托管的电子书。</span><span class="sxs-lookup"><span data-stu-id="a19cd-127">The Managed eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a19cd-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a19cd-128">JSON Representation</span></span>
<span data-ttu-id="a19cd-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a19cd-129">Here is a JSON representation of the resource.</span></span>
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



