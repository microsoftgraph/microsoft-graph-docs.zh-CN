# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="aab05-101">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="aab05-101">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="aab05-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aab05-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aab05-103">当共享 PC 上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="aab05-103">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="aab05-104">成员</span><span class="sxs-lookup"><span data-stu-id="aab05-104">Members</span></span>
|<span data-ttu-id="aab05-105">成员</span><span class="sxs-lookup"><span data-stu-id="aab05-105">Member</span></span>|<span data-ttu-id="aab05-106">值</span><span class="sxs-lookup"><span data-stu-id="aab05-106">Value</span></span>|<span data-ttu-id="aab05-107">说明</span><span class="sxs-lookup"><span data-stu-id="aab05-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aab05-108">immediate</span><span class="sxs-lookup"><span data-stu-id="aab05-108">   [-immediate]</span></span>|<span data-ttu-id="aab05-109">0</span><span class="sxs-lookup"><span data-stu-id="aab05-109">{0}</span></span>|<span data-ttu-id="aab05-110">立即删除。</span><span class="sxs-lookup"><span data-stu-id="aab05-110">Delete immediately.</span></span>|
|<span data-ttu-id="aab05-111">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="aab05-111">diskSpaceThreshold</span></span>|<span data-ttu-id="aab05-112">1</span><span class="sxs-lookup"><span data-stu-id="aab05-112">-1</span></span>|<span data-ttu-id="aab05-113">删除至磁盘空间阈值。</span><span class="sxs-lookup"><span data-stu-id="aab05-113">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="aab05-114">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="aab05-114">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="aab05-115">2</span><span class="sxs-lookup"><span data-stu-id="aab05-115">-2</span></span>|<span data-ttu-id="aab05-116">删除在磁盘空间阈值或非活动状态的阈值。</span><span class="sxs-lookup"><span data-stu-id="aab05-116">Delete at disk space threshold or inactive threshold.</span></span>|








