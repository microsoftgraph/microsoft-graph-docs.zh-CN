# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="8b54b-101">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8b54b-101">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="8b54b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8b54b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b54b-103">代表设备的剪贴板可能在应用程序之间共享的级别</span><span class="sxs-lookup"><span data-stu-id="8b54b-103">The level to which the clipboard may be shared between apps on the managed device.</span></span>
## <a name="members"></a><span data-ttu-id="8b54b-104">成员</span><span class="sxs-lookup"><span data-stu-id="8b54b-104">Members</span></span>
|<span data-ttu-id="8b54b-105">成员</span><span class="sxs-lookup"><span data-stu-id="8b54b-105">Member</span></span>|<span data-ttu-id="8b54b-106">值</span><span class="sxs-lookup"><span data-stu-id="8b54b-106">Value</span></span>|<span data-ttu-id="8b54b-107">说明</span><span class="sxs-lookup"><span data-stu-id="8b54b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b54b-108">allApps</span><span class="sxs-lookup"><span data-stu-id="8b54b-108">allApps</span></span>|<span data-ttu-id="8b54b-109">0</span><span class="sxs-lookup"><span data-stu-id="8b54b-109">{0}</span></span>|<span data-ttu-id="8b54b-110">在所有的应用程序（托管或非托管）之间共享</span><span class="sxs-lookup"><span data-stu-id="8b54b-110">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="8b54b-111">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="8b54b-111">managedAppsWithPasteIn</span></span>|<span data-ttu-id="8b54b-112">1</span><span class="sxs-lookup"><span data-stu-id="8b54b-112">-1</span></span>|<span data-ttu-id="8b54b-113">允许在启用粘贴的所有托管应用程序之间共享</span><span class="sxs-lookup"><span data-stu-id="8b54b-113">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="8b54b-114">managedApps</span><span class="sxs-lookup"><span data-stu-id="8b54b-114">managedApps</span></span>|<span data-ttu-id="8b54b-115">2</span><span class="sxs-lookup"><span data-stu-id="8b54b-115">-2</span></span>|<span data-ttu-id="8b54b-116">允许在所有的托管应用程序之间共享</span><span class="sxs-lookup"><span data-stu-id="8b54b-116">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="8b54b-117">blocked</span><span class="sxs-lookup"><span data-stu-id="8b54b-117">blocked</span></span>|<span data-ttu-id="8b54b-118">3</span><span class="sxs-lookup"><span data-stu-id="8b54b-118">-3</span></span>|<span data-ttu-id="8b54b-119">禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="8b54b-119">Sharing between apps is disabled</span></span>|








