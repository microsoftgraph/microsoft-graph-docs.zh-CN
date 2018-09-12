# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="df656-101">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df656-101">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="df656-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="df656-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df656-103">允许该设备发送诊断和使用情况的遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="df656-103">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="df656-104">成员</span><span class="sxs-lookup"><span data-stu-id="df656-104">Members</span></span>
|<span data-ttu-id="df656-105">成员</span><span class="sxs-lookup"><span data-stu-id="df656-105">Member</span></span>|<span data-ttu-id="df656-106">值</span><span class="sxs-lookup"><span data-stu-id="df656-106">Value</span></span>|<span data-ttu-id="df656-107">说明</span><span class="sxs-lookup"><span data-stu-id="df656-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df656-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="df656-108">UserDefined</span></span>|<span data-ttu-id="df656-109">0</span><span class="sxs-lookup"><span data-stu-id="df656-109">{0}</span></span>|<span data-ttu-id="df656-110">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="df656-110">Allow the user to set.</span></span>|
|<span data-ttu-id="df656-111">none</span><span class="sxs-lookup"><span data-stu-id="df656-111">none</span></span>|<span data-ttu-id="df656-112">1</span><span class="sxs-lookup"><span data-stu-id="df656-112">-1</span></span>|<span data-ttu-id="df656-113">从操作系统组件不发送任何遥测数据。</span><span class="sxs-lookup"><span data-stu-id="df656-113">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="df656-114">注意：此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="df656-114">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="df656-115">在其他设备上使用此设置等效于将值设为 1。</span><span class="sxs-lookup"><span data-stu-id="df656-115">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="df656-116">basic</span><span class="sxs-lookup"><span data-stu-id="df656-116">Basic</span></span>|<span data-ttu-id="df656-117">2</span><span class="sxs-lookup"><span data-stu-id="df656-117">-2</span></span>|<span data-ttu-id="df656-118">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="df656-118">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="df656-119">enhanced</span><span class="sxs-lookup"><span data-stu-id="df656-119">enhanced presence</span></span>|<span data-ttu-id="df656-120">3</span><span class="sxs-lookup"><span data-stu-id="df656-120">-3</span></span>|<span data-ttu-id="df656-121">发送包括使用情况和见解数据的增强型遥测数据。</span><span class="sxs-lookup"><span data-stu-id="df656-121">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="df656-122">full</span><span class="sxs-lookup"><span data-stu-id="df656-122">Full</span></span>|<span data-ttu-id="df656-123">4</span><span class="sxs-lookup"><span data-stu-id="df656-123">-4</span></span>|<span data-ttu-id="df656-124">发送全 部遥测数据，包括诊断数据（如系统状态）。</span><span class="sxs-lookup"><span data-stu-id="df656-124">Sends full telemetry data including diagnostic data, such as system state.</span></span>|








