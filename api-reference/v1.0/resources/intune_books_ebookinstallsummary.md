# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="e66d9-101">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e66d9-101">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="e66d9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e66d9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e66d9-103">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="e66d9-103">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="e66d9-104">方法</span><span class="sxs-lookup"><span data-stu-id="e66d9-104">Methods</span></span>
|<span data-ttu-id="e66d9-105">方法</span><span class="sxs-lookup"><span data-stu-id="e66d9-105">Method</span></span>|<span data-ttu-id="e66d9-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="e66d9-106">Return Type</span></span>|<span data-ttu-id="e66d9-107">说明</span><span class="sxs-lookup"><span data-stu-id="e66d9-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e66d9-108">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e66d9-108">Get eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_get.md)|[<span data-ttu-id="e66d9-109">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e66d9-109">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="e66d9-110">读取 [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e66d9-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="e66d9-111">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e66d9-111">Update eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_update.md)|[<span data-ttu-id="e66d9-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e66d9-112">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="e66d9-113">更新 [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e66d9-113">Update the properties of a [calendar](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e66d9-114">属性</span><span class="sxs-lookup"><span data-stu-id="e66d9-114">Properties</span></span>
|<span data-ttu-id="e66d9-115">属性</span><span class="sxs-lookup"><span data-stu-id="e66d9-115">Property</span></span>|<span data-ttu-id="e66d9-116">类型</span><span class="sxs-lookup"><span data-stu-id="e66d9-116">Type</span></span>|<span data-ttu-id="e66d9-117">说明</span><span class="sxs-lookup"><span data-stu-id="e66d9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e66d9-118">id</span><span class="sxs-lookup"><span data-stu-id="e66d9-118">id</span></span>|<span data-ttu-id="e66d9-119">String</span><span class="sxs-lookup"><span data-stu-id="e66d9-119">String</span></span>|<span data-ttu-id="e66d9-120">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e66d9-120">Key of the setting.</span></span>|
|<span data-ttu-id="e66d9-121">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e66d9-121">installedDeviceCount</span></span>|<span data-ttu-id="e66d9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e66d9-122">Int32</span></span>|<span data-ttu-id="e66d9-123">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="e66d9-123">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="e66d9-124">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e66d9-124">failedDeviceCount</span></span>|<span data-ttu-id="e66d9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e66d9-125">Int32</span></span>|<span data-ttu-id="e66d9-126">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="e66d9-126">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="e66d9-127">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e66d9-127">notInstalledDeviceCount</span></span>|<span data-ttu-id="e66d9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e66d9-128">Int32</span></span>|<span data-ttu-id="e66d9-129">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="e66d9-129">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="e66d9-130">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="e66d9-130">installedUserCount</span></span>|<span data-ttu-id="e66d9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e66d9-131">Int32</span></span>|<span data-ttu-id="e66d9-132">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="e66d9-132">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="e66d9-133">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="e66d9-133">failedUserCount</span></span>|<span data-ttu-id="e66d9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e66d9-134">Int32</span></span>|<span data-ttu-id="e66d9-135">有 1 个或以上设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="e66d9-135">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="e66d9-136">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="e66d9-136">notInstalledUserCount</span></span>|<span data-ttu-id="e66d9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e66d9-137">Int32</span></span>|<span data-ttu-id="e66d9-138">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="e66d9-138">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e66d9-139">关系</span><span class="sxs-lookup"><span data-stu-id="e66d9-139">Relationships</span></span>
<span data-ttu-id="e66d9-140">无</span><span class="sxs-lookup"><span data-stu-id="e66d9-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e66d9-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e66d9-141">JSON Representation</span></span>
<span data-ttu-id="e66d9-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e66d9-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```



