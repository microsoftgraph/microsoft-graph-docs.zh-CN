# <a name="compliancestate-enum-type"></a><span data-ttu-id="9aec5-101">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9aec5-101">complianceState enum type</span></span>

> <span data-ttu-id="9aec5-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9aec5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9aec5-103">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="9aec5-103">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="9aec5-104">成员</span><span class="sxs-lookup"><span data-stu-id="9aec5-104">Members</span></span>
|<span data-ttu-id="9aec5-105">成员</span><span class="sxs-lookup"><span data-stu-id="9aec5-105">Member</span></span>|<span data-ttu-id="9aec5-106">值</span><span class="sxs-lookup"><span data-stu-id="9aec5-106">Value</span></span>|<span data-ttu-id="9aec5-107">说明</span><span class="sxs-lookup"><span data-stu-id="9aec5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aec5-108">unknown</span><span class="sxs-lookup"><span data-stu-id="9aec5-108">unknown</span></span>|<span data-ttu-id="9aec5-109">0</span><span class="sxs-lookup"><span data-stu-id="9aec5-109">{0}</span></span>|<span data-ttu-id="9aec5-110">未知。</span><span class="sxs-lookup"><span data-stu-id="9aec5-110">Unknown</span></span>|
|<span data-ttu-id="9aec5-111">compliant</span><span class="sxs-lookup"><span data-stu-id="9aec5-111">Compliant</span></span>|<span data-ttu-id="9aec5-112">1</span><span class="sxs-lookup"><span data-stu-id="9aec5-112">-1</span></span>|<span data-ttu-id="9aec5-113">合规。</span><span class="sxs-lookup"><span data-stu-id="9aec5-113">Compliant</span></span>|
|<span data-ttu-id="9aec5-114">noncompliant</span><span class="sxs-lookup"><span data-stu-id="9aec5-114">noncompliant</span></span>|<span data-ttu-id="9aec5-115">2</span><span class="sxs-lookup"><span data-stu-id="9aec5-115">-2</span></span>|<span data-ttu-id="9aec5-116">设备不合规，并阻止访问企业资源。</span><span class="sxs-lookup"><span data-stu-id="9aec5-116">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="9aec5-117">conflict</span><span class="sxs-lookup"><span data-stu-id="9aec5-117">Conflict</span></span>|<span data-ttu-id="9aec5-118">3</span><span class="sxs-lookup"><span data-stu-id="9aec5-118">-3</span></span>|<span data-ttu-id="9aec5-119">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="9aec5-119">Conflict with other rules.</span></span>|
|<span data-ttu-id="9aec5-120">error</span><span class="sxs-lookup"><span data-stu-id="9aec5-120">error</span></span>|<span data-ttu-id="9aec5-121">4</span><span class="sxs-lookup"><span data-stu-id="9aec5-121">-4</span></span>|<span data-ttu-id="9aec5-122">错误。</span><span class="sxs-lookup"><span data-stu-id="9aec5-122">Error.</span></span>|
|<span data-ttu-id="9aec5-123">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="9aec5-123">inGracePeriod</span></span>|<span data-ttu-id="9aec5-124">254</span><span class="sxs-lookup"><span data-stu-id="9aec5-124">254</span></span>|<span data-ttu-id="9aec5-125">设备不合规，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="9aec5-125">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="9aec5-126">configManager</span><span class="sxs-lookup"><span data-stu-id="9aec5-126">configManager</span></span>|<span data-ttu-id="9aec5-127">255</span><span class="sxs-lookup"><span data-stu-id="9aec5-127">255 characters</span></span>|<span data-ttu-id="9aec5-128">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="9aec5-128">Managed by Config Manager</span></span>|








