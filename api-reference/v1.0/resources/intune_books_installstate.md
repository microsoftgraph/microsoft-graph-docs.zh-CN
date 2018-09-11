# <a name="installstate-enum-type"></a><span data-ttu-id="77556-101">installState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="77556-101">installState enum type</span></span>

> <span data-ttu-id="77556-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="77556-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77556-103">安装状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="77556-103">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="77556-104">成员</span><span class="sxs-lookup"><span data-stu-id="77556-104">Members</span></span>
|<span data-ttu-id="77556-105">成员</span><span class="sxs-lookup"><span data-stu-id="77556-105">Member</span></span>|<span data-ttu-id="77556-106">值</span><span class="sxs-lookup"><span data-stu-id="77556-106">Value</span></span>|<span data-ttu-id="77556-107">说明</span><span class="sxs-lookup"><span data-stu-id="77556-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77556-108">notApplicable</span><span class="sxs-lookup"><span data-stu-id="77556-108">NotApplicable</span></span>|<span data-ttu-id="77556-109">0</span><span class="sxs-lookup"><span data-stu-id="77556-109">{0}</span></span>|<span data-ttu-id="77556-110">不适用。</span><span class="sxs-lookup"><span data-stu-id="77556-110">Not applicable.</span></span>|
|<span data-ttu-id="77556-111">installed</span><span class="sxs-lookup"><span data-stu-id="77556-111">Installed</span></span>|<span data-ttu-id="77556-112">1</span><span class="sxs-lookup"><span data-stu-id="77556-112">-1</span></span>|<span data-ttu-id="77556-113">安装。</span><span class="sxs-lookup"><span data-stu-id="77556-113">Installed</span></span>|
|<span data-ttu-id="77556-114">failed</span><span class="sxs-lookup"><span data-stu-id="77556-114">failed</span></span>|<span data-ttu-id="77556-115">2</span><span class="sxs-lookup"><span data-stu-id="77556-115">-2</span></span>|<span data-ttu-id="77556-116">失败。</span><span class="sxs-lookup"><span data-stu-id="77556-116">failed.</span></span>|
|<span data-ttu-id="77556-117">notInstalled</span><span class="sxs-lookup"><span data-stu-id="77556-117">notInstalled</span></span>|<span data-ttu-id="77556-118">3</span><span class="sxs-lookup"><span data-stu-id="77556-118">-3</span></span>|<span data-ttu-id="77556-119">未安装。</span><span class="sxs-lookup"><span data-stu-id="77556-119">Not Installed.</span></span>|
|<span data-ttu-id="77556-120">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="77556-120">uninstallFailed</span></span>|<span data-ttu-id="77556-121">4</span><span class="sxs-lookup"><span data-stu-id="77556-121">-4</span></span>|<span data-ttu-id="77556-122">卸载失败。</span><span class="sxs-lookup"><span data-stu-id="77556-122">Uninstall Failed.</span></span>|
|<span data-ttu-id="77556-123">unknown</span><span class="sxs-lookup"><span data-stu-id="77556-123">unknown</span></span>|<span data-ttu-id="77556-124">5</span><span class="sxs-lookup"><span data-stu-id="77556-124">-5</span></span>|<span data-ttu-id="77556-125">未知。</span><span class="sxs-lookup"><span data-stu-id="77556-125">Unknown</span></span>|








