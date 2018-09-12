# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="e0284-101">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e0284-101">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="e0284-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0284-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0284-103">代表向其应用程序数据进行加密托管的应用程序级别</span><span class="sxs-lookup"><span data-stu-id="e0284-103">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="e0284-104">成员</span><span class="sxs-lookup"><span data-stu-id="e0284-104">Members</span></span>
|<span data-ttu-id="e0284-105">成员</span><span class="sxs-lookup"><span data-stu-id="e0284-105">Member</span></span>|<span data-ttu-id="e0284-106">值</span><span class="sxs-lookup"><span data-stu-id="e0284-106">Value</span></span>|<span data-ttu-id="e0284-107">说明</span><span class="sxs-lookup"><span data-stu-id="e0284-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0284-108">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="e0284-108">useDeviceSettings</span></span>|<span data-ttu-id="e0284-109">0</span><span class="sxs-lookup"><span data-stu-id="e0284-109">{0}</span></span>|<span data-ttu-id="e0284-110">应用程序数据根据设备默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="e0284-110">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="e0284-111">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="e0284-111">afterDeviceRestart</span></span>|<span data-ttu-id="e0284-112">1</span><span class="sxs-lookup"><span data-stu-id="e0284-112">-1</span></span>|<span data-ttu-id="e0284-113">应用程序数据在设备重新启动时进行加密。</span><span class="sxs-lookup"><span data-stu-id="e0284-113">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="e0284-114">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="e0284-114">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="e0284-115">2</span><span class="sxs-lookup"><span data-stu-id="e0284-115">-2</span></span>|<span data-ttu-id="e0284-116">与此策略关联的应用程序数据在设备锁定时进行加密，文件中打开的数据除外</span><span class="sxs-lookup"><span data-stu-id="e0284-116">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="e0284-117">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e0284-117">whenDeviceLocked</span></span>|<span data-ttu-id="e0284-118">3</span><span class="sxs-lookup"><span data-stu-id="e0284-118">-3</span></span>|<span data-ttu-id="e0284-119">与此策略关联的应用程序数据在设备锁定时进行加密</span><span class="sxs-lookup"><span data-stu-id="e0284-119">App data associated with this policy is encrypted when the device is locked</span></span>|








