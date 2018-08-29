# <a name="reportroot-resource-type"></a><span data-ttu-id="56a27-101">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="56a27-101">reportRoot resource type</span></span>

> <span data-ttu-id="56a27-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="56a27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56a27-103">表示一个历史记录报告实例的资源。</span><span class="sxs-lookup"><span data-stu-id="56a27-103">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="56a27-104">方法</span><span class="sxs-lookup"><span data-stu-id="56a27-104">Methods</span></span>
|<span data-ttu-id="56a27-105">方法</span><span class="sxs-lookup"><span data-stu-id="56a27-105">Method</span></span>|<span data-ttu-id="56a27-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="56a27-106">Return Type</span></span>|<span data-ttu-id="56a27-107">说明</span><span class="sxs-lookup"><span data-stu-id="56a27-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56a27-108">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="56a27-108">Get reportRoot</span></span>](../api/intune_deviceconfig_reportroot_get.md)|[<span data-ttu-id="56a27-109">reportRoot</span><span class="sxs-lookup"><span data-stu-id="56a27-109">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="56a27-110">读取 [reportRoot](../resources/intune_deviceconfig_reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56a27-110">Read properties and relationships of the [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="56a27-111">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="56a27-111">Update reportRoot</span></span>](../api/intune_deviceconfig_reportroot_update.md)|[<span data-ttu-id="56a27-112">reportRoot</span><span class="sxs-lookup"><span data-stu-id="56a27-112">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="56a27-113">更新 [reportRoot](../resources/intune_deviceconfig_reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56a27-113">Update the properties of a [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="56a27-114">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="56a27-114">deviceConfigurationUserActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[<span data-ttu-id="56a27-115">报告</span><span class="sxs-lookup"><span data-stu-id="56a27-115">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="56a27-116">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="56a27-116">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="56a27-117">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="56a27-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="56a27-118">报告</span><span class="sxs-lookup"><span data-stu-id="56a27-118">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="56a27-119">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="56a27-119">Metadata for the device configuration device activity report</span></span>|

## <a name="relationships"></a><span data-ttu-id="56a27-120">关系</span><span class="sxs-lookup"><span data-stu-id="56a27-120">Relationships</span></span>
<span data-ttu-id="56a27-121">无</span><span class="sxs-lookup"><span data-stu-id="56a27-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56a27-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56a27-122">JSON Representation</span></span>
<span data-ttu-id="56a27-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56a27-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
}
```

## <a name="example"></a><span data-ttu-id="56a27-124">示例</span><span class="sxs-lookup"><span data-stu-id="56a27-124">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
