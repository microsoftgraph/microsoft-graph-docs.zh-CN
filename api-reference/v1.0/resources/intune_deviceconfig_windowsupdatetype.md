# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="dbe43-101">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dbe43-101">windowsUpdateType enum type</span></span>

> <span data-ttu-id="dbe43-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dbe43-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbe43-103">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="dbe43-103">Determines which branch devices will receive their updates from Possible values are: , , .</span></span>
## <a name="members"></a><span data-ttu-id="dbe43-104">成员</span><span class="sxs-lookup"><span data-stu-id="dbe43-104">Members</span></span>
|<span data-ttu-id="dbe43-105">成员</span><span class="sxs-lookup"><span data-stu-id="dbe43-105">Member</span></span>|<span data-ttu-id="dbe43-106">值</span><span class="sxs-lookup"><span data-stu-id="dbe43-106">Value</span></span>|<span data-ttu-id="dbe43-107">说明</span><span class="sxs-lookup"><span data-stu-id="dbe43-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbe43-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="dbe43-108">UserDefined</span></span>|<span data-ttu-id="dbe43-109">0</span><span class="sxs-lookup"><span data-stu-id="dbe43-109">{0}</span></span>|<span data-ttu-id="dbe43-110">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="dbe43-110">Allow the user to set.</span></span>|
|<span data-ttu-id="dbe43-111">all</span><span class="sxs-lookup"><span data-stu-id="dbe43-111">all</span></span>|<span data-ttu-id="dbe43-112">1</span><span class="sxs-lookup"><span data-stu-id="dbe43-112">-1</span></span>|<span data-ttu-id="dbe43-113">半年频道（定向）。</span><span class="sxs-lookup"><span data-stu-id="dbe43-113">Semi-Annual Channel (Targeted)</span></span> <span data-ttu-id="dbe43-114">设备从半年频道（定向）中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="dbe43-114">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="dbe43-115">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="dbe43-115">businessReadyOnly</span></span>|<span data-ttu-id="dbe43-116">2</span><span class="sxs-lookup"><span data-stu-id="dbe43-116">-2</span></span>|<span data-ttu-id="dbe43-117">半年频道。</span><span class="sxs-lookup"><span data-stu-id="dbe43-117">Semi-Annual Channel</span></span> <span data-ttu-id="dbe43-118">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="dbe43-118">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="dbe43-119">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="dbe43-119">windowsInsiderBuildFast</span></span>|<span data-ttu-id="dbe43-120">3</span><span class="sxs-lookup"><span data-stu-id="dbe43-120">-3</span></span>|<span data-ttu-id="dbe43-121">Windows 预览体验内部版本 - 快</span><span class="sxs-lookup"><span data-stu-id="dbe43-121">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="dbe43-122">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="dbe43-122">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="dbe43-123">4</span><span class="sxs-lookup"><span data-stu-id="dbe43-123">-4</span></span>|<span data-ttu-id="dbe43-124">Windows 预览体验内部版本 - 慢</span><span class="sxs-lookup"><span data-stu-id="dbe43-124">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="dbe43-125">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="dbe43-125">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="dbe43-126">5</span><span class="sxs-lookup"><span data-stu-id="dbe43-126">-5</span></span>|<span data-ttu-id="dbe43-127">发布 Windows 预览体验内部版本</span><span class="sxs-lookup"><span data-stu-id="dbe43-127">Release Windows Insider build</span></span>|








