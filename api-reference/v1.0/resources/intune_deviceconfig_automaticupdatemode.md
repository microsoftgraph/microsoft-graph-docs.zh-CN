# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="9adf1-101">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9adf1-101">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="9adf1-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9adf1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9adf1-103">自动更新模式可能的赋值。</span><span class="sxs-lookup"><span data-stu-id="9adf1-103">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="9adf1-104">成员</span><span class="sxs-lookup"><span data-stu-id="9adf1-104">Members</span></span>
|<span data-ttu-id="9adf1-105">成员</span><span class="sxs-lookup"><span data-stu-id="9adf1-105">Member</span></span>|<span data-ttu-id="9adf1-106">值</span><span class="sxs-lookup"><span data-stu-id="9adf1-106">Value</span></span>|<span data-ttu-id="9adf1-107">说明</span><span class="sxs-lookup"><span data-stu-id="9adf1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9adf1-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="9adf1-108">UserDefined</span></span>|<span data-ttu-id="9adf1-109">0</span><span class="sxs-lookup"><span data-stu-id="9adf1-109">{0}</span></span>|<span data-ttu-id="9adf1-110">用户已定义，默认值，无特定意图。</span><span class="sxs-lookup"><span data-stu-id="9adf1-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="9adf1-111">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="9adf1-111">notifyDownload</span></span>|<span data-ttu-id="9adf1-112">1</span><span class="sxs-lookup"><span data-stu-id="9adf1-112">-1</span></span>|<span data-ttu-id="9adf1-113">通知下载。</span><span class="sxs-lookup"><span data-stu-id="9adf1-113">Notify on download.</span></span>|
|<span data-ttu-id="9adf1-114">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="9adf1-114">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="9adf1-115">2</span><span class="sxs-lookup"><span data-stu-id="9adf1-115">-2</span></span>|<span data-ttu-id="9adf1-116">维护期间自动安装。</span><span class="sxs-lookup"><span data-stu-id="9adf1-116">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="9adf1-117">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="9adf1-117">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="9adf1-118">3</span><span class="sxs-lookup"><span data-stu-id="9adf1-118">-3</span></span>|<span data-ttu-id="9adf1-119">维护期间自动安装和重新启动。</span><span class="sxs-lookup"><span data-stu-id="9adf1-119">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="9adf1-120">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="9adf1-120">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="9adf1-121">4</span><span class="sxs-lookup"><span data-stu-id="9adf1-121">-4</span></span>|<span data-ttu-id="9adf1-122">在计划时间自动安装并重新启动。</span><span class="sxs-lookup"><span data-stu-id="9adf1-122">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="9adf1-123">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="9adf1-123">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="9adf1-124">5</span><span class="sxs-lookup"><span data-stu-id="9adf1-124">-5</span></span>|<span data-ttu-id="9adf1-125">自动安装并重新启动，无需最终用户控制</span><span class="sxs-lookup"><span data-stu-id="9adf1-125">Auto-install and restart without end-user control</span></span>|








