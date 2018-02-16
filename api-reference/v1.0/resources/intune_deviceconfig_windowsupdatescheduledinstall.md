# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="c9ef9-101">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9ef9-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="c9ef9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c9ef9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9ef9-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c9ef9-103">Not yet documented</span></span>

<span data-ttu-id="c9ef9-104">继承自 [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c9ef9-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9ef9-105">属性</span><span class="sxs-lookup"><span data-stu-id="c9ef9-105">Properties</span></span>
|<span data-ttu-id="c9ef9-106">属性</span><span class="sxs-lookup"><span data-stu-id="c9ef9-106">Property</span></span>|<span data-ttu-id="c9ef9-107">类型</span><span class="sxs-lookup"><span data-stu-id="c9ef9-107">Type</span></span>|<span data-ttu-id="c9ef9-108">说明</span><span class="sxs-lookup"><span data-stu-id="c9ef9-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9ef9-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="c9ef9-109">scheduledInstallDay</span></span>|<span data-ttu-id="c9ef9-110">String</span><span class="sxs-lookup"><span data-stu-id="c9ef9-110">String</span></span>|<span data-ttu-id="c9ef9-111">一周内计划安装日的可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="c9ef9-111">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="c9ef9-112">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="c9ef9-112">scheduledInstallTime</span></span>|<span data-ttu-id="c9ef9-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c9ef9-113">TimeOfDay</span></span>|<span data-ttu-id="c9ef9-114">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="c9ef9-114">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9ef9-115">关系</span><span class="sxs-lookup"><span data-stu-id="c9ef9-115">Relationships</span></span>
<span data-ttu-id="c9ef9-116">无</span><span class="sxs-lookup"><span data-stu-id="c9ef9-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9ef9-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9ef9-117">JSON Representation</span></span>
<span data-ttu-id="c9ef9-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9ef9-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



