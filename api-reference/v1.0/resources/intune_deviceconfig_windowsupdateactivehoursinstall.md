# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="651c0-101">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="651c0-101">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="651c0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="651c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="651c0-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="651c0-103">Not yet documented</span></span>

<span data-ttu-id="651c0-104">继承自 [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="651c0-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="651c0-105">属性</span><span class="sxs-lookup"><span data-stu-id="651c0-105">Properties</span></span>
|<span data-ttu-id="651c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="651c0-106">Property</span></span>|<span data-ttu-id="651c0-107">类型</span><span class="sxs-lookup"><span data-stu-id="651c0-107">Type</span></span>|<span data-ttu-id="651c0-108">说明</span><span class="sxs-lookup"><span data-stu-id="651c0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="651c0-109">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="651c0-109">activeHoursStart</span></span>|<span data-ttu-id="651c0-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="651c0-110">TimeOfDay</span></span>|<span data-ttu-id="651c0-111">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="651c0-111">Active Hours Start</span></span>|
|<span data-ttu-id="651c0-112">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="651c0-112">activeHoursEnd</span></span>|<span data-ttu-id="651c0-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="651c0-113">TimeOfDay</span></span>|<span data-ttu-id="651c0-114">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="651c0-114">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="651c0-115">关系</span><span class="sxs-lookup"><span data-stu-id="651c0-115">Relationships</span></span>
<span data-ttu-id="651c0-116">无</span><span class="sxs-lookup"><span data-stu-id="651c0-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="651c0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="651c0-117">JSON Representation</span></span>
<span data-ttu-id="651c0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="651c0-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```








