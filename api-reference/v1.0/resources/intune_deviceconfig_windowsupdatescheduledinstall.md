# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="ffdc2-101">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffdc2-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="ffdc2-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ffdc2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffdc2-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ffdc2-103">Not yet documented</span></span>

<span data-ttu-id="ffdc2-104">继承自 [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc2-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ffdc2-105">属性</span><span class="sxs-lookup"><span data-stu-id="ffdc2-105">Properties</span></span>
|<span data-ttu-id="ffdc2-106">属性</span><span class="sxs-lookup"><span data-stu-id="ffdc2-106">Property</span></span>|<span data-ttu-id="ffdc2-107">类型</span><span class="sxs-lookup"><span data-stu-id="ffdc2-107">Type</span></span>|<span data-ttu-id="ffdc2-108">说明</span><span class="sxs-lookup"><span data-stu-id="ffdc2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffdc2-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="ffdc2-109">scheduledInstallDay</span></span>|[<span data-ttu-id="ffdc2-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="ffdc2-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="ffdc2-111">周中的计划安装一天。</span><span class="sxs-lookup"><span data-stu-id="ffdc2-111">Scheduled Install Day in week.</span></span> <span data-ttu-id="ffdc2-112">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="ffdc2-112">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="ffdc2-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="ffdc2-113">scheduledInstallTime</span></span>|<span data-ttu-id="ffdc2-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ffdc2-114">TimeOfDay</span></span>|<span data-ttu-id="ffdc2-115">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="ffdc2-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffdc2-116">关系</span><span class="sxs-lookup"><span data-stu-id="ffdc2-116">Relationships</span></span>
<span data-ttu-id="ffdc2-117">无</span><span class="sxs-lookup"><span data-stu-id="ffdc2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ffdc2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffdc2-118">JSON Representation</span></span>
<span data-ttu-id="ffdc2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffdc2-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



