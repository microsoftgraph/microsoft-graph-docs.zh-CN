# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="a7f99-101">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a7f99-101">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="a7f99-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7f99-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7f99-103">与 Apple 大宗采购计划令牌相关的可能同步状态。</span><span class="sxs-lookup"><span data-stu-id="a7f99-103">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="a7f99-104">成员</span><span class="sxs-lookup"><span data-stu-id="a7f99-104">Members</span></span>
|<span data-ttu-id="a7f99-105">成员</span><span class="sxs-lookup"><span data-stu-id="a7f99-105">Member</span></span>|<span data-ttu-id="a7f99-106">值</span><span class="sxs-lookup"><span data-stu-id="a7f99-106">Value</span></span>|<span data-ttu-id="a7f99-107">说明</span><span class="sxs-lookup"><span data-stu-id="a7f99-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7f99-108">无</span><span class="sxs-lookup"><span data-stu-id="a7f99-108">none</span></span>|<span data-ttu-id="a7f99-109">0</span><span class="sxs-lookup"><span data-stu-id="a7f99-109">{0}</span></span>|<span data-ttu-id="a7f99-110">默认状态。</span><span class="sxs-lookup"><span data-stu-id="a7f99-110">Default status</span></span>|
|<span data-ttu-id="a7f99-111">inProgress</span><span class="sxs-lookup"><span data-stu-id="a7f99-111">InProgress</span></span>|<span data-ttu-id="a7f99-112">1</span><span class="sxs-lookup"><span data-stu-id="a7f99-112">-1</span></span>|<span data-ttu-id="a7f99-113">上次同步正在进行中。</span><span class="sxs-lookup"><span data-stu-id="a7f99-113">Last Sync in progress.</span></span>|
|<span data-ttu-id="a7f99-114">已完成</span><span class="sxs-lookup"><span data-stu-id="a7f99-114">completed()</span></span>|<span data-ttu-id="a7f99-115">2</span><span class="sxs-lookup"><span data-stu-id="a7f99-115">-2</span></span>|<span data-ttu-id="a7f99-116">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="a7f99-116">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="a7f99-117">failed</span><span class="sxs-lookup"><span data-stu-id="a7f99-117">failed</span></span>|<span data-ttu-id="a7f99-118">3</span><span class="sxs-lookup"><span data-stu-id="a7f99-118">-3</span></span>|<span data-ttu-id="a7f99-119">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="a7f99-119">Last Sync failed.</span></span>|



