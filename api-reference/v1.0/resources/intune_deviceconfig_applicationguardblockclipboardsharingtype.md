# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="95d92-101">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="95d92-101">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="95d92-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="95d92-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95d92-103">ApplicationGuardBlockClipboardSharingType 可能的赋值</span><span class="sxs-lookup"><span data-stu-id="95d92-103">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="95d92-104">成员</span><span class="sxs-lookup"><span data-stu-id="95d92-104">Members</span></span>
|<span data-ttu-id="95d92-105">成员</span><span class="sxs-lookup"><span data-stu-id="95d92-105">Member</span></span>|<span data-ttu-id="95d92-106">值</span><span class="sxs-lookup"><span data-stu-id="95d92-106">Value</span></span>|<span data-ttu-id="95d92-107">说明</span><span class="sxs-lookup"><span data-stu-id="95d92-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95d92-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="95d92-108">notConfigured</span></span>|<span data-ttu-id="95d92-109">0</span><span class="sxs-lookup"><span data-stu-id="95d92-109">{0}</span></span>|<span data-ttu-id="95d92-110">未配置</span><span class="sxs-lookup"><span data-stu-id="95d92-110">Not configured</span></span>|
|<span data-ttu-id="95d92-111">blockBoth</span><span class="sxs-lookup"><span data-stu-id="95d92-111">blockBoth</span></span>|<span data-ttu-id="95d92-112">1</span><span class="sxs-lookup"><span data-stu-id="95d92-112">-1</span></span>|<span data-ttu-id="95d92-113">阻止从从主机到容器和从容器到主机通过剪贴板共享数据</span><span class="sxs-lookup"><span data-stu-id="95d92-113">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|
|<span data-ttu-id="95d92-114">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="95d92-114">blockHostToContainer</span></span>|<span data-ttu-id="95d92-115">2</span><span class="sxs-lookup"><span data-stu-id="95d92-115">-2</span></span>|<span data-ttu-id="95d92-116">阻止从主机到容器通过剪贴板共享数据</span><span class="sxs-lookup"><span data-stu-id="95d92-116">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|
|<span data-ttu-id="95d92-117">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="95d92-117">blockContainerToHost</span></span>|<span data-ttu-id="95d92-118">3</span><span class="sxs-lookup"><span data-stu-id="95d92-118">-3</span></span>|<span data-ttu-id="95d92-119">阻止从容器到主机通过剪贴板共享数据</span><span class="sxs-lookup"><span data-stu-id="95d92-119">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|
|<span data-ttu-id="95d92-120">blockNone</span><span class="sxs-lookup"><span data-stu-id="95d92-120">blockNone</span></span>|<span data-ttu-id="95d92-121">4</span><span class="sxs-lookup"><span data-stu-id="95d92-121">-4</span></span>|<span data-ttu-id="95d92-122">阻止从从主机到容器和从容器到主机通过剪贴板共享数据</span><span class="sxs-lookup"><span data-stu-id="95d92-122">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span>|








