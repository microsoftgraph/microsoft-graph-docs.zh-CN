# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="c7e34-101">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7e34-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="c7e34-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c7e34-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7e34-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7e34-103">Not yet documented</span></span>

<span data-ttu-id="c7e34-104">继承自 [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c7e34-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7e34-105">属性</span><span class="sxs-lookup"><span data-stu-id="c7e34-105">Properties</span></span>
|<span data-ttu-id="c7e34-106">属性</span><span class="sxs-lookup"><span data-stu-id="c7e34-106">Property</span></span>|<span data-ttu-id="c7e34-107">类型</span><span class="sxs-lookup"><span data-stu-id="c7e34-107">Type</span></span>|<span data-ttu-id="c7e34-108">说明</span><span class="sxs-lookup"><span data-stu-id="c7e34-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e34-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="c7e34-109">scheduledInstallDay</span></span>|[<span data-ttu-id="c7e34-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="c7e34-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="c7e34-111">周中计划安装的一天。</span><span class="sxs-lookup"><span data-stu-id="c7e34-111">Scheduled Install Day in week Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="c7e34-112">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="c7e34-112">The possible values are `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, , , or .</span></span>|
|<span data-ttu-id="c7e34-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="c7e34-113">scheduledInstallTime</span></span>|<span data-ttu-id="c7e34-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c7e34-114">TimeOfDay</span></span>|<span data-ttu-id="c7e34-115">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="c7e34-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7e34-116">关系</span><span class="sxs-lookup"><span data-stu-id="c7e34-116">Relationships</span></span>
<span data-ttu-id="c7e34-117">无</span><span class="sxs-lookup"><span data-stu-id="c7e34-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7e34-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7e34-118">JSON Representation</span></span>
<span data-ttu-id="c7e34-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7e34-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsUpdateInstallScheduleType",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



