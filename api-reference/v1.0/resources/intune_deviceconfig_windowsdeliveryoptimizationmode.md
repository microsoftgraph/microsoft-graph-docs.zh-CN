# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="327bf-101">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="327bf-101">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="327bf-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="327bf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="327bf-103">节点分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="327bf-103">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="327bf-104">成员</span><span class="sxs-lookup"><span data-stu-id="327bf-104">Members</span></span>
|<span data-ttu-id="327bf-105">成员</span><span class="sxs-lookup"><span data-stu-id="327bf-105">Member</span></span>|<span data-ttu-id="327bf-106">值</span><span class="sxs-lookup"><span data-stu-id="327bf-106">Value</span></span>|<span data-ttu-id="327bf-107">说明</span><span class="sxs-lookup"><span data-stu-id="327bf-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="327bf-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="327bf-108">UserDefined</span></span>|<span data-ttu-id="327bf-109">0</span><span class="sxs-lookup"><span data-stu-id="327bf-109">{0}</span></span>|<span data-ttu-id="327bf-110">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="327bf-110">Allow the user to set.</span></span>|
|<span data-ttu-id="327bf-111">httpOnly</span><span class="sxs-lookup"><span data-stu-id="327bf-111">httpOnly</span></span>|<span data-ttu-id="327bf-112">1</span><span class="sxs-lookup"><span data-stu-id="327bf-112">-1</span></span>|<span data-ttu-id="327bf-113">仅HTTP ，无对等互联</span><span class="sxs-lookup"><span data-stu-id="327bf-113">HTTP only, no peering</span></span>|
|<span data-ttu-id="327bf-114">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="327bf-114">httpWithPeeringNat</span></span>|<span data-ttu-id="327bf-115">2</span><span class="sxs-lookup"><span data-stu-id="327bf-115">-2</span></span>|<span data-ttu-id="327bf-116">OS 默认 – Http 与同一网络地址转换器后进行对等互联混合</span><span class="sxs-lookup"><span data-stu-id="327bf-116">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="327bf-117">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="327bf-117">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="327bf-118">3</span><span class="sxs-lookup"><span data-stu-id="327bf-118">-3</span></span>|<span data-ttu-id="327bf-119">HTTP 与跨专用组对等互联混合</span><span class="sxs-lookup"><span data-stu-id="327bf-119">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="327bf-120">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="327bf-120">httpWithInternetPeering</span></span>|<span data-ttu-id="327bf-121">4</span><span class="sxs-lookup"><span data-stu-id="327bf-121">-4</span></span>|<span data-ttu-id="327bf-122">HTTP 与 Internet 对等互联混合</span><span class="sxs-lookup"><span data-stu-id="327bf-122">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="327bf-123">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="327bf-123">simpleDownload</span></span>|<span data-ttu-id="327bf-124">99</span><span class="sxs-lookup"><span data-stu-id="327bf-124">-99</span></span>|<span data-ttu-id="327bf-125">无对等互联的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="327bf-125">Simple download mode with no peering</span></span>|
|<span data-ttu-id="327bf-126">bypassMode</span><span class="sxs-lookup"><span data-stu-id="327bf-126">bypassMode</span></span>|<span data-ttu-id="327bf-127">100</span><span class="sxs-lookup"><span data-stu-id="327bf-127">100%</span></span>|<span data-ttu-id="327bf-128">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="327bf-128">Bypass mode.</span></span> <span data-ttu-id="327bf-129">不要使用传递优化，而应使用BITS</span><span class="sxs-lookup"><span data-stu-id="327bf-129">Do not use Delivery Optimization and use BITS instead</span></span>|








