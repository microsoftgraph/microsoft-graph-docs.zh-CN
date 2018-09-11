# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="a1ef9-101">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a1ef9-101">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="a1ef9-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1ef9-103">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-103">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="a1ef9-104">成员</span><span class="sxs-lookup"><span data-stu-id="a1ef9-104">Members</span></span>
|<span data-ttu-id="a1ef9-105">成员</span><span class="sxs-lookup"><span data-stu-id="a1ef9-105">Member</span></span>|<span data-ttu-id="a1ef9-106">值</span><span class="sxs-lookup"><span data-stu-id="a1ef9-106">Value</span></span>|<span data-ttu-id="a1ef9-107">说明</span><span class="sxs-lookup"><span data-stu-id="a1ef9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ef9-108">notRegistered</span><span class="sxs-lookup"><span data-stu-id="a1ef9-108">notRegistered</span></span>|<span data-ttu-id="a1ef9-109">0</span><span class="sxs-lookup"><span data-stu-id="a1ef9-109">{0}</span></span>|<span data-ttu-id="a1ef9-110">未注册设备。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-110">The device is not registered.</span></span>|
|<span data-ttu-id="a1ef9-111">registered</span><span class="sxs-lookup"><span data-stu-id="a1ef9-111">Registered</span></span>|<span data-ttu-id="a1ef9-112">2</span><span class="sxs-lookup"><span data-stu-id="a1ef9-112">-2</span></span>|<span data-ttu-id="a1ef9-113">已注册设备。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-113">The device is registered.</span></span>|
|<span data-ttu-id="a1ef9-114">revoked</span><span class="sxs-lookup"><span data-stu-id="a1ef9-114">Revoked</span></span>|<span data-ttu-id="a1ef9-115">3</span><span class="sxs-lookup"><span data-stu-id="a1ef9-115">-3</span></span>|<span data-ttu-id="a1ef9-116">已阻止、擦除或停用该设备。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-116">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="a1ef9-117">keyConflict</span><span class="sxs-lookup"><span data-stu-id="a1ef9-117">keyConflict</span></span>|<span data-ttu-id="a1ef9-118">4</span><span class="sxs-lookup"><span data-stu-id="a1ef9-118">-4</span></span>|<span data-ttu-id="a1ef9-119">设备存在重大冲突。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-119">The device has a key conflict.</span></span>|
|<span data-ttu-id="a1ef9-120">approvalPending</span><span class="sxs-lookup"><span data-stu-id="a1ef9-120">approvalPending</span></span>|<span data-ttu-id="a1ef9-121">5</span><span class="sxs-lookup"><span data-stu-id="a1ef9-121">-5</span></span>|<span data-ttu-id="a1ef9-122">设备处于待审批状态。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-122">The device is pending approval.</span></span>|
|<span data-ttu-id="a1ef9-123">certificateReset</span><span class="sxs-lookup"><span data-stu-id="a1ef9-123">certificateReset</span></span>|<span data-ttu-id="a1ef9-124">6</span><span class="sxs-lookup"><span data-stu-id="a1ef9-124">-6</span></span>|<span data-ttu-id="a1ef9-125">设备证书已被重置。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-125">The device certificate has been reset.</span></span>|
|<span data-ttu-id="a1ef9-126">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="a1ef9-126">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="a1ef9-127">7</span><span class="sxs-lookup"><span data-stu-id="a1ef9-127">-7</span></span>|<span data-ttu-id="a1ef9-128">未注册设备以及待处理注册。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-128">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="a1ef9-129">unknown</span><span class="sxs-lookup"><span data-stu-id="a1ef9-129">unknown</span></span>|<span data-ttu-id="a1ef9-130">8</span><span class="sxs-lookup"><span data-stu-id="a1ef9-130">-8</span></span>|<span data-ttu-id="a1ef9-131">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="a1ef9-131">The device registration status is unknown.</span></span>|








