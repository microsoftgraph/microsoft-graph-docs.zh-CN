# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="fdd0c-101">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdd0c-101">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="fdd0c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fdd0c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdd0c-103">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="fdd0c-103">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="fdd0c-104">属性</span><span class="sxs-lookup"><span data-stu-id="fdd0c-104">Properties</span></span>
|<span data-ttu-id="fdd0c-105">属性</span><span class="sxs-lookup"><span data-stu-id="fdd0c-105">Property</span></span>|<span data-ttu-id="fdd0c-106">类型</span><span class="sxs-lookup"><span data-stu-id="fdd0c-106">Type</span></span>|<span data-ttu-id="fdd0c-107">说明</span><span class="sxs-lookup"><span data-stu-id="fdd0c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdd0c-108">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="fdd0c-108">platformBlocked</span></span>|<span data-ttu-id="fdd0c-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdd0c-109">Boolean</span></span>|<span data-ttu-id="fdd0c-110">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="fdd0c-110">Block the platform from enrolling</span></span>|
|<span data-ttu-id="fdd0c-111">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="fdd0c-111">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="fdd0c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdd0c-112">Boolean</span></span>|<span data-ttu-id="fdd0c-113">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="fdd0c-113">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="fdd0c-114">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="fdd0c-114">osMinimumVersion</span></span>|<span data-ttu-id="fdd0c-115">String</span><span class="sxs-lookup"><span data-stu-id="fdd0c-115">String</span></span>|<span data-ttu-id="fdd0c-116">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="fdd0c-116">Min OS version supported</span></span>|
|<span data-ttu-id="fdd0c-117">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="fdd0c-117">osMaximumVersion</span></span>|<span data-ttu-id="fdd0c-118">String</span><span class="sxs-lookup"><span data-stu-id="fdd0c-118">String</span></span>|<span data-ttu-id="fdd0c-119">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="fdd0c-119">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdd0c-120">关系</span><span class="sxs-lookup"><span data-stu-id="fdd0c-120">Relationships</span></span>
<span data-ttu-id="fdd0c-121">无</span><span class="sxs-lookup"><span data-stu-id="fdd0c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fdd0c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdd0c-122">JSON Representation</span></span>
<span data-ttu-id="fdd0c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdd0c-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```








