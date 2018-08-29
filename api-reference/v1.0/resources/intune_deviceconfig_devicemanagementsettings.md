# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="8f4cd-101">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f4cd-101">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="8f4cd-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8f4cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f4cd-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8f4cd-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8f4cd-104">属性</span><span class="sxs-lookup"><span data-stu-id="8f4cd-104">Properties</span></span>
|<span data-ttu-id="8f4cd-105">属性</span><span class="sxs-lookup"><span data-stu-id="8f4cd-105">Property</span></span>|<span data-ttu-id="8f4cd-106">类型</span><span class="sxs-lookup"><span data-stu-id="8f4cd-106">Type</span></span>|<span data-ttu-id="8f4cd-107">说明</span><span class="sxs-lookup"><span data-stu-id="8f4cd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f4cd-108">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="8f4cd-108">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="8f4cd-109">Int32</span><span class="sxs-lookup"><span data-stu-id="8f4cd-109">Int32</span></span>|<span data-ttu-id="8f4cd-110">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="8f4cd-110">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="8f4cd-111">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="8f4cd-111">Valid values 0 to 120</span></span>|
|<span data-ttu-id="8f4cd-112">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="8f4cd-112">isScheduledActionEnabled</span></span>|<span data-ttu-id="8f4cd-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f4cd-113">Boolean</span></span>|<span data-ttu-id="8f4cd-114">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="8f4cd-114">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="8f4cd-115">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="8f4cd-115">secureByDefault</span></span>|<span data-ttu-id="8f4cd-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f4cd-116">Boolean</span></span>|<span data-ttu-id="8f4cd-117">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="8f4cd-117">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f4cd-118">关系</span><span class="sxs-lookup"><span data-stu-id="8f4cd-118">Relationships</span></span>
<span data-ttu-id="8f4cd-119">无</span><span class="sxs-lookup"><span data-stu-id="8f4cd-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f4cd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f4cd-120">JSON Representation</span></span>
<span data-ttu-id="8f4cd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f4cd-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



