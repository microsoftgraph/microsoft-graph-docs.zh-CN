# <a name="actionstate-enum-type"></a><span data-ttu-id="17717-101">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="17717-101">actionState enum type</span></span>

> <span data-ttu-id="17717-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="17717-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17717-103">设备上的操作状态</span><span class="sxs-lookup"><span data-stu-id="17717-103">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="17717-104">成员</span><span class="sxs-lookup"><span data-stu-id="17717-104">Members</span></span>
|<span data-ttu-id="17717-105">成员</span><span class="sxs-lookup"><span data-stu-id="17717-105">Member</span></span>|<span data-ttu-id="17717-106">值</span><span class="sxs-lookup"><span data-stu-id="17717-106">Value</span></span>|<span data-ttu-id="17717-107">说明</span><span class="sxs-lookup"><span data-stu-id="17717-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17717-108">none</span><span class="sxs-lookup"><span data-stu-id="17717-108">none</span></span>|<span data-ttu-id="17717-109">0</span><span class="sxs-lookup"><span data-stu-id="17717-109">{0}</span></span>|<span data-ttu-id="17717-110">none</span><span class="sxs-lookup"><span data-stu-id="17717-110">Not a valid action state</span></span>|
|<span data-ttu-id="17717-111">待执行</span><span class="sxs-lookup"><span data-stu-id="17717-111">Pending</span></span>|<span data-ttu-id="17717-112">1</span><span class="sxs-lookup"><span data-stu-id="17717-112">-1</span></span>|<span data-ttu-id="17717-113">操作待执行</span><span class="sxs-lookup"><span data-stu-id="17717-113">Action is pending</span></span>|
|<span data-ttu-id="17717-114">已取消</span><span class="sxs-lookup"><span data-stu-id="17717-114">Canceled</span></span>|<span data-ttu-id="17717-115">2</span><span class="sxs-lookup"><span data-stu-id="17717-115">-2</span></span>|<span data-ttu-id="17717-116">操作已取消。</span><span class="sxs-lookup"><span data-stu-id="17717-116">Action has been cancelled.</span></span>|
|<span data-ttu-id="17717-117">活动</span><span class="sxs-lookup"><span data-stu-id="17717-117">active</span></span>|<span data-ttu-id="17717-118">3</span><span class="sxs-lookup"><span data-stu-id="17717-118">-3</span></span>|<span data-ttu-id="17717-119">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="17717-119">Action is active.</span></span>|
|<span data-ttu-id="17717-120">完成</span><span class="sxs-lookup"><span data-stu-id="17717-120">done</span></span>|<span data-ttu-id="17717-121">4</span><span class="sxs-lookup"><span data-stu-id="17717-121">-4</span></span>|<span data-ttu-id="17717-122">操作已完成，没有错误。</span><span class="sxs-lookup"><span data-stu-id="17717-122">Action completed without errors.</span></span>|
|<span data-ttu-id="17717-123">失败</span><span class="sxs-lookup"><span data-stu-id="17717-123">failed</span></span>|<span data-ttu-id="17717-124">5</span><span class="sxs-lookup"><span data-stu-id="17717-124">-5</span></span>|<span data-ttu-id="17717-125">操作失败</span><span class="sxs-lookup"><span data-stu-id="17717-125">Action failed</span></span>|
|<span data-ttu-id="17717-126">notSupported</span><span class="sxs-lookup"><span data-stu-id="17717-126">notSupported</span></span>|<span data-ttu-id="17717-127">6</span><span class="sxs-lookup"><span data-stu-id="17717-127">-6</span></span>|<span data-ttu-id="17717-128">不支持的操作。</span><span class="sxs-lookup"><span data-stu-id="17717-128">is not supported.</span></span>|








