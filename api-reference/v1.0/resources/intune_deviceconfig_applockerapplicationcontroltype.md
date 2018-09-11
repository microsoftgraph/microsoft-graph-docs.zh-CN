# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="ddf7b-101">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ddf7b-101">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="ddf7b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ddf7b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddf7b-103">AppLocker 应用程序控制类型的可能值</span><span class="sxs-lookup"><span data-stu-id="ddf7b-103">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="ddf7b-104">成员</span><span class="sxs-lookup"><span data-stu-id="ddf7b-104">Members</span></span>
|<span data-ttu-id="ddf7b-105">成员</span><span class="sxs-lookup"><span data-stu-id="ddf7b-105">Member</span></span>|<span data-ttu-id="ddf7b-106">值</span><span class="sxs-lookup"><span data-stu-id="ddf7b-106">Value</span></span>|<span data-ttu-id="ddf7b-107">说明</span><span class="sxs-lookup"><span data-stu-id="ddf7b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddf7b-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ddf7b-108">notConfigured</span></span>|<span data-ttu-id="ddf7b-109">0</span><span class="sxs-lookup"><span data-stu-id="ddf7b-109">{0}</span></span>|<span data-ttu-id="ddf7b-110">设备默认值，未选择的应用程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="ddf7b-110">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="ddf7b-111">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ddf7b-111">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="ddf7b-112">1</span><span class="sxs-lookup"><span data-stu-id="ddf7b-112">-1</span></span>|<span data-ttu-id="ddf7b-113">强制使用 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="ddf7b-113">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="ddf7b-114">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ddf7b-114">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="ddf7b-115">2</span><span class="sxs-lookup"><span data-stu-id="ddf7b-115">-2</span></span>|<span data-ttu-id="ddf7b-116">审核 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="ddf7b-116">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="ddf7b-117">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ddf7b-117">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ddf7b-118">3</span><span class="sxs-lookup"><span data-stu-id="ddf7b-118">-3</span></span>|<span data-ttu-id="ddf7b-119">强制使用 Windows 组件、应用商店应用和智能锁柜。</span><span class="sxs-lookup"><span data-stu-id="ddf7b-119">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="ddf7b-120">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ddf7b-120">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ddf7b-121">4</span><span class="sxs-lookup"><span data-stu-id="ddf7b-121">-4</span></span>|<span data-ttu-id="ddf7b-122">审核 Windows 组件、应用商店应用和智能锁柜。</span><span class="sxs-lookup"><span data-stu-id="ddf7b-122">Audit Windows components, store apps and smart locker.</span></span>|








