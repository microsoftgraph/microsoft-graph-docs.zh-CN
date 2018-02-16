# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="08ae0-101">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="08ae0-101">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="08ae0-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="08ae0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08ae0-103">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="08ae0-103">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="08ae0-104">属性</span><span class="sxs-lookup"><span data-stu-id="08ae0-104">Properties</span></span>
|<span data-ttu-id="08ae0-105">属性</span><span class="sxs-lookup"><span data-stu-id="08ae0-105">Property</span></span>|<span data-ttu-id="08ae0-106">类型</span><span class="sxs-lookup"><span data-stu-id="08ae0-106">Type</span></span>|<span data-ttu-id="08ae0-107">说明</span><span class="sxs-lookup"><span data-stu-id="08ae0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ae0-108">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="08ae0-108">platformBlocked</span></span>|<span data-ttu-id="08ae0-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="08ae0-109">Boolean</span></span>|<span data-ttu-id="08ae0-110">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="08ae0-110">Block the platform from enrolling</span></span>|
|<span data-ttu-id="08ae0-111">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="08ae0-111">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="08ae0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="08ae0-112">Boolean</span></span>|<span data-ttu-id="08ae0-113">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="08ae0-113">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="08ae0-114">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="08ae0-114">osMinimumVersion</span></span>|<span data-ttu-id="08ae0-115">String</span><span class="sxs-lookup"><span data-stu-id="08ae0-115">String</span></span>|<span data-ttu-id="08ae0-116">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="08ae0-116">Min OS version supported</span></span>|
|<span data-ttu-id="08ae0-117">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="08ae0-117">osMaximumVersion</span></span>|<span data-ttu-id="08ae0-118">String</span><span class="sxs-lookup"><span data-stu-id="08ae0-118">String</span></span>|<span data-ttu-id="08ae0-119">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="08ae0-119">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="08ae0-120">关系</span><span class="sxs-lookup"><span data-stu-id="08ae0-120">Relationships</span></span>
<span data-ttu-id="08ae0-121">无</span><span class="sxs-lookup"><span data-stu-id="08ae0-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08ae0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08ae0-122">JSON Representation</span></span>
<span data-ttu-id="08ae0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08ae0-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



