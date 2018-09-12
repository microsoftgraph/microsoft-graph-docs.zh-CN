# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="e8abc-101">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e8abc-101">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="e8abc-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8abc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8abc-103">设备 Exchange 访问状态。</span><span class="sxs-lookup"><span data-stu-id="e8abc-103">Device Exchange Access State summary</span></span>
## <a name="members"></a><span data-ttu-id="e8abc-104">成员</span><span class="sxs-lookup"><span data-stu-id="e8abc-104">Members</span></span>
|<span data-ttu-id="e8abc-105">成员</span><span class="sxs-lookup"><span data-stu-id="e8abc-105">Member</span></span>|<span data-ttu-id="e8abc-106">值</span><span class="sxs-lookup"><span data-stu-id="e8abc-106">Value</span></span>|<span data-ttu-id="e8abc-107">说明</span><span class="sxs-lookup"><span data-stu-id="e8abc-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8abc-108">无</span><span class="sxs-lookup"><span data-stu-id="e8abc-108">none</span></span>|<span data-ttu-id="e8abc-109">0</span><span class="sxs-lookup"><span data-stu-id="e8abc-109">{0}</span></span>|<span data-ttu-id="e8abc-110">没有从 Exchange 中发现访问状态</span><span class="sxs-lookup"><span data-stu-id="e8abc-110">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="e8abc-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e8abc-111">unknown</span></span>|<span data-ttu-id="e8abc-112">1</span><span class="sxs-lookup"><span data-stu-id="e8abc-112">-1</span></span>|<span data-ttu-id="e8abc-113">到 Exchange 的设备访问状态是未知</span><span class="sxs-lookup"><span data-stu-id="e8abc-113">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="e8abc-114">allowed</span><span class="sxs-lookup"><span data-stu-id="e8abc-114">Allowed</span></span>|<span data-ttu-id="e8abc-115">2</span><span class="sxs-lookup"><span data-stu-id="e8abc-115">-2</span></span>|<span data-ttu-id="e8abc-116">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="e8abc-116">Device has access to Exchange</span></span>|
|<span data-ttu-id="e8abc-117">blocked</span><span class="sxs-lookup"><span data-stu-id="e8abc-117">blocked</span></span>|<span data-ttu-id="e8abc-118">3</span><span class="sxs-lookup"><span data-stu-id="e8abc-118">-3</span></span>|<span data-ttu-id="e8abc-119">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="e8abc-119">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="e8abc-120">quarantined</span><span class="sxs-lookup"><span data-stu-id="e8abc-120">quarantined</span></span>|<span data-ttu-id="e8abc-121">4</span><span class="sxs-lookup"><span data-stu-id="e8abc-121">-4</span></span>|<span data-ttu-id="e8abc-122">设备在 Exchange 中被隔离</span><span class="sxs-lookup"><span data-stu-id="e8abc-122">Device is Quarantined in Exchange</span></span>|








